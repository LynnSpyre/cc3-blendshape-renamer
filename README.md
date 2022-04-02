# cc3-blendshape-renamer

Just a quick script to rename the arkit blendshapes on your cc3 model, in a blender project.
This is not good code, but again, it does the job.

## Why make this?

Because Cc3 models have their own naming convention for blendshapes that breaks literally any piece of software trying to use arkit, that isn't specifically designed to handle CC3 stuff. This script corrects the problem, bringing your model into line with the same naming conventions the rest of the world is using. This should save you from having to do fuzzy lookups or add interpolation layers to your unity app. Just do it, get it done.

This should work for you if you have a blender to unity pipeline, or a blender to unreal engine pipeline. I haven't tested it in any other scenarios, and ymmv. It should also work if you're moving a model between cc3 and CATS.

## Instructions

**Step 1** Export your model with the "Mouth Open as Morph" option enabled.
For your own sanity, you're probably going to want to do all of the t-pose things too. The whole t-pose dance that character creator makes you do.

**Step 2** Using the cc3_blender_bake plugin, import your model with animations enabled, physics, and lighting.

**Step 3** Cross open a second window, and select text editor. Click on "new," and create an empty text file.

**Step 4** Paste my happy little code snippet into your text editor. It will run through all of the layers of everything in your scene, so it's super important that you have only your cc3 model in the scene for now. 

**Step 5** Open the blender console to see the script output.

**Step 6** Hit the play button on the text editor. This will execute your code.

**Step 7** Yuh done
