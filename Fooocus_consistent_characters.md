# Character consistency

- use same seed for same character
- use name on prompt, like `cameron mila swift` this is a well known characters, Cameron Diaz, Mila Kunis, Taylor Swift, they are all beautiful, so the model will try to generate a beautiful character, this is only a example name this will be referenced as `{YOUR_CHAR_NAME}`, from now on. 
- Create a `headshot` of the character, with the name of the character
- If we want to change the mood of the character, we can use the prompt we can include it in the prompt, like "`{YOUR_CHAR_NAME}` angry" or "`{YOUR_CHAR_NAME}` big smile" or use `enhance` checkbox and use variation like `vary (Subtle)` or `vary (Strong)` to change the mood of the character.
- Create  3 pictures with the same seed, but with different prompts, like `{YOUR_CHAR_NAME}`, `{YOUR_CHAR_NAME} angry`, `{YOUR_CHAR_NAME} big smile`
- Use the `input image` checkbox to use a image of the character, then take each of the 3 pictures and use the `input image` checkbox. Select advanced and `FaceSwap` for all 3 pictures. This will make the result very consistent with the character.

## Creating character

Positive Prompt: `beautiful woman, soft skin, freckles, arkan blue eyes, cameron mila swift, studio portrait, blond hair`\
Negative Prompt: `bad eyes, cgi, airbrushed, plastic, deformed, watermark`\
seed: `644515184151156`

Then we got the some an chose one.
Then we used the same seed and prompt, only adding `, angry` to the prompt, and got the second image.
Then we used the same seed and prompt, only adding `, big smile` to the prompt, and got the third image.
Try to take pictures with the little diferent tilts.
you can use `input image` checkbox, in tab `upscale and variation`, select the image generated before and chose `Vary (strong)` (not used for the images below).


| Original                                         | Angry                                        | Big Smile                                            |
| ------------------------------------------------ | -------------------------------------------- | ---------------------------------------------------- |
| ![Original](./assets/consistent_char_normal.png) | ![Angry](./assets/consistent_char_angry.png) | ![Big Smile](./assets/consistent_char_big_smile.png) |

With this 3 images we can create a consistent character, with different moods.

### usage sample

Positive Prompt: `beautiful woman, on the beach, in a red dress, soft skin, freckles, arkan blue eyes, cameron mila swift, blond hair`
Negative Prompt: `bad eyes, cgi, airbrushed, plastic, deformed, watermark`
seed: `644515184151156`

Using the`input image` checkbox, in tab `image prompt` select the 3 images generated before and chose `FaceSwap` for all 3 images, with the default settings.
Here is the result:\
![Consistent Character](./assets/consistent_char_result1.png)


### Using Inpating and FaceSwap at same time

I have a image that I liked and I want to use it as a base for the character, but I want to change the character face to be more consistent with the character I created before.\

First I will use the `input image` checkbox, in tab `Inpaint or Outpaint` select the image I want to use as base, and chose `Inpaint` for the image, with the default settings.

![mix inpait](./assets/consistent_char_mix_ipaint_faceswap1.png)

Then I will use the `input image` checkbox, in tab `image prompt` select the 1 or more images generated before and chose `FaceSwap`.

![mix faceSwap](./assets/consistent_char_mix_ipaint_faceswap2.png)

then check the `advanced` checkbox and select the `developer debug mode` checkbox,  and the select the `control` tab. check `Mixing Image Prompt and Inpaint` checkbox.

![mix checkbox](./assets/consistent_char_mix_ipaint_faceswap3.png)

Then click on `Generate` and the model will use the image inpainted and the face swapped image to
then generate the image.\

![mix result](./assets/consistent_char_mix_ipaint_result.png)

**upscaling images in my pc is buggy, Vram 8GB, RTX 4060, notebook.**

### FaceSwap with different angles (more precise)

Now lets generate some grid images as pose to our character.

