
# SEUS PTGI GeForceLegend's Modified Edition

A deeply modified version of SEUS PTGI

## Language Files

If you want to add language file for your own language, create a pull request!

Please make sure the name of your language file is lower-case like `en_us.lang` but not `en_US.lang`, or low versions of Minecraft and Optifine won't read them.

## Install

### Due to PTGI's EULA, its illegal to distribute PTGI's code directly, so you need to follow these steps to extract SEUS PTGI GFME

1. Download the jar file from release page, and download a **vanilla unedited** GFME based PTGI version (currently HRR 2.1) file from [Cody's Patreon page](https://www.patreon.com/sonicether/posts) if you don't have one.

2. Put the jar file and PTGI HRR 2.1 file into the same path, and double click the jar file. If everything is fine, there will be a new folder (older version of GFME) or a zip file (newer GFME version) that can be used directly as a shaderpack by moving this file or folder into .minecraft/shaderpacks.

If there is nothing happened while double clicking jar, you can run this jar in CMD or Powershell by `java -jar "<your GFME jar path>"` for more information.

## Features

### Per-pixel rendering in path tracing, include cutout, transpanret and even PBR support

![Per_pixel_rendering.png](Images/Per_pixel_rendering.png)

### More colored vanilla lighting sources and block shapes

![More_vanilla_support.png](Images/More_vanilla_support.png)

### Auto texture resolution, better support for incomplete texture packs

![Auto_resolution.png](Images/Auto_resolution.png)

### Metal sunlight caustics

![Metal_caustics.png](Images/Metal_caustics.png)

### Many more small fixes and improvements for vanilla PTGI...

## Compatible with [Iris](https://github.com/IrisShaders/Iris) above 1.5.0, with some bugs:

### Iris version 1.5.0 to 1.6.1X:

- block.properties parsing does not work perfectly, as Iris just deletes comments in block.properties, which may cause some issue on `#else` macro. I'm not sure if this really caused any problem, but of course their way handiling macros in block.properties is not good enough.

### Iris version above 1.6.1X (Probably 1.6.12 or 1.6.13?):

- block.properties parsing is changed for unknown reason, causing macros in block.properties is parsed incorrectly, and tons of blocks in block.properties cannot get correct blockID, and lose their special shape in path tracing.
