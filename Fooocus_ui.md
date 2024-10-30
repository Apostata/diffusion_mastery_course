# Fooocus UI
Fooocus is a interface that you can use to generate images with Stable Diffusion. It is a very simple and easy to use interface that you can use to generate images with Stable Diffusion.

## How to use Fooocus
There ar 2 ways to use Fooocus:
* Locally
* In the cloud

[GitHub](https://github.com/lllyasviel/Fooocus)


### Locally
Just follow the instructions in the [Fooocus GitHub repository](https://github.com/lllyasviel/Fooocus)

### Cloud (Google Colab)
Go to the github repository and click on the [`Open in Colab`](https://colab.research.google.com/github/lllyasviel/Fooocus/blob/main/fooocus_colab.ipynb) button. Then you can use the interface in the cloud.

![Fooocus](./assets/fooocus_colab.png)

Before you start using Fooocus in the colab notebook, go to the `Runtime` menu and click on `Change runtime type`. Then select `GPU` in the `Hardware accelerator` dropdown.

![Change runtime type](./assets/fooocus_colab2.png)
![Change runtime type](./assets/fooocus_colab3.png)

Then click on save and you are ready to use Fooocus in the cloud.
run the first cell to install the dependencies and then run the second cell to start the interface.

![Run on colab](./assets/fooocus_colab4.png)

You may want to se this [Using checkpoints and LoRAs from CivitAI.](./using_checkpoints_loras_from_cvitia.md) to use checkpoints and LoRAs from CivitAI.

## The interface
The interface is very simple and easy to use. here is the initial view.

![Initial view](./assets/fooocus_ui.png)

There ar 3 checkboxes that you can use to change the settings of the image generation process.
* Advanced: If you want to use advanced settings, check this box.
* Input Image: If you want to use an input image, check this box and upload the image.
* Enhance: If you want to enhance the image, check this box.
  
**You can enable more than one checkbox at the same time.**

### Advanced settings
![Advanced settings](./assets/fooocus_ui_advanced_tab.png)

#### Settings Tab
##### Pressets
The presset is a simpler way to change the model that will be used to generate the image. You can select the presset that you want to use in the dropdown.

##### Performance
You can change the performance settings to make the image generation faster or slower. You can select the performance that you want to use in the radio buttons.
Faster the image generation, lower is the number of steps and the quality of the image.

##### Aspect Ratio
You can change the aspect ratio of the image. You can select the aspect ratio that you want to use in the radio buttons.

##### Image Number
You can change the number of images that will be generated. You can select the number of images that you want to generate in the slide button.

##### Output Format
You can change the output format of the image. You can select the output format that you want to use in the radio buttons.
There are 3 options:
* PNG - Portable Network Graphics - recommended
* JPEG - Joint Photographic Experts Group
* WEBP - WebP image format

##### Negative Prompt
You can type a negative prompt to generate the image. You can type the negative prompt that you want to use in the text box.

##### Random Seed
You can change the random seed of the image. You can unchek the random and type the seed that you want to use in the text box.

##### History log
You can see the history log of the image generation process. You can see the history log by clicking on the button.
The history log is a list of the images that were generated with the settings that were used.

#### Styles Tab
The styles tab is where you can change the styles of the image. You can change the styles of the image by clicking on the buttons.
also you can improve the prompt with the `Fooocus V2`, `Fooocus Enhance`, `Fooocus Sharp` styles, that already are checked by default with the `Initial` Presset.
All styles show a image preview of the style if you hover the mouse over the button.

#### Models Tab
The models tab is where you can change the models that will be used to generate the image. You can change the models by clicking on the Dropdown model button.
You also can use LoRAs, that are a way to use a model that was trained with a specific prompt. You can use LoRAs by clicking on the Dropdown LoRA button, selecting the LoRA that you want to use and at the right you will have the `Weight` slider to change the weight of the LoRA.

#### Advanced Tab
##### Guidance Scale
Is how much the IA will follow the prompt. You can change the guidance scale by clicking on the slide button.
Best values are between 3 and 7
##### Image Sharpness

##### Documentation
You can see the documentation of the image generation process. You can see the documentation by clicking on the button.
Here is the direct link to the [documentation](https://github.com/lllyasviel/Fooocus/discussions/117)

##### Developer Debug Mode
Advanced settings for developers. You can see the developer debug mode by clicking on the button.

### Enhance settings
![Enhance settings](./assets/fooocus_ui_enhance_tab.png)

#### Upscale or Variation
##### Upscale or Variation
You can change the upscale or variation of the image. You can select the upscale or variation that you want to use in the radio buttons.

##### Order of Processing
Use before or after the image generation process. You can select the order of processing that you want to use in the radio buttons.

### Input Image settings
![Input Image settings](./assets/fooocus_ui_input_image_tab.png)

#### Upscale or Variation
as in the enhance settings, you can change the upscale or variation of the image. You can select the upscale or variation that you want to use in the radio buttons.

#### Image Prompt
You can upload an image to generate the image. You can upload the image by clicking on the button.

#### Inpaint or Outpaint
You can inpaint or outpaint the image

#### Describe
This will get the prompt from the image. You can get the prompt from the image by uploading the image and clicking on the button.

#### Enhance
Same as the enhance settings, you can enhance the image.

#### Metadata
Get the metadata from the image. You can get the metadata from the image by uploading the image and clicking on the button.
Metadata is the data that describes the image, for example, the size of the image, the format of the image, the date that the image was created, the model used to generate this image, etc.

## Extra
As de default checkpoint of `Fooocus` is Juggernaut XL, here is a link to guide a good prompt for this model: [Juggernaut XL Prompt Guide](https://learn.rundiffusion.com/prompt-guide-for-juggernaut-xi-and-xii/)

[BACK to Stable Diffusion models](./stable_difusion.md)\
[BACK TO BEGIN](./README.md)