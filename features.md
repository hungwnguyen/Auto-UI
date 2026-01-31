# Supported Features

The **Auto UI Generator** provides several advanced features to streamline the bridge between UI Design and Development.

## 1. AI-Powered Detection
* **OCR (Optical Character Recognition):** Automatically extracts text content from your mockup and assigns it to TextMeshPro components.
* **Button Matching:** Identifies potential buttons in the image and applies your custom Button Prefab logic.
* **Sprite Matching:** Compares mockup regions against your `Templates` library to find and assign the correct source sprites.

## 2. Intelligent Anchoring (Nine-Slice Regions)
The tool calculates coordinates to assign optimized **Anchors** based on screen position:
* **Standard Regions:** Top-Left, Top-Center, Top-Right, Middle-Left, Center, Middle-Right, and Bottom regions.
* **Full Stretch:** Elements occupying >99% of the screen are automatically set to Stretch-Stretch with zero offsets.

## 3. Hierarchy Management
* **Z-Order Sorting:** Elements are automatically ordered in the hierarchy based on the depth (z) data from the analysis.
* **Nested UI Support:** Supports Parent-Child relationships to maintain a clean and organized hierarchy.

## 4. Utility Tools
* **Sprite Converter:** Quickly converts Sprite assets into Texture2D format for AI processing.
* **Screenshot Tool:** Capture high-quality screenshots of your Game View directly within the Editor.
* **Undo Support:** Fully integrated with Unity's Undo system, allowing you to revert generation with `Ctrl + Z`.