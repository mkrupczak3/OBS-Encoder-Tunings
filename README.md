# OBS-Encoder-Tunings
Some custom encoder tunings for Open Broadcast Software, for pretty and butter-smooth videorecording and streaming:


```
Open Broadcaster Studio settings:

Plugins:
github.com/univrsal/input-overlay

Recording
3440x1440 60fps
Encoder:NvidiaASIC
CQ level: 18 (Lower is better!)
Preset: High Quality

Streaming
Canvas Res: 3440x1440 30fps
Downscale to: 1720x720 30fps (2x) (When playing multiplayer)
Downscale Filter: Lanczos (Sharpened scaling, 36 samples)
Stream Delay: 7s (When Multiplayer)
Encoder:NvidiaASIC
CQ level:~27 normal games to 30 fast-paced multiplayer (Lower is better!)
Keyframe interval: 2sec (or auto, or whatever I feel like)
Max B-frames: 1 (higher 2-4 for slow pace games)
Preset: High Quality
Output → Enforce streaming service encoder settings → False
 ```
