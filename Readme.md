
# SEUS PTGI GeForceLegend's Modified Edition

A deeply modified version of SEUS PTGI

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

## Compatible with latest beta (1.5.0 Beta2) of [Iris](https://github.com/IrisShaders/Iris)

### Currently there are 2 issues stopping GFME from loading on previous Iris, and issue 1 only affect GFME 1.10 and above:

1. (Get fixed by iris side on iris 1.5.0 beta2)~~Unable to parsing settings (MC_VERSION, etc) in block.properties, causing parsing issues with block.properties. See [Iris#1712](https://github.com/IrisShaders/Iris/issues/1712) for more info.~~
2. (Get fixed for 1.17+ in v1.11 Pre2. Sorry for 1.16.5 iris players) ~~Attribute indexes are not same as Optifine. For cleaner game output logs, GFME uses below code to get some vertex attributes, but since location index in Iris is different from Optifine, GFME can't get correct vertex attributes while running on Iris.~~
```glsl
#if MC_VERSION >= 11500
layout(location = 11) in vec4 mc_Entity;
layout(location = 12) in vec4 mc_midTexCoord;
layout(location = 13) in vec4 at_tangent;
#else
layout(location = 10) in vec4 mc_Entity;
layout(location = 11) in vec4 mc_midTexCoord;
layout(location = 12) in vec4 at_tangent;
#endif
```
1. (Get fixed in v1.11 Pre1) ~~Custom uniform in Iris works different from Optifine. In Optifine, all custom uniforms are calculated in floating point, so something like integer / integer will returns a correct floating point value but not an integer value. But in iris, integer / integer will returns a floored integer value, this caused the TAA offset could not working in Iris. I have to say this is my fault, and should be fixed in future versions (if there are future versions).~~
