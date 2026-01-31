# Getting Started

> The **Auto UI Generator** empowers Unity Developers to transform static UI mockups into fully functional Unity UI hierarchies in seconds. By leveraging AI-powered image analysis, this tool bridges the gap between design and implementation.

## Technical Specifications

Before you begin, ensure your development environment meets these core requirements to guarantee a stable workflow.

### Operating System
**Windows (Required)**  
The AI-powered detection engine (`ui-detect.exe`) is optimized specifically for Windows-based workstations to ensure low-latency image analysis and reliable execution.

### Unity Support
**Unity 2019.4 LTS → Unity 6 (6000.3.6f1)**  
The package is fully compatible with all Long-Term Support (LTS) versions starting from Unity 2019.4 up to the latest Unity 6 releases.

## Step-by-Step Setup

Follow these steps to configure your project and generate your first UI layout.

### Step 1: Scene Preparation & Resolution Matching
For the AI to accurately map your mockup to the game world, your scene must match the original design's properties.
1. **Create a Canvas:** Add a Canvas to your scene and set the **Canvas Scaler** to `Scale With Screen Size`.
![Image: Unity Game View resolution settings demo](images\1.png)
2. **Match Aspect Ratio:** Set your Unity **Game View** resolution to the exact dimensions of your source mockup image (e.g., if your mockup is 1080x1920, set your Game View to 1080x1920).
![Image: Unity Game View resolution settings demo](images\2.png)


### Step 2: Open the Auto UI Tool
Launch the interface via **Tools > Auto UI Tools** or use the shortcut `Shift + A`.
![Image: Unity Game View resolution settings demo](images\3.png)
### Step 3: Input & Asset Mapping
Populate the tool with your project assets using a simple drag-and-drop workflow:
1. **Templates Assets:** Drag your project's UI Sprites or asset folders into the **"DROP FOLDERS / IMAGES HERE"** zone.
2. **Main Screenshot:** Drop the mockup image (the target design) into the **Main Screenshot** field.
3. **Target Root:** Drag the **RectTransform** of your Canvas (or a specific Panel) from the Hierarchy into this slot.
![Image: Unity Game View resolution settings demo](images\4.png)


### Step 4: Intelligent Detection Options
Choose what the AI should identify in the **Detection Options** section:
* **Detect Text (OCR):** Enable this to let the AI read text in the image and convert it into **TextMeshPro** objects automatically.
* **Detect Buttons:** Enable this to identify clickable elements and apply your custom **Button.prefab** logic.
![Image: Unity Game View resolution settings demo](images\5.png)
### Step 5: Execute Generation
Ensure the **Backend Status** indicator is **Green (✔ Backend Ready)**. Click **Apply UI**. The tool will process the data and build the UI hierarchy in your scene automatically.

![Image: Unity Game View resolution settings demo](images\6.png)

---
[Next Step: Explore Supported Features](features.md)