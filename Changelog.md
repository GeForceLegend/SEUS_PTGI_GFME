## HRR 2.1 v1.19
### Added
- Added support up to 1.21.9;
- Added `ja_jp.lang` from @src3453
- Added `hu_hu.lang` from @Karpatok9089
### Updated
- Updated `ru_ru.lang` from @NizeroXs;
- Updated the look of glowing berries and glowing lichen to match HRR3;
### Fixed
- Fixed overexposure caused by contrast code (#70);
- Fixed compiling error when trying to enable WET_CAVE_EFFECT with Distant Horizons (#76);
- Fixed cloud shadow changes position with camera Y coordinate;
- Fixed parallax with different texture resolution and atlas size;
- Fixed rain ripple not visible under water (#92)

## HRR 2.1 v1.18

* Added support up to 1.21.5;
* Added auto shape detection for mods based on Iris tag support;
* Added contrast slider;
* Added average exposure switch;
* ru_ru.lang from @NizeroXs;
* uk_ua.lang from @yehor-bachurin;
* Held light changed from switch to slider;
* Fixed SUNLIGHT_BRIGHTNESS do not work on leaves

## HRR 2.1 v1.17

* Added support up to 1.21.4;
* en_us.lang update from @LimeDragonBoi ;
* Fixed path traced shadow will ignore the block in the same voxel of start position;
* Fixed path traced shadow using wrong param;
* Fixed caustics on certain height;
* Fixed depth of DH terrain when projection matrix changes (related to IrisShaders/Iris#2534);

## HRR 2.1 v1.16

* Added 1.21 support;
* Added Distant Horizons support;
* Improved distant screen space shadow on leaves;

## HRR 2.1 v1.15

* Added 1.20.5 support;
* Added Physics ocean support;
* Added zh_tw language file by @new1271 ;
* Ignored black background of texts;
* Fixed snow in Physics mod;
* Fixed specular texture when parallax is enabled;
* Fixed materialID precision on some AMD device;
* Fixed SUNLIGHT_BRIGHTNESS setting;

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
