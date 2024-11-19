# Input Image settings
![Input Image settings](./assets/fooocus_ui_input_image_tab.png)

## Upscale or Variation
as in the enhance settings, you can change the upscale or variation of the image. You can select the upscale or variation that you want to use in the radio buttons.

## Image Prompt
You can upload an image to generate the image. You can upload the image by clicking on the button.

## Inpaint or Outpaint
You can inpaint or outpaint the image
 let's consider this initial prompt: `a half body photo of a beautiful indigenous lady, 40 yo, in the nature, big smile, brown hazel eyes, ponytail, dark makeup, hyperdetailed photography, soft light` 

let's change the color of the woman's eyes in the image.

* Inpaint - The AI will inpaint the image. This is useful when you want to change, add, or remove some parts or details of the image.
![Inpaint image](./assets/inpaint1.png)

changed prompt: `a half body photo of a beautiful indigenous lady, 40 yo, in the nature, big smile, brigth green eyes, ponytail, dark makeup, hyperdetailed photography, soft light`

| original image                             | inpainted image                        | inpainted image and prompt change                           |
| ------------------------------------------ | -------------------------------------- | ----------------------------------------------------------- |
| ![original](./assets/inpaint_original.png) | ![inpaint](./assets/inpaint_after.png) | ![inpaint prompt change](./assets/inpaint_after_prompt.png) |

the above image is the result of the inpaint process with the inpaint method seted to `Improve Detail (face, hand, eyes, etc.)`


| inpainted hair                                      | inpainted background                                      |
| --------------------------------------------------- | --------------------------------------------------------- |
| ![inpaint hair](./assets/inpaint_after_modify1.png) | ![inpaint background](./assets/inpaint_after_modify2.png) |

the above image is the result of the inpaint process with the inpaint method seted to `Modify Content (add objects, change background, etc.)`


* Outpaint - The AI will outpaint the image. This is useful when you want to change the resolution, making the image bigger or smaller.
  
Original prompt: `beautiful Afro american brazilian woman, long hair, eyeglasses, casual clothing, sitting at desk, wrinting a book, laptop, home office, indoor, nightlight, spot light, focus medium shot`

![Outpaint image](./assets/outpaint.png)

| original image                              | outpainted image left                   | outpainted image right  and left              |
| ------------------------------------------- | --------------------------------------- | --------------------------------------------- |
| ![original](./assets/outpaint_original.png) | ![outpaint](./assets/outpaint_left.png) | ![outpaint](./assets/outpaint_left_right.png) |

### Fix malformed hands
You can fix the malformed hands of the image. You can fix the malformed hands by using inpainting.

Original prompt: `beautiful brazilian woman, long hair, eyeglasses, casual clothing, sitting at desk, cheerful expression, smiling, waving, laptop, home office, indoor, nightlight, spot light, focus medium shot`

![Fix malformed hands](./assets/fix_hands.png)

| 1. original image                            | 2. details method                          | 3. inpaint prompt & modified content method           |
| -------------------------------------------- | ------------------------------------------ | ----------------------------------------------------- |
| ![original](./assets/fix_hands_original.png) | ![inpaint](./assets/fix_hands_details.png) | ![inpaint](./assets/fix_hands_ony_inpaint_prompt.png) |

| 4. changed prompt, inpaint prompt & modified content method | 5. changed prompt, inpaint prompt, modified content method and respective field | 6. changed prompt, inpaint prompt, modified content method and respective field then details method |
| ----------------------------------------------------------- | ------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
| ![inpaint](./assets/fix_hands_both_prompts.png)             | ![inpaint](./assets/fix_hands_respective_field.png)                             | ![inpaint](./assets/fix_hands_final.png)                                                            |


Lets try to fix the image:
1. The first image is the original image.
2. In the second image, we will use the inpaint method seted to `Improve Detail (face, hand, eyes, etc.)` and the inpaint prompt seted to `detailed hand`, with no change in the original prompt.
3. In the third image, we will use the inpaint method seted to `Modify Content (add objects, change background, etc.)` and the inpaint prompt seted to `detailed hand`, with no change in the original prompt.
4. In the fourth image, we will change both prompts to `detailed hand` and the inpaint method seted to `Modify Content (add objects, change background, etc.)`.
5. In the fifth image, we will change input prompt to `detailed female hand, five fingers`, and the original prompt to `beautiful brazilian woman, long hair, eyeglasses, casual clothing, sitting at desk, cheerful expression, smiling, waving, laptop, home office, indoor, nightlight, spot light, focus medium shot, detailed female hand, five fingers` the inpaint method seted to `Modify Content (add objects, change background, etc.)` and the inpaint respective field seted to `0.8`. **The inpaint respective field, is on the advaced settings, enabled by the `Advanced` checkbox, then in the advanced settings check the `Developer Debug Mode` checkbox, and then you will see the `Inpaint Respective Field` option.**
6. The sixth image is the final image, we getted the fifth image and used the inpaint method seted to `Improve Detail (face, hand, eyes, etc.)`.

**NOTE: Inpainting respective field is a way to inpaint the image with more context of the whole image. Higher the number, more context of the whole image.**

## Describe
This will get the prompt from the image. You can get the prompt from the image by uploading the image and clicking on the button.

## Enhance
Same as the enhance settings, you can enhance the image.
In here, you can drop the image and enhance it.
To do that, drop the image in the `Drop image here` box and also check the `Enhance` checkbox. Then enable at least on of the `#` tabs.

![Enhance image](./assets/image_enhancement.png)

We now add the following prompt to the image `Enhancement positive prompt` : `perfect blue eyes`.
Now we will compare the original image with the enhanced image and with another enhanced image with the inpaint method seted to `Improve Detail (face, hand, eyes, etc.)`

![Enhance image](./assets/enhance_inpaint_method.png)

let's see an example of an image enhancement.

in this sample we will use the `Enhance` checkbox and the `#1` tab. and enhance and change the eyes of the boxer in the image.

| original image                             | enhanced image                             | enhanced image with the impaint method            |
| ------------------------------------------ | ------------------------------------------ | ------------------------------------------------- |
| ![original](./assets/enhance_original.png) | ![enhanced](./assets/enhance_enhanced.png) | ![enhanced inpaint](./assets/enhance_inpaint.png) |


## Metadata
Get the metadata from the image. You can get the metadata from the image by uploading the image and clicking on the button.
Metadata is the data that describes the image, for example, the size of the image, the format of the image, the date that the image was created, the model used to generate this image, etc.

[BACK to Fooocus Ui](./Fooocus_ui.md)\
[BACK TO BEGIN](./README.MD)