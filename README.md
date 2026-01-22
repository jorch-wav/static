# Static - Interactive Distance-Reactive Video Installation

An interactive web-based art installation that reveals a music video through a static curtain, simulating proximity-based interaction using keyboard and scroll controls.

## 🎨 Concept

Static creates an immersive experience where viewers "unveil" hidden video content by simulating movement closer to or further from the installation. As distance decreases, a music video gradually emerges from behind a static noise curtain, accompanied by smooth audio crossfading.

Originally designed as a Raspberry Pi installation using a VL53L1X distance sensor, this web version uses keyboard controls to simulate the physical interaction.

## 🎮 Controls

- **↑ Arrow / Scroll Up** - Move Closer (Reveal Music Video)
- **↓ Arrow / Scroll Down** - Move Away (Show Static)
- **I** - Toggle Distance Indicator
- **M** - Mute/Unmute
- **ESC** - Exit Fullscreen
- **ENTER** - Start Experience

## 🚀 Live Demo

**GitHub Pages:** [https://jorch-wav.github.io/static/](https://jorch-wav.github.io/static/)

## 🛠️ Technical Implementation

- **Dual Video Layers:** Two HTML5 video elements layered with z-index
- **Alpha Blending:** Dynamic opacity control on static curtain based on simulated distance
- **Web Audio API:** Separate AudioContext for each video with GainNode crossfade
- **Distance Simulation:** Range from 100mm (NEAR) to 3000mm (FAR)
- **Smooth Transitions:** requestAnimationFrame update loop with blend speed control
- **Vertical Distance Bar:** Visual feedback showing proximity level

## 📁 Project Structure

```
static-web/
├── index.html          # Main application
├── video1.mp4          # Static curtain overlay (5.3MB)
├── video2.mp4          # Music video content (33MB)
├── VIDEO_SETUP.md      # Video file setup instructions
└── README.md           # This file
```

## 🎥 Video Credits

Videos sourced from the original Raspberry Pi Static installation project.

## 🔗 Related Projects

- [Blue Square](https://github.com/jorch-wav/blue-square) - Interactive particle system
- Original Static v2.0 (Raspberry Pi + VL53L1X sensor)

## 📄 License

Created by Jorge

---

*Experience the installation at [jorch-wav.github.io/static](https://jorch-wav.github.io/static/)*
