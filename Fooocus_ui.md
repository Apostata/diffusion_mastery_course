# Fooocus UI
Fooocus is a interface that you can use to generate images with Stable Diffusion. It is a very simple and easy to use interface that you can use to generate images with Stable Diffusion.

Summary:
- [Fooocus UI](#fooocus-ui)
	- [How to use Fooocus](#how-to-use-fooocus)
		- [Locally](#locally)
		- [Cloud (Google Colab)](#cloud-google-colab)
	- [The interface](#the-interface)
		- [Advanced settings checkbox](#advanced-settings-checkbox)
		- [Enhanced settings checkbox](#enhanced-settings-checkbox)
		- [Input Image settings checkbox](#input-image-settings-checkbox)
	- [Extra](#extra)

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

### Advanced settings checkbox

The advanced settings checkbox is where you can change things like the performance, aspect ratio, image number, output format, negative prompt, random seed, history log, guidance scale, image sharpness, inpaint respective field, and documentation.\
[GO TO Advanced settings checkbox content](./Fooocus_ui_advanced_checkbox.md)

### Enhanced settings checkbox

The enhanced settings checkbox is where you can change things like the upscaling, order of processing, detection prompt, enhancement positive prompt, detection, inpaint, inpaint engine, inpaint denoising strength.\
[GO TO Enhanced settings checkbox content](./Fooocus_ui_enhanced_checkbox.md)

### Input Image settings checkbox

The input image settings checkbox is where you can change things like the inpaint method, inpaint prompt, original prompt, inpaint respective field, and details method. Ever with a selected image, you can change the prompt and inpaint method to generate a new image.\
[GO TO Input Image settings checkbox content](./Fooocus_ui_input_image_checkbox.md)

## Extra
As de default checkpoint of `Fooocus` is Juggernaut XL, here is a link to guide a good prompt for this model: [Juggernaut XL Prompt Guide](https://learn.rundiffusion.com/prompt-guide-for-juggernaut-xi-and-xii/)

[BACK to Stable Diffusion models](./stable_difusion.md)\
[BACK TO BEGIN](./README.MD)