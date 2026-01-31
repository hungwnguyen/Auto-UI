# Introduction
> **Auto UI Generator: The bridge between design mockups and Unity production.**

<center>

<iframe width="100%" height="450" src="//www.youtube.com/embed/6stlCkUDG_s?si=gRfKQXVDOrreWA3B" title="Auto UI Generator Demo" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

</center>

**Auto UI Generator** is a specialized Unity Editor tool designed to automatically generate Unity UI from a single screenshot. Instead of manually recreating layouts from Figma or Photoshop, this tool analyzes your design image, detects elements, and converts them into production-ready Unity UI—including Images, Text, and Buttons—with precise layout, anchors, and hierarchy.

---

## What Problem Does It Solve?
Building UI in Unity is traditionally a bottleneck in game development. It is often:
* ⏱ **Time-consuming**: Manual drag-and-drop for every element.
* 🔄 **Repetitive**: Setting up the same components for dozens of screens.
* ⚠️ **Error-prone**: Tedious work when configuring anchors and scaling.
* 📐 **Inconsistent**: Difficult to maintain pixel-perfect alignment with design mockups.

**Auto UI Generator** solves this by using image-based detection and smart layout rules. You focus on design and logic the tool handles the setup.

---

## How It Works (High-Level)

1. **Input**: You provide a UI screenshot (from Figma, Photoshop, or any mockup).
2. **Assets**: You provide the template sprites used in that UI.
3. **Analysis**: The backend detection system analyzes the image and returns UI element data.
4. **Generation**: Unity Editor generates the UI automatically inside your Canvas.
5. **Output**: All elements are standard **Unity UGUI** components and fully editable.

---

## Core Features

### 🖼 Screenshot-Based UI Generation
* Compatible with PNG / JPG screenshots.
* Supports designs from Figma, Photoshop, Sketch, and more.

### 🧠 Smart Element Detection
* **Image elements**: Precise shape and color detection.
* **Text (OCR)**: Automatic text extraction and font mapping.
* **Button detection**: Identifies interactive regions automatically.
* **Z-order sorting**: Maintains the correct layering hierarchy.

### 📐 Automatic Layout & Anchors
* **Auto-stretch**: Full-screen elements are configured automatically.
* **Smart Anchors**: Non-fullscreen elements get anchors based on their relative region (Top, Center, Bottom, etc.).
* **Responsive**: Calculated based on your specific Canvas resolution.

### 🎨 Template-Based Sprite Matching
* Drag & drop template folders or individual images.
* Sprites are matched automatically by filename or visual properties.

### 🛠 Unity Editor Integration
* **No runtime code**: Everything happens in the Editor.
* **Clean Hierarchy**: Generates standard, editable RectTransforms.

---

## Typical Use Cases
* 🎮 **Game UI prototyping**: Go from concept to engine in seconds.
* 🚀 **Rapid UI iteration**: Test different layouts without manual rebuilding.
* 🎨 **Designer-to-developer handoff**: Reduce friction between departments.
* 📱 **Multi-resolution setup**: Quickly verify how UI scales across devices.

---

## What This Tool Is (and Is Not)

| ✔ What It Is | ✖ What It Is Not |
| :--- | :--- |
| A productivity tool for developers | A replacement for UI design tools |
| A UI generator (creates editable objects) | A runtime UI renderer |
| A starting point for clean, production UI | A "one-click final UI" (fine-tuning is expected) |

---

## Requirements

### 🖥 Operating System
* **Windows**: Currently, the Auto UI Generator is optimized and required to run on **Windows OS**.

### 🎮 Unity Version Support
The tool has been extensively tested and is confirmed to work across a wide range of Unity versions. Whether you are on an older LTS or the latest cutting-edge release, Auto UI Generator maintains high stability.

**Confirmed Working Versions:**
* **Unity 2019.4.41f2** (LTS)
* **Unity 2020.3.49f1** (LTS)
* **Unity 2021.3.42f1** (LTS)
* **Unity 2022.3.62f2** (LTS)
* **Unity 2023.1.22f1**
* **Unity 6000.3.6f1** (Unity 6)

### 🛠 UI System
* **UGUI**: Designed specifically for the **Canvas-based UI (UGUI)** system.
* **Knowledge**: A basic understanding of RectTransforms, Anchors, and the Unity UI workflow is recommended for fine-tuning results.

---

## Next Steps

Now that you understand the concept, you can proceed to:

1. [Set up your first UI generation](getting-started)
2. [Prepare template assets correctly](sprite-matching)
3. [Understand layout and anchor logic](layout-logic)

👉 **Ready to begin?** Start with [Getting Started](getting-started) to generate your first UI in minutes.