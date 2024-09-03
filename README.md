# Awesome HDR in the Browser [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of awesome tools, issues, resources and other awesomeness. Inspired by [awesome-python](https://github.com/vinta/awesome-python), [awesome-bigdata](https://github.com/oxnr/awesome-bigdata) & [awesome](https://github.com/sindresorhus/awesome) itself.

Your [contributions](./contributing.md) are always welcome!

The list is about displaying [HDR](https://en.wikipedia.org/wiki/High_dynamic_range) contents in a browser, currently leaning heavily towards images. HDR video might be added later. This is is only a list, it doesn't contain an introduction. A great good starting point on the topic is the [HDR page by Greg Benz](https://gregbenzphotography.com/hdr/).

## Contents

- [Formats](#formats)
- [Tools](#tools)
- [Ressources](#ressources)

## Formats

There are more HDR image formats (like [OpenEXR](https://openexr.com/en/latest/), [JPEG XR](https://jpeg.org/jpegxr/), [JPEG XT](https://jpeg.org/jpegxt/)), this list only only contains those that are supported by current browsers.

### Images

- [Ultra HDR](https://developer.android.com/media/platform/hdr-image-format)
  - [Gainmap specification](https://helpx.adobe.com/camera-raw/using/gain-map.html)
- [AVIF (HDR)](https://en.wikipedia.org/wiki/AVIF)
- [JPEG XL](https://jpeg.org/jpegxl/)
- [PNG](https://github.com/w3c/ColorWeb-CG/blob/main/hdr-in-png-requirements.md) - with HDR support.

### Video

Several video formats support HDR videos, sites like YouTube usually support some or all of the above, see also [Wikipedia on HDR video / television](https://en.wikipedia.org/wiki/High-dynamic-range_television).

#### Container formats

These container formats allow the for HDR require metadata.

- MKV
- MOV/QuickTime
- MP4

#### Codecs

These formats support HDR video content. there are others as well, but those usually have very limited browser support, if at all.

- AV1
- HEVC/H.265
- VP9 Profile 2

### 3D

#### WebGPU

- [WebGPU Extended Range Brightness](https://github.com/ccameron-chromium/webgpu-hdr/blob/main/EXPLAINER.md)

#### WebGL

- [WebGL Extended Range Brightness](https://github.com/ccameron-chromium/webgl-hdr)

### Browser support

Since browser change rapidly this list might be outdated soon, currently there is an afford to [add this data to CanIUse](https://github.com/Fyrd/caniuse/issues/6759).



## Tools

Currently graphic programs are missing. The focus is (currently) on libraries and command line tools.

### AVIF HDR

- [Avif HDR diagnostic page](https://alexfry.github.io/ACES_ODT_Candidates_Examples/diagnostic.html)

### Ultra HDR (Adobe Gain Map)

### General

- [OpenHDR Viewer (Browser based)](https://viewer.openhdr.org/)

#### `libultrahdr`
- [`libultrahdr` on GitHub](https://github.com/google/libultrahdr)
- [`libultrahdr` and Python](https://github.com/albertz/playground/blob/master/ultrahdr.py)
  - [discussion](https://www.reddit.com/r/Python/comments/1ac8ooy/playing_around_with_ultra_hdr/?utm_source=share&utm_medium=web3x&utm_name=web3xcss&utm_term=1&utm_content=share_button)
  - [demo](https://github.com/albertz/playground/wiki/HDR-demo) - by [Albert Zeyer](https://github.com/albertz)

#### Other

- [Gainmap Creator](https://gainmap-creator.monogrid.com/)
- [`gainmap-js`](https://github.com/MONOGRID/gainmap-js) - A JavaScript (TypeScript) Port of Adobe Gainmap Technology for storing HDR Images using an SDR Image + a gainmap.
- [`libultrahdr-wasm`](https://github.com/MONOGRID/libultrahdr-wasm) - WASM build of `libultrahdr.

### Apple HDR

- [Applying Apple HDR effect to your photos](https://developer.apple.com/documentation/appkit/images_and_pdf/applying_apple_hdr_effect_to_your_photos)
- [AppleJPEGGainMap](https://github.com/grapeot/AppleJPEGGainMap)

### Viewer / Desktop browsers

Currently the only [Chrome](https://www.google.com/chrome/) seems to be able to display Ultra HDR images.
Since it's based on Chromium, other Browsers using this base will work as well, some might need to be configured accordingly:
- [Edge](https://www.microsoft.com/en-us/edge) - works.
- [Brave](https://brave.com/) - needs configuration - `brave://flags/#gainmap-hdr-images`.
- [Opera](https://www.opera.com/) - need configuration - `opera://flags/#gainmap-hdr-images`.
- [Vivaldi](https://vivaldi.com/) - need configuration.

Firefox currently only has limited HDR support.

### Issues / feature requests for important tools

The first step to foster the adoption of HDR in the browser is to improve tooling. Several projects already have requests to improve support for UltraHDR JPEGs.

- [LibVips](https://github.com/libvips/libvips/issues/3799)
- [ImageMagick](https://github.com/ImageMagick/ImageMagick/issues/6377)
- [Tev](https://github.com/Tom94/tev/issues/226)
- [HDRImageViewer](https://github.com/13thsymphony/HDRImageViewer/issues/66)
- [`ffmpeg`](https://trac.ffmpeg.org/ticket/10974)
- [Python Pillow](https://github.com/python-pillow/Pillow/issues/8036)
- [memories](https://github.com/pulsejet/memories/issues/1110)
- [CanIUse](https://github.com/Fyrd/caniuse/issues/6759)
- [`libjxl`](https://github.com/libjxl/libjxl/issues/2685)

## Ressources

The specifications and technical documentations are linked in the first section on file formats.

### Documentation

### Examples
- [Greg Benz on HDR](https://gregbenzphotography.com/hdr/)

### Other HDR **awesome** lists
Mostly outdated / unmaintained

- [Awesome-Deep-HDR](https://github.com/vinthony/awesome-deep-hdr) - A collection of deep learning based methods for HDR image synthesis.
- [Awesome-HDR](https://github.com/ytZhang99/Awesome-HDR) - Collect High Dynamic Range Imaging (especially for Multi-exposure Fusion and High Dynamic Range Imaging) Related Papers and Codes.
- [Awesome HDR Deghosting](https://github.com/liuzhen03/awesome-hdr-deghosting) - A curated list of multi-frame HDR deghosting resources.
- [awesome-hdr-imaging](https://github.com/Jonashwang/awesome-hdr-imaging) - A collection of methods for high dynamic range imaging High dynamic range imaging is an important topic on image processing, especially in mobile photography.
