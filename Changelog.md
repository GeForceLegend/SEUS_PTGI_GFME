## HRR 2.1 v1.14

* Added 1.20.3 support;
* Added ko_kr language file by @DominoKorean (you can add your own by creating pull requests, but plz read the requirements in readme.md);
* Improved GI filter to match HRR3 behavoir;
* Fixed fence gates on some blockstates;
* Fixed volumetric light offset in low Minecraft versions;
* Fixed black screen when sun angle is set to ±90;

## HRR 2.1 v1.13.1

* Fixed compiling error with pixel look set to 1;
* Fixed compatibility with normal/specular switch on shader list menu;
* Fixed off-hand light in nether and the end;

## HRR 2.1 v1.13

* Added 1.20 support (`suspicious_gravel` and `calibrated_sculk_sensor`);
* Merged some missing changes from HRR3;
* Reduced default parallax depth;
* Fixed some entities like shulker box will write to voxel map at noon or midnight;
* Fixed sky brightness is 2x as expected;

## HRR 2.1 v1.12.1

* Fixed invisible experience orb;
* Fixed depth factor in reflection filter;
* Fixed reflection outside of voxelization radius;
* Fixed hand held light value with only off hand helds light;

## HRR 2.1 v1.12

* Added support for 1.19.4 new blocks
* Added support for bamboo buttons. They are forgotten in my 1.19.3 support.
* Added new setting SHAPE_CALC_FUNC, this can make you choose higher framerate or faster compiling while changing shader options.
* Fixed sky light leaking fix does not affect cloud light in irradiance cache ([#10](https://github.com/GeForceLegend/SEUS_PTGI_GFME/issues/10))
* Fixed sky rendering after joining a new world or turn back from the end.

## HRR 2.1 v1.11.1

* Fixed compiling error with screen space gi on;
* Fixed ray traced contact shadow issue with parallax;
* Fixed multiple stained glass blocks in one ray;
* Fixed furnace light does not get stained.

## HRR 2.1 v1.11

* Lite optimization on GI program, 5% - 10% FPS boost;
* Fixed compiling error on 1.16.5;
* Fixed lots of non-full blocks do not get voxelized;
* Fixed 1.19.3 support

### Preview2

* Fixed something unknown (but related to fishing rod line) calculated in voxelization;
* Fixed Iris incompatibility issue 2 (see Readme.md for more info) in 1.17 and above.

### Preview1

* Pre-support for 1.19.3 new blocks;
* Added amethyst buds as light sources;
* Fixed crack in caustics;
* Fixed powder snow and mangrove roots

## HRR 2.1 v1.10

* Latest version when setting up this repo
