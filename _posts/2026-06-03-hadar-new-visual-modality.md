---
title: "HADAR: Toward a New Visual Modality Beyond Appearance"
date: 2026-06-03
permalink: /posts/2026/06/hadar-new-visual-modality/
tags:
  - HADAR
  - thermal hyperspectral imaging
  - physical vision
  - TeX
  - dataset
---

Most machine vision systems still see the world through proxies. RGB records how a scene appears under visible illumination. Depth sensors estimate geometry by projecting or receiving structured signals. These modalities have enabled remarkable progress, but they do not directly describe the stable physical properties of objects. They are sensitive to lighting, weather, surface reflectance, transparency, and occlusion.

HADAR, short for heat-assisted detection and ranging, points to a different route: sensing the world through thermal radiation and recovering physical attributes from it. The original HADAR work, led by my advisor Fanglin Bao and published in *Nature* in 2023, formulated ground-based thermal perception using a radiative-transfer view of the scene. For an observed pixel or object element \(\alpha\), the measured thermal spectrum can be written conceptually as

```text
S_alpha = e_alpha B(T_alpha)
        + (1 - e_alpha) sum_{beta != alpha} S_beta V_{alpha beta}.
```

The first term is self-emission: an object radiates according to its temperature \(T\), emissivity \(e\), and Planck's blackbody law \(B(T)\). The second term is reflected environmental thermal radiation: each surface also reflects heat from the surrounding scene. In other words, a thermal hyperspectral image is not merely a blurry temperature map. It is a mixture of temperature, material response, geometry, and environmental illumination.

The key idea of HADAR is to invert this mixture. Instead of only producing an infrared image, HADAR tries to decompose the observed heat signal into a TeX representation: temperature, emissivity, and texture. In the first version of HADAR, texture was defined from the reflected environmental radiance. In our later internal formulation, which I call HADAR-v2 here, texture becomes a more learnable scalar factor determined jointly by scene geometry, emissivity, and sky/environmental structure.[^hadar-v2] This change matters because it turns texture from an unstable exposure-dependent radiance field into a physical coordinate that learning systems can better approximate.

Put simply: a single passive thermal hyperspectral observation can, in principle, reveal temperature, material emissivity, texture-like geometric structure, depth cues, humidity, and atmospheric pressure. This is why I see HADAR not as a better infrared camera, but as a candidate for a new physical visual modality.

Why is such a modality needed? RGB perception breaks under extreme illumination contrast: darkness, fog, glare, strong reflections from metal, and partial occlusion can all destroy the signal. Depth sensing has its own failure modes. LiDAR and structured-light systems struggle with transparent surfaces, mirrors, highly reflective or absorptive materials, multi-path interference, rain, dust, and long-range energy cost. Stereo depth depends on visible texture and illumination. Time-of-flight sensors can be confused by ambient light and surface reflectance. More importantly, many depth systems are active: they must emit light or laser pulses. That costs power, can be fragile in outdoor deployment, and may even damage sensitive imaging electronics in some real-world settings.

These limitations are not just engineering inconveniences. They arise because conventional visual signals are sensing proxies: they describe how a scene appears to a sensor, rather than directly representing the object's stable physical properties. HADAR changes the question. Since every object emits and reflects thermal radiation, thermal hyperspectral sensing can operate passively. It does not need headlights, projected patterns, or active laser illumination to begin extracting physical information from a scene.

The current limitation is equally clear: HADAR is still expensive and technically hard. Thermal hyperspectral cameras can cost hundreds of thousands of dollars. Hardware noise, spectral interference, calibration drift, low signal-to-noise ratios, and unstable acquisition conditions can easily overwhelm the physical signal. These problems directly affect the recognizability of TeX fields. Algorithmic work can reduce the burden, but the bottleneck is not only software. Hardware, calibration, acquisition protocols, and scalable datasets all matter.

Our recent work is therefore still at an early stage, but it is beginning to form a pipeline. TAG studies universal computational thermal imaging and anti-ghosting. HAIR introduces a HADAR-based restoration framework for thermal infrared hyperspectral images. TeX-1500 builds, to the best of our knowledge, the first large-scale paired real-world LWIR hyperspectral dataset for supervised temperature-emissivity-texture decomposition. TeX-1500 is imperfect, as any first dataset in a new modality must be, but it opens an important door: lightweight real-time models can now be trained to approximate HADAR-style physical decomposition on the edge.

This is the direction I am most excited about. The long-term goal is not simply to make prettier night-vision images. It is to build AI systems that see physical properties rather than only appearance. If HADAR can be made cheaper, more robust, and more learnable, it could complement or even reshape the current RGB-depth-centered perception stack for autonomous driving, robotics, remote sensing, safety monitoring, and scientific imaging.

For now, HADAR remains a young field with difficult physics and difficult hardware. But that is also why it is interesting. A new sensing modality does not become useful because it is immediately convenient. It becomes useful when it reveals information that existing modalities fundamentally miss.

## Related Work

- HADAR: [Heat-assisted detection and ranging](https://www.nature.com/articles/s41586-023-06174-6)
- TAG: [Universal computational thermal imaging overcoming the ghosting effect](https://arxiv.org/abs/2604.01542)
- HAIR: [HADAR-Based Thermal Infrared Hyperspectral Image Restoration](https://arxiv.org/abs/2605.13664)
- TeX-1500: [A Paired Real-World LWIR Hyperspectral Dataset and Benchmark for Temperature-Emissivity-Texture Decomposition](https://arxiv.org/abs/2606.03806)

[^hadar-v2]: HADAR-v2 is unpublished work. I mention it here only to clarify the evolving definition of texture in our internal research line.
