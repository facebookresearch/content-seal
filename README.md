<div align="center">

<img src="static/images/meta-logo-black.png" width="180" alt="Meta">

# Content Seal

### State-of-the-Art Invisible Watermarking

[![Website](https://img.shields.io/badge/Website-Visit-blue)](https://facebookresearch.github.io/meta-seal)
[![License: MIT](https://img.shields.io/badge/License-MIT-green)](LICENSE)

**[Visit the Content Seal Website →](https://facebookresearch.github.io/meta-seal)**

</div>

---

Content Seal is a comprehensive framework for invisible, robust watermarking across **all modalities** — audio, image, video, and text. It spans the entire generative AI lifecycle, from training data and inference to generated media, providing state-of-the-art tools for content provenance and authentication.

<div align="center">

![Content Seal Overview](assets/banner_vid2.gif)

</div>

## Contents

- [Post-Hoc Watermarking](#post-hoc-watermarking)
- [In-Model and Generation-Time Watermarking](#in-model-and-generation-time-watermarking)
- [Watermark Security](#watermark-security)
- [License](#license)

Each entry links to its paper; the badge links to the GitHub repository (and shows its stars).

---

## Post-Hoc Watermarking

Watermarks applied **after content generation** by any model or system — model-agnostic and universal across all content types.

<div align="center">

![Post-Hoc Watermarking](assets/2025-12-posthoc.gif)

</div>

### Content Seal for Images and Video

Content Seal Image is deployed at scale for Muse Image with a custom proprietary implementation. We also provide open-source versions of our research models for images and video, readily available to download.

- [Pixel Seal: Adversarial-Only Training for Invisible Image and Video Watermarking](https://ai.meta.com/research/publications/pixel-seal-adversarial-only-training-for-invisible-image-and-video-watermarking/) — Flagship image & video watermarking model, SOTA in robustness and imperceptibility, built with a more stable adversarial-only training paradigm. [![Stars](https://img.shields.io/github/stars/facebookresearch/videoseal?style=social)](https://github.com/facebookresearch/videoseal)
- [We Can Hide More Bits: The Unused Watermarking Capacity in Theory and in Practice](https://arxiv.org/abs/2510.12812) — Bigger model with 4× capacity boost to 1024 bits while preserving quality and robustness. [![Stars](https://img.shields.io/github/stars/facebookresearch/videoseal?style=social)](https://github.com/facebookresearch/videoseal)
- [Video Seal: Open and Efficient Video Watermarking](https://arxiv.org/abs/2412.09492) — Extension of image watermarking models to video, resilient to editing and video codecs. [Demo](https://aidemos.meta.com/videoseal) · [![Stars](https://img.shields.io/github/stars/facebookresearch/videoseal?style=social)](https://github.com/facebookresearch/videoseal)
- [Watermark Anything with Localized Messages](https://arxiv.org/abs/2411.07231) — Embed (possibly multiple) localized watermarks into images; survives inpainting and splicing attacks. [![Stars](https://img.shields.io/github/stars/facebookresearch/watermark-anything?style=social)](https://github.com/facebookresearch/watermark-anything)
- [Geometric Image Synchronization with Deep Watermarking](https://arxiv.org/abs/2509.15208) — Robust image synchronization, enabling reversal of geometric transformations applied to an image. [![Stars](https://img.shields.io/github/stars/facebookresearch/watermark-anything?style=social)](https://github.com/facebookresearch/watermark-anything)

### Content Seal for Audio

- [Proactive Detection of Voice Cloning with Localized Watermarking](https://arxiv.org/abs/2401.17264) — Localized audio watermarking with sample-level detection and streaming support for real-time applications. [![Stars](https://img.shields.io/github/stars/facebookresearch/audioseal?style=social)](https://github.com/facebookresearch/audioseal)

### Content Seal for Text

- [How Good is Post-Hoc Watermarking With Language Model Rephrasing?](https://arxiv.org/abs/2512.16904) — Comprehensive evaluation framework for post-hoc text watermarking with LLM rephrasing. [![Stars](https://img.shields.io/github/stars/facebookresearch/textseal?style=social)](https://github.com/facebookresearch/textseal)

---

## In-Model and Generation-Time Watermarking

Watermarks embedded **during content generation** by modifying model behavior or latent representations.

<div align="center">

![In-Model Watermarking](assets/2025-12-inmodel.gif)

</div>

### Content Seal for Text

- [TextSeal: A Localized LLM Watermark for Provenance & Distillation Protection](https://arxiv.org/abs/2605.12456) — SOTA LLM watermark with dual-key Gumbel-max sampling, entropy-weighted scoring, and multi-region localization. Distortion-free, preserves reasoning and benchmark performance, detectable when diluted in human text, radioactive through distillation. [![Stars](https://img.shields.io/github/stars/facebookresearch/textseal?style=social)](https://github.com/facebookresearch/textseal)

### Content Seal for Image & Audio

- [Learning to Watermark in the Latent Space of Generative Models](https://ai.meta.com/research/publications/distilling-latent-space-watermarkers-into-generative-image-models/) — Unified latent-space watermarking that enables 20× speedup over pixel methods and secures open-source models via in-model distillation. [![Stars](https://img.shields.io/github/stars/facebookresearch/distseal?style=social)](https://github.com/facebookresearch/distseal)
- [The Stable Signature: Rooting Watermarks in Latent Diffusion Models](https://arxiv.org/abs/2303.15435) — Roots the watermark in the model's latent decoder for tracing the outputs of latent generative models. [![Stars](https://img.shields.io/github/stars/facebookresearch/stable_signature?style=social)](https://github.com/facebookresearch/stable_signature)
- [Watermarking Autoregressive Image Generation](https://arxiv.org/abs/2506.16349) — Watermarking for autoregressive image generation models. [![Stars](https://img.shields.io/github/stars/facebookresearch/wmar?style=social)](https://github.com/facebookresearch/wmar)

### Radioactivity

- [Watermarking Makes Language Models Radioactive](https://arxiv.org/abs/2402.14904) — Detects if a language model was trained on synthetic text by finding weak residuals of watermark signals in fine-tuned LLMs — high-confidence even when as little as 5% of training text is watermarked. [![Stars](https://img.shields.io/github/stars/facebookresearch/radioactive-watermark?style=social)](https://github.com/facebookresearch/radioactive-watermark)
- [Detecting Benchmark Contamination Through Watermarking](https://arxiv.org/abs/2502.17259) — Watermarks benchmarks before release to detect if models were trained on test sets, using theoretically grounded statistical tests while preserving benchmark utility. [![Stars](https://img.shields.io/github/stars/facebookresearch/textseal?style=social)](https://github.com/facebookresearch/textseal)

---

## Watermark Security

Research on **adversarial attacks and defenses** for watermarking systems through red teaming.

<div align="center">

![Security Demo](assets/2025-12-forger.gif)

</div>

- [Transferable Black-Box One-Shot Forging of Watermarks via Image Preference Models](https://arxiv.org/abs/2510.20468) — Black-box watermark forging using image preference models for red-teaming watermarking systems. [![Stars](https://img.shields.io/github/stars/facebookresearch/videoseal?style=social)](https://github.com/facebookresearch/videoseal/tree/main/wmforger)

---

## License

The code is licensed under an [MIT license](LICENSE).
