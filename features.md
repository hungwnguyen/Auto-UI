# Supported Features

> The **Auto UI Generator** provides a professional suite of tools to automate the tedious aspects of UI implementation while maintaining full developer control through deep customization.

## Advanced AI Detection & Customization

### 🚀 Custom Text & OCR Integration
The tool doesn't just "read" text; it integrates it into your project's specific design system using TextMeshPro (TMP).
* **Automated OCR:** Automatically extracts text strings from your mockup and assigns them to generated objects.
* **Prefab-Based Styling:** All generated text is based on your `Text.prefab`. By customizing this prefab, every detected text element inherits your project's unique font and styling.
* **Intelligent Scaling:** The system enables TMP Auto-Sizing by default to ensure text fits perfectly within the detected bounding box.

![Image: Unity Game View resolution settings demo](images\7.png)
### 🛠️ Custom Button Logic
Go beyond simple images by generating interactive components that carry your specific game logic.
* **Smart Identification:** The AI identifies button-like regions and instantiates them using your custom `Button.prefab`.
* **Functional Customization:** You can add custom scripts, transitions, or audio triggers to your Button prefab, which are then applied to all generated buttons in the scene.
* **Complete Unpacking:** Buttons are "completely unpacked" upon instantiation, allowing you to modify individual button properties immediately without breaking prefab links.

### 🧠 Custom Model Training (AI "Brain" Training)
For advanced users, you can refine the detection engine by training a custom MobileNetV2 model using the provided Python training script.
* **MobileNetV2 Architecture:** Leverage a state-of-the-art lightweight model optimized for fast performance.
* **Aspect-Ratio Preserving Preprocessing:** The training script uses `resize_with_pad` to maintain the integrity of your UI assets, preventing distortion during training.
* **Automated Data Augmentation:** Built-in layers for Random Zoom and Translation help the AI recognize buttons even when they appear in varied positions or sizes.
* **Transfer Learning:** The script uses a pre-trained "ImageNet" backbone, allowing you to achieve high accuracy with a relatively small dataset of your project's specific UI elements.

![Image: Unity Game View resolution settings demo](images\8.png)

## Intelligent Anchoring (Nine-Slice Regions)

The tool features a sophisticated `NineSliceRegion` system that calculates the optimal anchor points based on an element's position on the Canvas.



* **Dynamic Region Mapping:** Automatically assigns anchors to one of 9 regions: **Top (Left/Center/Right)**, **Middle (Left/Center/Right)**, or **Bottom (Left/Center/Right)**.
* **Proportional Scaling:** The Y-axis is split into a 1:2:1 ratio to provide the "Middle" region more flexibility for content-heavy UI layouts.
* **Full Stretch Detection:** Any element occupying >99% of the Canvas (like backgrounds) is automatically set to **Stretch-Stretch** with zeroed-out offsets.

---

## Hierarchy & Workflow Utilities

### 🗂️ Hierarchy Management
* **Z-Order Sorting:** Elements are sorted by their `z` value before generation, ensuring that the Unity Hierarchy matches the visual depth of your design.
* **Parent-Child Reconstruction:** The generator reconstructs complex, nested UI structures based on detection data.

### 🔧 Developer Productivity
* **Full Undo Support:** Every generation is registered with Unity's `Undo` system, allowing you to revert changes with a single `Ctrl + Z`.

---
[Back to Getting Started](getting-started.md) | [View FAQ](faq.md)