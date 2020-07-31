# OBS-Encoder-Tunings
Some custom encoder tunings for Open Broadcast Software, for pretty and butter-smooth videorecording and streaming:


```
Why use I NVENC (NVIDIA Turing and better) GPU ASIC encoding instead of CPU encoding?
https://youtu.be/6fyP7kg0QAc?t=434

GPU encoding = Fast but dumb
CPU encoding = Smart but slow:
https://venturebeat.com/2018/10/15/nvenc-vs-x264-does-cpu-or-rtx-gpu-encoding-work-best-for-twitch/

Open Broadcaster Studio settings:

Plugins:
github.com/univrsal/input-overlay

Recording
3440x1440 60fps
Encoder:NvidiaASIC
CQ level: 18 (Lower is better!)
Preset: High Quality (Max Quality recommended, If you Dare!)

Streaming
Canvas Res: 3440x1440 30fps
Downscale to: 1720x720 30fps (2x) (When playing multiplayer)
Downscale Filter: Lanczos (Sharpened scaling, 36 samples)
Stream Delay: 7s (When Multiplayer)
Encoder:NvidiaASIC
CQ level:~27 normal games to 30 fast-paced multiplayer (Lower is better!)
Keyframe interval: 2sec (or auto, or whatever I feel like)
Max B-frames: 1 (higher 2-4 for slow pace games)
Preset: High Quality (Max Quality recommended, if you dare!)
Output → Enforce streaming service encoder settings → False
 ```
