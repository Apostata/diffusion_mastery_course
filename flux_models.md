# Flux models

Flux models are a class of generative models that are based on the flux process. The flux process is a process that describes how a system evolves over time. In the context of generative models, the flux process is used to model the distribution of data. The idea is to start with a simple distribution, such as a Gaussian distribution, and then apply a series of transformations to it to gradually transform it into the target distribution. The key insight behind flux models is that the process of transforming a simple distribution into a complex distribution can be done in a reversible way, which allows us to generate samples from the target distribution by starting with samples from the simple distribution and applying the reverse transformations.
Flux models tend to be more stable and easier to train than diffusion models, making them a popular choice for generative modeling tasks. They have been used in a wide range of applications, including image generation, text-to-image synthesis, and style transfer, hoeever they require a lot of VRAM.

Flux models, diferent from Stable Diffusion, are very good at generation images with text. They are also very good at generating images from text descriptions by starting with a noisy, random image and refining it step-by-step. Through this gradual "flux" process, the model removes the noise in a way that aligns with the given description, resulting in a clear and detailed image. These models have learned to generate realistic and high-quality images, capturing intricate details based on vast amounts of training data, making them very effective in creative applications like art generation and visual design.*

## Flux models are better than Stable Diffusion models?

Flux models are better than Stable Diffusion models in some aspects, like the training process, the quality of the generated images, generating texts in images and the time to generate the images. However, Flux models require a lot of VRAM to train and generate images, so you need to have a good GPU to use them. Stable Diffusion models are easier to train and generate images, but they are not as good as Flux models in terms of image quality, text in images and training time.

Here is a playground to FLux models:

[Flux Pro](https://fal.ai/models/fal-ai/flux-pro/v1.1)

Here you will able to see every model that Flux has to offer, and you can test them out with your own images.
[Flux Dashboard](https://fal.ai/dashboard)

[Colab Flux Notebook with realism lora gradio](https://colab.research.google.com/github/camenduru/flux-jupyter/blob/main/flux.1-dev-realism-lora-gradio_jupyter.ipynb)
This notebook use Gradio Ui to test the model with your own images.

## Flux Dev or schnell models and machine requirements 
[Flux 16+VRAM module](https://huggingface.co/black-forest-labs/FLUX.1-dev) - is a model that requires at least 16GB of VRAM to run. If you have a GPU with less than 16GB of VRAM, you will not be able to run this model. If you have a GPU with 16GB of VRAM or more, you will be able to run this model.\

[Flux 8VRAM module](https://huggingface.co/XLabs-AI/flux-dev-fp8) - is a model that requires at least 8GB of VRAM to run. If you have a GPU with less than 8GB of VRAM, you will not be able to run this model. If you have a GPU with 16GB of VRAM or more, you will be able to run this model.

[Quantized Flux model ](https://huggingface.co/city96/FLUX.1-dev-gguf) - is a model to run in weaker GPUs, it requires at least 4GB of VRAM to run. If you have a GPU with less than 4GB of VRAM, you will not be able to run this model. If you have a GPU with 4GB of VRAM or more, you will be able to run this model.

If you have a machine taht can run the 16+VRAM module, download the `flux-dev.safetensors` or `flux-schnell.safetensors`

If you have a machine that can run the 8VRAM module, download the `flux-dev-fp8.safetensors` an so on.\

**Aways download: `ae.safetensors`. from [Flux 16+VRAM module](https://huggingface.co/black-forest-labs/FLUX.1-dev)and put this file on the `VAE` folder**


### Text Encoders
[Text Encoder](https://huggingface.co/lllyasviel/flux_text_encoders/tree/main) 

donwload the saftensors according to the model your machine can run.\
fp16, fp8\
and the `clip_l.safetensors`

https://github.com/lllyasviel/stable-diffusion-webui-forge/discussions/1050

[BACK TO BEGIN](./README.MD)