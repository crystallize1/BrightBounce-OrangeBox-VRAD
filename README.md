# BrightBounceVRAD-OrangeBox
Light bouncing from Goldsource ported to Source (to avoid an impression of Doom2 per-sector lighting)

Produce brighter indirect lighting (bounced lighting) than stock OrangeBox VRAD

How to enable the algo:
-hl1bounce -skipchildren (can be used separately)

How to make the effect stronger:  
-uniform

How to make the effect weaker:
-MonteCarlo

Hardcoded cloud lighting patterns for skyboxes used on maps before Ravenholm:
-clouds

Quick dirty autobalance algo that can figure out the optimal number of bounces for you! (prevents the bouncing light from stabilization and then a chain reaction) Active by default as long as you do not specify bounce number. Typically gives you 3-4 bounces. Stops bouncing when the new bounce is less than 10% weaker.

Since HL2 was originally made with so much fake lighting, here's a legacy system to clean it up:
-SkipFakeLights

Also you can disable different lighting types or all at once:
-SkipPointlights
-SkipSpotlights
-SkipSun

Misc:
-ForceTexlights
-ForceAttn
-DebugClouds
-SimpleChildren
