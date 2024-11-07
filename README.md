# BrightBounceVRAD-OrangeBox
Light bouncing from Goldsource ported to Source (to avoid an impression of Doom2 per-sector lighting)

Produces brighter indirect lighting (bounced lighting) than stock OrangeBox VRAD

How to enable the algo:  
-hl1bounce -skipchildren (can be used separately)

How to make the effect stronger:  
-uniform

How to make the effect weaker:  
-MonteCarlo

Hardcoded cloud lighting for skyboxes, that are used on maps before Ravenholm:  
-clouds

Autobalance algo to figure out the optimal number of bounces.
(prevents the bouncing light from a chain reaction)
Active by default unless a bounce number was specified. Typically gives you 3-4 bounces. Stops if next bounce was weakened by less than 10%.

Since HL2 was made with so much fake lighting, here's system to clean it up:  
-SkipFakeLights

For debug purposes you can disable different lighting types or all at once:  
-SkipPointlights  
-SkipSpotlights  
-SkipSun

Misc:  
-ForceTexlights  
-ForceAttn  
-DebugClouds  
-SimpleChildren

Default game (HL2: Update):
![e7e8a8452e8e8d6d8c939730673c25ff](https://github.com/user-attachments/assets/70a17d48-a8ed-4424-985c-14025398402b)

-hl1bounce
![7fe6926858812574160a6d8e79365c7b](https://github.com/user-attachments/assets/184fdba3-6d4f-4527-aa9b-31c6ba50562f)

-hl1bounce -skipchildren
![6064d1b5a63581476ba5543675bb525f](https://github.com/user-attachments/assets/fc2a3b94-54de-4ee6-8d97-641d0bd6e9de)

-hl1bounce -skipchildren -uniform
![fac51803c3a0ce9577a9ace96b1c0383](https://github.com/user-attachments/assets/25c5c0a4-de9e-4f5f-9baa-cf63a7004f00)


