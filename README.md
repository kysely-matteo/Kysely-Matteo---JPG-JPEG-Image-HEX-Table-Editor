# JPG/JPEG IMAGE HEX TABLE EDITOR

A browser-based tool for glitching JPEG images by directly editing their internal data — no re-encoding, no quality loss, just raw byte manipulation.

---

## What it does

### QT Value Editing
JPEG images store **Quantisation Tables (QT)** that control how image data is compressed. By tweaking these values you can introduce glitchy compression artifacts — blocky distortions, color bleeds, and psychedelic noise — while keeping the file a valid JPEG.

- **Blue cells** = Luminance table (brightness/luma data)
- **Red cells** = Chrominance table (color data)

Crank values up for heavy glitch, go low for subtle artifacts.

### Width / Height Warping
The JPEG frame header stores the image dimensions as raw bytes. Changing these fools the decoder into misreading the image geometry — stretching, squashing, or shearing the image in ways that can't be achieved through normal editing.

---

## Usage

1. Drop a `.jpg` / `.jpeg` onto the left panel
2. Edit hex values in the grid — changes preview live
3. Optionally warp the dimensions in the **Aspect Ratio Glitching** panel
4. Hit **↓ Download Glitched JPEG** to save

No install, no dependencies — just open the HTML file in a browser.
