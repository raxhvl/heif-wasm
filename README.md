## Context
[HEIF](https://en.wikipedia.org/wiki/High_Efficiency_Image_File_Format) is a standard developed by the Moving Picture Experts Group (MPEG) for storage and sharing of images and image sequences. It offers superior quality, compression, and the higher color depth support than JPEG.

HEIF was adopted by Apple in 2017 with the introduction of iOS 11, and support on other platforms is growing.

## Problem statement
There is no native browser support for HEIF at the moment ([Can I use HEIF?](https://caniuse.com/heif) ). Currently, we are rendering HEIF using https://github.com/catdad-experiments/libheif-emscripten but are running into performace issues. 

We want package this library as a wasm module to leverage native performance for rendering HEIF inside a browser environment.
