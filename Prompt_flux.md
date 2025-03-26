# Prompt Engineering iN Flux Models
The proccess to generate images with Flux is very similar than between other IA models, so the [Prompt Engineering Basics](./Prompt_enginneering.md) are the same, but there are some differences that you need to know.

Different from Stable Diffusion, models, Flux doesn't have negative prompts.
You can, and should, be very specific in your prompt, yu can use about 255 tokens in your prompt, but the more specific you are, the better the result will be.

sample of a prompt in Flux:
`An image of a woman with fair skin and natural, wavy hair styled in soft curls andround her face. Shae has defined eyebrows and light-colored eyes that draw attention. She's dressed in a red and navy plaid shirt with top unbuttoned to show a white undershirt, and the sleeves rolled up to the forearms. The woman is casuallu leaning against a weathered blue door frame with peeling paint, adding rustic charm to the scene. Her arms are crossed or resting in front of her, and she has a soft, contemplative expression on her face.`

## Flux prompt generators
[Flux prompt generator on huggingface](https://huggingface.co/spaces/gokaygokay/FLUX-Prompt-Generator)
[Flux primpt wizard ChatGPT](https://chatgpt.com/g/g-6PGP543zE-flux-prompt-wizard)

## Flux Loras
[Flux loras collection](https://huggingface.co/XLabs-AI/flux-lora-collection)

Test prompt: `A close-up of a stunningly beautiful tattooed goth singer mid-performance, gripping the microphone with passion. Her long, silky black hair flows wildly as she sings, eyes closed in deep emotion. The spotlight casts a moody glow on her flawless pale skin, highlighting her high cheekbones and dark, dramatic makeup. The smoky concert atmosphere enhances the scene. Behind her, a massive LED screen displays the band's name, **"Infernus"**, in a fiery gothic font, glowing red against the dark stage.`