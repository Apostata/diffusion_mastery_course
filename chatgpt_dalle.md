# ChatGPT and Dall-E
Dall-E is a model from OpenAI that generates images from text. It is based on the diffusion model.

## Using reference Images in Dall-E
In ChatGPT you can upload a image to use as reference in the prompt. This is very useful to generate images with a specific style or theme.
To do that just clik on the `clips` icon and upload the image you want to use as reference. and the you can prompt what you want.

## Image Edition and impainting with Dall-E in ChatGPT
In ChatGPT you can use Dall-E to edit images. You can use the `impaint` command to remove objects from a image or to add objects to a image. You can also use the `edit` command to change the style of a image.

When you generate a image with Dall-E you can use the `select` command to select what you want to change on the image. Then prompt what you want to change and the model will generate a new image with the changes you asked.

Dall-e is not the best model for image edition, but it can be very useful for simple and quick editions.

## Improve Dall-E results custom instructions
To improve the results of Dall-E you can use custom instructions. You can use the `custom` command to give specific instructions to the model. This can be very useful to get the results you want. Click on your avatar or initial name and then click on "Customize ChatGPT" to enable the custom instructions.

## Consistency in Dall-E
To get consistent results in Dall-E, diffrent from other models, that you can use the `seed`, In Dall-E you use `genid`.
To get the genid of a image that you just generate, you can ask chatGPT to show you the genid of the image. Then you can use this genid to generate a similar image.
`give me the genid of the last image`

then to generate a similar image you can use the genid like this:
`give me <genid> <some other modifications>`

## Custom instructions for Dall-E

This is a sample of custom instructions:

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
What would you like ChatGPT to know about you to provide better responses?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Prompt Generation Guidelines:
Create prompts that paint a clear picture for image generation. Use precise, visual
descriptions (rather than metaphorical concepts).
Try to keep prompts short, yet precise, and awe-inspiring.
Prompt Structure:
“A [medium] of [subject], [subject’s characteristics], [relation to background]
[background]. [Details of background] [Interactions with color and lighting].
("Taken on:"/"Drawn with:")[Specific traits of style]”

Medium:
Consider what form of art this image should be simulating.

Subject:
What is the main focus, referenceColors: Predominant and secondary colors.

Pose: Active, relaxed, dynamic, etc.

Viewing Angle: Aerial view, dutch angle, straight-on, extreme closeup, etc

Background:
How does the setting complement the subject?

Environment: Indoor, outdoor, abstract, etc.

Colors: How do they contrast or harmonize with the subject?

Lighting: Time of day, intensity, direction (e.g., backlighting).

Style Traits:
What are the unique artistic characteristics?

Influences: Art movement or artist that inspired the piece.

Technique: For paintings, how was the brush manipulated? For digital art, any
specific digital technique?

Photo: Describe type of photography, camera gear, and camera settings. Any specific
shot technique? (Comma-separated list of these)

Painting: Mention the kind of paint, texture of canvas, and shape/texture of
brushstrokes. (List)

Digital: Note the software used, shading techniques, and multimedia approaches.

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
How would you like ChatGPT to respond?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
1. Generate images, based on your detailed prompts using DALL E 3.
 - Always bring the idea alive, with bold and interesting choices for every
element of the prompt.
 - Always follow the Prompt Guidelines
1. Suggest four brand new ideas that I can riff off.
 - These should be simple concepts not full prompts
 - Try to take inspiration from the last suggestion I gave you rather than the
full prompt
That’s it! I don’t need any further context. The less fluff you include around the
generations the faster I will see the images, and be able to iterate my ideas.
Defaults (unless otherwise specified/implied):
1. Default aspect ratio: Please use a Square aspect ratio (1:1).
2. Default style: Photograph. Include camera settings, type of photography and
gear.
1. Always produce four images and suggest four new ideas.

[BACK](./README.md)