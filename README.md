Python script using Stable diffusion to inpaint images which has object and white background.

Approach used:
1) Given an image with an object and white background, -> generate a mask for that object. This is to ensure that our stable diffusion model doesn't change the object.
2) Added extra padding surrounding the image to have more space to contain more inpainting in background.
3) Passed the image and mask to pipeline with suitable text prompt to obtain the results.
