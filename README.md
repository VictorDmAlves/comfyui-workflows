<div align="center">

# ComfyUI Workflows
**My personal Workflows.**

![ComfyUI Screenshot](./Images/Main.png)
</div>

This is simply a repository I decided to create to keep a copy of my ComfyUI Workflows, which I've been using for over two years. Furthermore, since I've learned so much from the community on Discord and Reddit, I'm happy to share it with everyone.

Feel free to use them and make your own customizations. Note that I am using GGUF models on my computer; change its nodes if you are using native models.

If you find something that could be improved and you'd like to share it with me, let me know here or through my Reddit by the username VictorDmAlves.

If you like to keep track of any changes that I make to the Workflows, be sure to Watch this repository on GitHub.

## Dependencies
I highly recommend using Straight lines in the "Lite Graph" settings, under the "Graph" section. Either this, or keep the lines invisible. My Workflows were built with this in mind.

To use this Workflows, install the following Custom_Nodes in your ComfyUI (you probably already have most of them):
- [ComfyUI Manager](https://github.com/Comfy-Org/ComfyUI-Manager).
- [Comfy-KepListStuff](https://github.com/M1kep/Comfy_KepListStuff).
- [ComfyUI's ControlNet Auxiliary Preprocessors](https://github.com/Fannovel16/comfyui_controlnet_aux).
- [ComfyUI Essentials](https://github.com/cubiq/ComfyUI_essentials).
- [ComfyUI-Detail-Daemon](https://github.com/Jonseed/ComfyUI-Detail-Daemon).
- [Florence2 in ComfyUI](https://github.com/kijai/ComfyUI-Florence2).
- [ComfyUI-GGUF](https://github.com/city96/ComfyUI-GGUF).
- [ComfyUI-Impact-Pack](https://github.com/ltdrdata/ComfyUI-Impact-Pack).
- [ComfyUI-Impact-Subpack](https://github.com/ltdrdata/ComfyUI-Impact-Subpack).
- [ComfyUI-Inspire-Pack](https://github.com/ltdrdata/ComfyUI-Inspire-Pack).
- [KJNodes for ComfyUI](https://github.com/kijai/ComfyUI-KJNodes).
- [QwenVL for ComfyUI](https://github.com/1038lab/ComfyUI-QwenVL).
- [ComfyUI-SeedVR2_VideoUpscaler](https://github.com/numz/ComfyUI-SeedVR2_VideoUpscaler).
- [ComfyUI Simple Prompt Batcher](https://github.com/ai-joe-git/ComfyUI-Simple-Prompt-Batcher).
- [ComfyUI-VideoHelperSuite](https://github.com/Kosinkadink/ComfyUI-VideoHelperSuite).
- [rgthree-comfy](https://github.com/rgthree/rgthree-comfy).
- [WAS Node Suite (Revised)](https://github.com/ltdrdata/was-node-suite-comfyui).
- [Z-Image Power Nodes](https://github.com/martin-rizzo/ComfyUI-ZImagePowerNodes).

## The Workflows

#### [Z-Image-Turbo](https://github.com/Tongyi-MAI/Z-Image)
![Z-Image-Turbo Collage](./Images/Z-Image-Turbo.png)

One of my favorites so far. Realistic, versatile and fast. It's recommended to use the Z-Image for training, so I'm not going to build a Workflow for it; just using the Turbo one is enough and very competent.

I've created this Workflows so far:
- TXT2IMG: A simple text to image using a custom_node with styles presets.
- IMG2IMG: A image to image with ControlNet implementation, if you want to make a very similar image.
- SeedVR2 Upscaler: First it runs through a second KSampler to add more details. After that, by enabling the group "SeedVR2", you can upscale the image.

Folder to the Workflows [Z-Image-Turbo](./Workflows/Z-IMAGE/).
Folder with example [Images](./Images/Z-Image-Turbo/).

#### [Wan 2.2](https://github.com/Wan-Video/Wan2.2)
![Wan 2.2 Collage](./Images/Wan22.png)

<div align="center">
  <video src="https://github.com/user-attachments/assets/a0dbcc65-0d17-4919-87fd-a60485ef7bca" width="70%" poster=""> </video>
</div>

Honestly, this model is extremely impressive. I'm surprised by its flexibility and realism, considering it's primarily a video model. That, and the vast collection of LoRAs available for it, makes it a very competent model for both image and video.

I've created this Workflows so far:
- TXT2IMG: A simple text to image using WanVideoNAG for better control.
- IMG2IMG: A image to image, but with no ControlNet of any kind yet (Wan has VACE; a different beast itself, I'm still learning).
- TXT & IMG2VID: With the help of the 5B model, that can creat text or image to video, this Workflow allow you to generate a video with good length and quality. I've add the possibility to "stitch" two videos at one, making it seem like it's a continuous video; for that, see the Note within this Workflow for more information.
- SeedVR2 Upscaler: Same as the others. First it runs through a second KSampler to add more details. After that, by enabling the group "SeedVR2", you can upscale the image.

Folder to the Workflows [Wan 2.2](./Workflows/WAN/).
Folder with example [Images and Video](./Images/WAN/).