Positive Prompt  `grid of a human head, androgynous, left side view, bald`\
Negative Prompt: `hair, grid lines, color, clothes, accessories`\
In the `advanced` checkbox, select `Style` tab, unselect all and select only `SAI Line art`, set the seed to `random` at `settings` tab, and click on `Generate`.
Generate for both sides, left and right at lest.

#### First approach
With this approach we will generate a single grid image of 4 images, with the same character face, but with different tilts.

![grid](./assets/char_grid1.png)

now in photopea or another image editor, create a single image with 4 images, 1 with front grid, 1 with left grid, 1 with right grid, and 1 with back grid(if you can).

Something like this:
![grid](./assets/facegrid2.png)

Then use the `input image` checkbox, in tab `image prompt` select the image generated before and chose `PyraCanny` for all 4 images, with the default settings.
and lets use a similar prompt to the one we used before, but with the grid images (`just added a grid of 4 images`).

Positive Prompt: `a grid of 4 images, beautiful woman, soft skin, freckles, arkan blue eyes, cameron mila swift, studio portrait, blond hair`\
Negative Prompt: `bad eyes, cgi, airbrushed, plastic, deformed, watermark`\
seed: `644515184151156`

![grid](./assets/char_grid2.png)

then this is one of the results:
![grid](./assets/char_grid_result1.png) 

split the image in 4 and you will have a grid of 4 images with the same character, but with different poses.
| Right                                  | Left angled                                  | Front                                  | left                                  |
| -------------------------------------- | -------------------------------------------- | -------------------------------------- | ------------------------------------- |
| ![Right](./assets/from_grid_right.png) | ![Left angled](./assets/from_grid_left1.png) | ![Front](./assets/from_grid_front.png) | ![Left](./assets/from_grid_left2.png) |

Finally, you can use the the splited images to create a new image of the caracter with a different pose, using the `input image` checkbox, in tab `image prompt` select the 3 images (front, left and right) generated before and chose `FaceSwap` for all 3 images.

![swap faces with 3](./assets/consistency_final_step.png)

here is the final prompt:

Positive Prompt: `beautiful woman, soft skin, freckles, arkan blue eyes, cameron mila swift,  loose blond hair, hyperdetailed photography, soft light, in the club wit a red dress`\
Negative Prompt: `bad eyes, cgi, airbrushed, plastic, deformed, watermark`\
seed: `644515184151156`

and here is the final result:
|                                                       |                                                             |
| ----------------------------------------------------- | ----------------------------------------------------------- |
| ![Right](./assets/consistency_final_step_result1.png) | ![Left angled](./assets/consistency_final_step_result2.png) |

### Second approach
With this approach we will generate a each face with a different tilt with `FaceSwap` of our first generated character image:

![first image](./assets/consistent_char_normal.png)

then create more 2 images with the same seed, same prompt but adding the grid image in the `input image` checkbox, in tab `image prompt` select the the grid image generated before and chose `PyraCanny` and then `FaceSwap` for the fist image.

![second approach](./assets/second_approach_facegen1.png)

in the end you will have 3 images with the same character, but with different tilts.
| Left                                       | Right                                        | Original                                            |
| ------------------------------------------ | -------------------------------------------- | --------------------------------------------------- |
| ![Left](./assets/second_approach_left.png) | ![Right](./assets/second_approach_right.png) | ![first image](./assets/consistent_char_normal.png) |


then use the `input image` checkbox, in tab `image prompt` select the 3 images generated before and chose `FaceSwap` for all 3 images.

then this is one of the results:

Positive Prompt: `beautiful woman, soft skin, freckles, arkan blue eyes, cameron mila swift, loose blond hair, hyperdetailed photography, soft light, in the club, wearing a red dress`\
Negative Prompt: `bad eyes, cgi, airbrushed, plastic, deformed, watermark`\
seed: `644515184151156`

|                                                   |                                                   |
| ------------------------------------------------- | ------------------------------------------------- |
| ![Result 1](./assets/second_approach_result1.png) | ![Result 2](./assets/second_approach_result2.png) |
