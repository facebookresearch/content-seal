<div align="center">

<img src="static/images/meta-logo-black.png" width="180" alt="Meta">

# Content Seal

### State-of-the-Art Invisible Watermarking

[![Website](https://img.shields.io/badge/Website-Visit-blue)](https://facebookresearch.github.io/meta-seal)
[![License: MIT](https://img.shields.io/badge/License-MIT-green)](LICENSE)

**[Visit the Content Seal Website →](https://facebookresearch.github.io/content-seal)**

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

---

## Post-Hoc Watermarking

Watermarks applied **after content generation** by any model or system — model-agnostic and universal across all content types.

<div align="center">

![Post-Hoc Watermarking](assets/2025-12-posthoc.gif)

</div>

### Content Seal for Images and Video

Content Seal Image is deployed at scale for Muse Image with a custom proprietary implementation. We also provide open-source versions of our research models for images and video, readily available to download.

| Research | Links |
|:---|:---|
| **Pixel Seal: Adversarial-Only Training for Invisible Image and Video Watermarking**<br>Flagship image & video watermarking model, SOTA in robustness and imperceptibility, built with a more stable adversarial-only training paradigm. | [![Paper](https://img.shields.io/badge/Paper-Meta_AI-0866FF?style=flat-square&logo=meta&logoColor=white)](https://ai.meta.com/research/publications/pixel-seal-adversarial-only-training-for-invisible-image-and-video-watermarking/) [![Code](https://img.shields.io/badge/Code-GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/facebookresearch/videoseal) |
| **We Can Hide More Bits: The Unused Watermarking Capacity in Theory and in Practice**<br>Bigger model with 4× capacity boost to 1024 bits while preserving quality and robustness. | [![Paper](https://img.shields.io/badge/Paper-arXiv-b31b1b?style=flat-square&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.12812) [![Code](https://img.shields.io/badge/Code-GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/facebookresearch/videoseal) |
| **Video Seal: Open and Efficient Video Watermarking**<br>Extension of image watermarking models to video, resilient to editing and video codecs. | [![Paper](https://img.shields.io/badge/Paper-arXiv-b31b1b?style=flat-square&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2412.09492) [![Code](https://img.shields.io/badge/Code-GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/facebookresearch/videoseal) [![Demo](https://img.shields.io/badge/Demo-Live-1877F2?style=flat-square&logo=meta&logoColor=white)](https://aidemos.meta.com/videoseal) |
| **Watermark Anything with Localized Messages**<br>Embed (possibly multiple) localized watermarks into images; survives inpainting and splicing attacks. | [![Paper](https://img.shields.io/badge/Paper-arXiv-b31b1b?style=flat-square&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2411.07231) [![Code](https://img.shields.io/badge/Code-GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/facebookresearch/watermark-anything) |
| **Geometric Image Synchronization with Deep Watermarking**<br>Robust image synchronization, enabling reversal of geometric transformations applied to an image. | [![Paper](https://img.shields.io/badge/Paper-arXiv-b31b1b?style=flat-square&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.15208) [![Code](https://img.shields.io/badge/Code-GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/facebookresearch/watermark-anything) |

### Content Seal for Audio

| Research | Links |
|:---|:---|
| **Proactive Detection of Voice Cloning with Localized Watermarking**<br>Localized audio watermarking with sample-level detection and streaming support for real-time applications. | [![Paper](https://img.shields.io/badge/Paper-arXiv-b31b1b?style=flat-square&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2401.17264) [![Code](https://img.shields.io/badge/Code-GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/facebookresearch/audioseal) |

### Content Seal for Text

| Research | Links |
|:---|:---|
| **How Good is Post-Hoc Watermarking With Language Model Rephrasing?**<br>Comprehensive evaluation framework for post-hoc text watermarking with LLM rephrasing. | [![Paper](https://img.shields.io/badge/Paper-arXiv-b31b1b?style=flat-square&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2512.16904) [![Code](https://img.shields.io/badge/Code-GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/facebookresearch/textseal) |

---

## In-Model and Generation-Time Watermarking

Watermarks embedded **during content generation** by modifying model behavior or latent representations.

<div align="center">

![In-Model Watermarking](assets/2025-12-inmodel.gif)

</div>

### Content Seal for Text

| Research | Links |
|:---|:---|
| **TextSeal: A Localized LLM Watermark for Provenance & Distillation Protection**<br>SOTA LLM watermark with dual-key Gumbel-max sampling, entropy-weighted scoring, and multi-region localization. Distortion-free, preserves reasoning and benchmark performance, detectable when diluted in human text, radioactive through distillation. | [![Paper](https://img.shields.io/badge/Paper-arXiv-b31b1b?style=flat-square&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.12456) [![Code](https://img.shields.io/badge/Code-GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/facebookresearch/textseal) |

### Content Seal for Image & Audio

| Research | Links |
|:---|:---|
| **Learning to Watermark in the Latent Space of Generative Models**<br>Unified latent-space watermarking that enables 20× speedup over pixel methods and secures open-source models via in-model distillation. | [![Paper](https://img.shields.io/badge/Paper-Meta_AI-0866FF?style=flat-square&logo=meta&logoColor=white)](https://ai.meta.com/research/publications/distilling-latent-space-watermarkers-into-generative-image-models/) [![Code](https://img.shields.io/badge/Code-GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/facebookresearch/distseal) |
| **The Stable Signature: Rooting Watermarks in Latent Diffusion Models**<br>Roots the watermark in the model's latent decoder for tracing the outputs of latent generative models. | [![Paper](https://img.shields.io/badge/Paper-arXiv-b31b1b?style=flat-square&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2303.15435) [![Code](https://img.shields.io/badge/Code-GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/facebookresearch/stable_signature) |
| **Watermarking Autoregressive Image Generation**<br>Watermarking for autoregressive image generation models. | [![Paper](https://img.shields.io/badge/Paper-arXiv-b31b1b?style=flat-square&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.16349) [![Code](https://img.shields.io/badge/Code-GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/facebookresearch/wmar) |

### Radioactivity

| Research | Links |
|:---|:---|
| **Watermarking Makes Language Models Radioactive**<br>Detects if a language model was trained on synthetic text by finding weak residuals of watermark signals in fine-tuned LLMs — high-confidence even when as little as 5% of training text is watermarked. | [![Paper](https://img.shields.io/badge/Paper-arXiv-b31b1b?style=flat-square&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2402.14904) [![Code](https://img.shields.io/badge/Code-GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/facebookresearch/radioactive-watermark) |
| **Detecting Benchmark Contamination Through Watermarking**<br>Watermarks benchmarks before release to detect if models were trained on test sets, using theoretically grounded statistical tests while preserving benchmark utility. | [![Paper](https://img.shields.io/badge/Paper-arXiv-b31b1b?style=flat-square&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2502.17259) [![Code](https://img.shields.io/badge/Code-GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/facebookresearch/textseal) |

---

## Watermark Security

Research on **adversarial attacks and defenses** for watermarking systems through red teaming.

<div align="center">

![Security Demo](assets/2025-12-forger.gif)

</div>

| Research | Links |
|:---|:---|
| **Transferable Black-Box One-Shot Forging of Watermarks via Image Preference Models**<br>Black-box watermark forging using image preference models for red-teaming watermarking systems. | [![Paper](https://img.shields.io/badge/Paper-arXiv-b31b1b?style=flat-square&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.20468) [![Code](https://img.shields.io/badge/Code-GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/facebookresearch/videoseal/tree/main/wmforger) |

---

## License

The code is licensed under an [MIT license](LICENSE).
