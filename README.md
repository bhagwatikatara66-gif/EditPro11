# EditProAI Offline Android Project (v1.1)

## Included and implemented in this starter
- Android WebView app shell that loads editor assets locally; no internet permission is declared.
- Select a local photo with Android's system file picker.
- Free in-project CSS/canvas templates: creator, story, sale, quote, photography, YouTube cover, wedding, food.
- Canvas sizes: Instagram portrait, square, Story/Reel, YouTube thumbnail, A4 poster, original image dimensions.
- Basic image adjustments: brightness, contrast, saturation, warmth, B&W/warm/vivid/fade/cool looks, vignette.
- Rotate 90 degrees and flip horizontally.
- Text and simple rectangle/circle-style shape layers; toggle visibility and delete.
- PNG and high-quality JPG export.
- Save/load basic project settings to JSON. Photo is not embedded; reselect it when reopening a project.
- GitHub Actions workflow for generating a debug APK.

## Build on GitHub from a phone
1. Download and extract this ZIP.
2. Create a repository at https://github.com/new called `EditProAI` (or `EditProAI-App`).
3. Upload the CONTENTS of the extracted folder into the repository root. Keep `.github/workflows/build-apk.yml`.
4. Commit to the `main` branch.
5. Open Actions and run `Build EditProAI APK`, if it did not start automatically.
6. When green/successful, open the run, download `EditProAI-debug-apk` under Artifacts, extract it and install `app-debug.apk`.

## Not implemented yet (do not assume present)
- True Photoshop-grade multi-layer raster compositing, masks, clipping masks, blend modes, path/pen tool, lasso/precise selection, clone stamp, healing/content-aware fill.
- RAW photo development, full Lightroom HSL/curves/color-grading pipeline, calibrated color management, advanced noise reduction and professional sharpening.
- AI background/object removal, generative fill, super-resolution/upscaling, face retouch AI. This build is offline and does not bundle those AI models.
- PSD/PSB compatibility, cloud sync, font packs, template marketplace.
- Full undo of pixel edits, crop selection UI, editable transforms/position handles and robust memory optimization for very large files.

## Quality and privacy
- Original photo is never intentionally overwritten; exports are new files.
- PNG is lossless for the rendered canvas, but editing/resizing can still reduce detail or crop parts of the image. Upscaling cannot recreate details missing from the source.
- Templates are made from original CSS/text/shapes in this project. No paid Canva or Adobe assets are included.
- This is a starter app, not a full Photoshop/Lightroom replacement. Test the APK on the target device before relying on it.
