# FrameForge 1.2.1 — Upscaling reliability update

A reported upscaling failure was reproduced and fixed. Under the previous settings, Real-ESRGAN could exhaust GPU memory while processing multiple frames, write black images and still return a successful exit code.

## What changed
- Lower GPU memory pressure during upscaling, using smaller tiles and a single GPU processing worker.
- Vulkan errors are detected even if the model exits with code zero.
- Automatic retries with smaller tiles after a GPU failure.
- Black-frame checks and the same recovery path for AI previews and exports.
- Cancellation and unrelated errors are not retried.

## Validation
The original failure was reproduced on an RTX 3080. The corrected build passed short 854×480 to 1708×960 exports with all three Real-ESRGAN models available in Free, plus an AI preview. Nine recovery tests and four resolution/clip tests also passed. This is not a guarantee for every GPU; this patch has not been physically retested on AMD or Intel.

Thank you for reporting problems. Each reproducible report helps improve FrameForge. If an issue remains, send the app version, GPU, model and error text to iheel.support@gmail.com.

---

# Changelog

## FrameForge Free 1.2.0

- Separate Free installer, application identity, settings and default model storage.
- RIFE 4.6 interpolation and slow motion up to 2x.
- Three Real-ESRGAN enhancement profiles, output upscaling up to 2x.
- One video per processing task; no watermark or edition-imposed duration cap.
- Image adjustments, preview comparison, clip selection, block processing and configurable temporary storage.
- Optional model downloads with confirmation and license acceptance.
- Interface and installer in English, Portuguese (Brazil), Spanish, Russian, French and German.

Known limitations: unsigned Windows build; Vulkan/driver requirements; no CPU-only AI mode; very long installation paths may exceed Windows/.NET path limits. Hardware compatibility and performance vary.
