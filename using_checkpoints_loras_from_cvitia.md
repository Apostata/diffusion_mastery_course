# Using checkpoints and LoRAs from CivitAI.
by [José Carlos Rodrigues Antonio](https://www.udemy.com/user/jose-carlos-rodrigues-antonio/) at https://www.udemy.com/course/diffusion-mastery-flux-stable-diffusion-midjourney-more/learn/lecture/45859067#questions/22505495

In Google Colab, you need to add the following codes:
```
!pip install pygit2==1.15.1
%cd /content
!git clone https://github.com/lllyasviel/Fooocus.git
%cd /content/Fooocus
```
then

from google.colab import drive
drive.mount('/content/drive')
After that, you need to execute both codes and log in to your Google Drive account. You need to have downloaded the checkpoints and loras you intended to use in Google Drive. I created a folder called "AI", then inside of it I created 2 folders, one called "Checkpoints" and the other called "LoRAs", as you can see in the following code snippet, which you should run:
```
# Models
!cp "/content/drive/MyDrive/AI/Checkpoints/[NameOfTheCheckpoint].safetensors" "/content/Fooocus/models/checkpoints"
# LoRAs
!cp "/content/drive/MyDrive/AI/LoRAs/[NameOfTheLoRA].safetensors" "/content/Fooocus/models/loras"
```
[NameOfTheCheckpoint] and [NameOfTheLoRA] represents the name of the files in Google Drive you intended to copy to Google Colab.

Then we run Fooocus:

`!python entry_with_update.py --share --always-high-vram`


Since Google Colab doesn't keep the generated images stored, after you use Fooocus and end the execution of the previous code, you need to run the following code:

`!cp -r "/content/Fooocus/outputs/" "/content/drive/MyDrive/AI"`

That way, Google Colab will copy the images from the outputs folder to your Google Drive folder (in my case, the folder "AI").

[BACK TO Fooocus UI](./fooocus_ui.md)\
[BACK TO BEGIN](./README.md)