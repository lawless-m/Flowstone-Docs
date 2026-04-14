# Camola

A [[rust]] real-time webcam pipeline — "Webcam FX" — that segments you from the background with a neural network and composites you onto replacement backgrounds or demoscene-style effects, then pipes the result into a v4l2loopback virtual camera that Teams, Zoom and friends see as an ordinary webcam.

**Repo:** `~/Git/Camola`
**Themes:** [[rust]]

Captures at 1080p, segments with RobustVideoMatting (primary) or MODNet (fallback) for alpha matting, composites, and outputs 720p @ 30fps to v4l2loopback. Runs on Linux with an NVIDIA RTX 3070/4070 via CUDA/TensorRT. Effect roster planned at last touch: background replacement, trails (ghosting / blur / chroma / glitch), plasma (demoscene colours), glitch (corruption / RGB split), cyberspace (Max Headroom style), and face mesh (wireframe overlay). Each effect has its own spec document — the pipeline itself is built in stages from a camera-to-loopback passthrough up through segmentation, background replacement and procedural effects.
