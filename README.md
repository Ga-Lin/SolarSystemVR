# SolarSystemVR
## Introduction
**SolarSystemVR** is an immersive virtual reality designed to educate and inspire users about our solar system. Built in Unreal Engine 5, this project leverages VR technology to allow users to explore planetary bodies at scale, interact with celestial objects, and gain a more intuitive experience of orbital mechanics through hands-on engagement.

## Preparation
**Platform**: Windows 10

**Device**: Oculus Rift and Touch

**Unreal Engine 5 Version**: 5.3.2

## Launch
Download:
- [Shipping version (733 MB)](https://drive.google.com/file/d/1ZeQWi-yfmhLCEk339D9Bs76Ww4sgPhbl/view?usp=sharing)
- [Development version (895.7 MB)](https://drive.google.com/file/d/1If8LlYYMKo0jQsuGOz1upyFQODjRBsgW/view?usp=sharing)

Run `SolarSystemVR.exe` in `/Build/Windows` - [Preview Video](https://drive.google.com/file/d/1sMiLaH8oU-Sym637rhuAwBGO1FLoa_d3/view?usp=sharing)

## Key Features
### Character Movement
- Unlike traditional VR teleportation, movement is controlled via the left thumbstick for smooth, continuous motion:
  - Forward/Backward: Thumbstick tilt up/down translates to movement along the actor’s forward vector.
  - Strafe: Thumbstick tilt left/right moves the player laterally.

- Sharp turns: A full right thumbstick press triggers an instant 90-degree snap turn (reducing motion sickness while maintaining immersion).

### Accurate Orbital Mechanics
- Real-scale solar system: Planets are scaled down proportionally to balance performance and visibility.
- Rotation and revolution:
  - Self-rotation: Updated per-frame with axis-aligned angular velocity.
  - Orbital revolution: Planets revolve around the sun in world space, with speeds derived from real orbital periods.

### Interactive Planet Manipulation
- Visual feedback:
  - Highlight: On overlap with VR controller, planets display a dynamic material overlay.
  - Label: A text render component anchored to the planet renders its name in glowing text.
- Grab mechanics: Holding either controller’s grip button (Grab action) attaches the planet to the hand.

### Orbital Sound Attenuation
A distance-based (between player and planet) volume falloff of the looping ambient track (e.g., low-frequency hum for gas giants) is spatialized for directional realism.

## Resource Reference
### [HDRI](https://ambientcg.com/view?id=NightSkyHDRI001 "Night Sky HDRI 001")
HDRI (High Dynamic Range Imaging) is a technique that captures and displays a wider range of luminance levels than standard imaging, allowing for greater detail in both shadows and highlights. It combines multiple exposures of the same scene into a single image, preserving a broader spectrum of light and color.

### Models
All 3D assets are free and downloadable on the [Sketchfab](https://sketchfab.com/) website:
- [Sun](https://sketchfab.com/3d-models/the-star-sun-519dddb6998545e2bf84225394dc71fe)
- [Mercury](https://sketchfab.com/3d-models/mercury-32347fa4ec1a4987b71f461a401d91c4)
- [Venus](https://sketchfab.com/3d-models/venus-b306aaadbf2b4fcea1afa2db5ed75b4f)
- [Earth](https://sketchfab.com/3d-models/earth-4de1bcbd22a444abb4f089b9b78ec96a)
- [Mars](https://sketchfab.com/3d-models/mars-9c7bbc64d8c74acfa9ec344c0fc10e1a)
- [Jupiter](https://sketchfab.com/3d-models/jupiter-d252c96ae3de48d7968b1206522ba9f5)
- [Saturn](https://sketchfab.com/3d-models/saturn-c09a1970148c43ad99db134a9d6d00b5)
- [Uranus](https://sketchfab.com/3d-models/uranus-0009a69dbace44608c0bd09af9ba20db)
- [Neptune](https://sketchfab.com/3d-models/neptune-fe05e06a265d4a8f9285d34c933878ee)

### Special Materials
[Hologram Effect](https://www.youtube.com/watch?v=LOKYUgfZI6Y): An advanced hologram material with a neat glitch effect.

### Audios
- **Background Music**: [Space Exploration - Starfield, Blue Wave Studio](https://music.apple.com/us/album/starfield/1629949902)
- [Orbital Sound](https://freesound.org/people/samsmyname/sounds/51363/): The orbital sound refers to the hypothetical or simulated audio effects that could be experienced in space near a planet, despite the vacuum of space normally preventing sound transmission.

### VR Expansion Plugin
The [VR Expansion Plugin (VRE)](https://vreue4.com/) is an Unreal Engine plugin designed to facilitate advanced Virtual Reality interactions and gameplay elements, especially motion controller interactions in this project.