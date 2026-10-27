# Frequently asked questions

## Is Free a timed trial?
No. There is no edition-imposed video-duration cap or watermark. It handles one video per task and factors up to 2x. RAM, VRAM, disk capacity and hardware speed still limit practical jobs.

## Which models are available?
RIFE 4.6 for interpolation and slow motion; Real-ESRGAN x4plus, x4plus Anime and AnimeVideo v3 for enhancement. The native model name does not override the Free output scaling limit of 2x.

## Does Free support CUDA?
Free uses Vulkan, also on NVIDIA GPUs. Supported CUDA options are part of the full edition.

## Can I set a target frame rate?
Yes, up to 2x the original frame rate. For example, a 30 FPS video can be interpolated to 60 FPS in Free.

## Why are the models not in the installer?
You choose which packages to install. The application shows download information and model licenses before installation.

## Are videos uploaded?
Video processing is local. Model downloads use their hosting services, which receive normal network connection data.

## Does it restore every missing detail?
No. Models can produce artifacts and cannot guarantee recovery of detail absent from a source. Test a short section and compare the result.

## What about AMD, Intel, Linux and CPU-only processing?
AMD, Intel and NVIDIA GPUs can use Vulkan if the GPU and vendor driver are compatible. Compatibility has not been physically validated on every GPU. This release is for Windows x64. No Linux installer or CPU-only AI mode is supplied.

## Why does Windows show an unrecognized-app warning?
This build is not digitally signed. Use the release checksum to compare the download. Never disable your antivirus to install it.

## Where is the app source code?
This is a distribution/support repository. Publishing a free-to-use edition does not release the FrameForge application source under an open-source license. Third-party code has its own licenses and corresponding-source obligations.
