> **General**

### Q: Why does the Backend Status show "Backend Not Ready"?
**A:** This is usually caused by one of the following:
1. The `ui-detect.exe` is missing or was blocked by antivirus software.
2. Port `38421` is being used by another application.
3. You haven't allowed the executable through your system Firewall.

### Q: How can I improve text detection accuracy?
**A:** Ensure **Detect Text (OCR)** is enabled in the Configuration panel. High-resolution mockups work best. Note that stylized or handwritten fonts may result in minor OCR errors.

### Q: Why are my generated sprites stretched?
**A:** The tool uses `SetNativeSize()` after assigning sprites. If the mockup dimensions differ significantly from your project's sprite assets, check the `Pixels Per Unit` settings in the Sprite Import settings.

### Q: Does the tool support multiple Canvases?
**A:** Yes. Drag any Canvas or UI root into the **Target Root** field. The tool will automatically locate the parent Canvas to calculate relative coordinates.

### Q: Why do some images appear as Magenta/Pink squares?
**A:** This occurs when the AI detects an element but cannot find a matching image in your **Templates** list. Ensure the filename of your sprite matches the element name in the detection data.

### Q: Why do I need to match the Game View ratio to the image ratio?
**A:** The tool calculates positions based on the screenshot's dimensions. If your Game View or Canvas has a different aspect ratio, the anchors and positions may shift during the `ApplyLayout` process.

### Q: Can I use custom fonts or button designs?
**A:** Yes. The tool uses prefabs located at `Assets/Auto UI Generator/Editor/Prefabs/`.
* **For Text:** Customize `Text.prefab` to set your default Font Asset.
* **For Buttons:** Customize `Button.prefab` to set your default transitions and scripts.