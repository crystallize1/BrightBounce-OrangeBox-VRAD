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

Default game:
![e7e8a8452e8e8d6d8c939730673c25ff](https://github.com/user-attachments/assets/70a17d48-a8ed-4424-985c-14025398402b)

Start to enable parameters:
![7fe6926858812574160a6d8e79365c7b](https://github.com/user-attachments/assets/184fdba3-6d4f-4527-aa9b-31c6ba50562f)
![6064d1b5a63581476ba5543675bb525f](https://github.com/user-attachments/assets/fc2a3b94-54de-4ee6-8d97-641d0bd6e9de)
![fac51803c3a0ce9577a9ace96b1c0383](https://github.com/user-attachments/assets/25c5c0a4-de9e-4f5f-9baa-cf63a7004f00)



