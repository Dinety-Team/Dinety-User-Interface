## Dinety User Interface

Technical Notes & Implementation Plan for Dinety UI  

> [简体中文](./README_zh.md)  

---

Visit the `Code` page to browse the source.  

---

This document explains the core ideas, implementation roadmap and design language of the Dinety User Interface (hereinafter referred to as “UI”).

The feature set shown here reflects the current research status; it is not the final release. Always refer to the official shipped version for production behavior.

---

## 3D-UI Implementation

We use dynamically flipping 3-D models as the game’s UI elements.

All models are created in Blender and imported into Unity, where the UI itself is built with Unity’s 3-D mode.

## Touch Feedback (Visual)

Hit-effects for notes resemble water ripples. The ripple integrates with the background scenery through smooth, interpolated animations that give players a silky visual feel while preserving overall picture harmony.

The same technique is applied to tools such as the Dinety chart editor, ensuring consistent real-world touch feedback.

Players can adjust the maximum ripple size in Settings.

## UI Animation Engine

To deliver a premium visual experience we continuously refine UI layout, interaction and motion. Our goals are:

- System-level animation smoothness  
- Compliance with our [UI Color-Grading Standard](./ColorGradingStandard.md) to guarantee beautiful and correct color reproduction

## UI “Tailoring”

On first launch we measure the device’s screen-corner radius. UI corners are then matched to the hardware’s physical curvature, producing icons that feel naturally at home on that specific device.

---

## License

This project is released under the MIT License.

Please observe all license terms when using any content contained herein.

[MIT License text](./LICENSE.md)

[Original MIT License](https://mit-license.org/)