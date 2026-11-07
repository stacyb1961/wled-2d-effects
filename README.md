# WLED Matrix Effects for ESP32 RGB Panels

This repository contains a collection of custom WLED effects designed specifically for LED matrix panels, with a current focus on the **Waveshare ESP32-RGB-LED-Matrix (ESP32-S3) boards**.

These effects are meant to be:

- Visually optimized for 2D matrices rather than LED strips  
- Performance‑friendly on ESP32‑class hardware  
- Easy to customize and remix for your own installations

---

## Hardware Target

The primary target hardware is:

- Waveshare ESP32 RGB LED Matrix board (ESP32‑S3)
- HUB75‑style LED matrix panels compatible with that controller

Other ESP32‑based matrix setups may work as well, but have not been tested.

---

## Effects Included

This repo focuses on **matrix‑oriented effects** for WLED, such as:

- 2D animations (e.g. waves, noise, flows, and patterns)
- Effects that take advantage of the full panel resolution
- Variants tuned for the timing and memory limits of ESP32‑S3

The exact list of effects and technical details may evolve over time; see the code and comments in each file for effect‑specific documentation.

---

## Using These Effects

There are two common ways to use these effects with WLED:

1. **As a code contribution / custom build**  
   - Integrate the effect source files into a local WLED checkout  
   - Rebuild WLED for your ESP32‑S3 board  
   - Flash the custom firmware to your Waveshare matrix controller

2. **As presets / configuration (if applicable)**  
   - Some content may be preset or configuration files rather than code  
   - Import them into WLED via the web UI or filesystem as described in WLED’s documentation  

Please refer to the official WLED documentation and the Waveshare board docs for details on building and flashing firmware.

---

## Compatibility and Notes

- These effects are developed and tested against recent WLED versions; older versions may not support all features used here.
- Certain effects may assume a specific panel size, orientation, or mapping. Check the comments in each effect file for any assumptions (panel width/height, rotation, segment mapping, etc.).
- The Waveshare ESP32 RGB S3 board has its own pin mappings and power considerations; make sure your hardware wiring and configuration match the board’s documentation.

---

## Contributing

Contributions are welcome. Examples of useful contributions:

- New matrix‑friendly effects
- Performance improvements for ESP32‑S3
- Adaptations for different matrix sizes or layouts
- Bug fixes and documentation improvements

If you open a pull request, please briefly describe:

- Your hardware setup (board + panel type + resolution)
- WLED version you tested with
- Any configuration assumptions your effect requires

---

## License

This project is licensed under the **MIT License**.

You are free to use, modify, and distribute these effects in your own projects, including commercial ones, as long as you retain the copyright and license notice.

See the `LICENSE` file for full details.
