<h1 align="center">Awesome MM-RAG</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Project-Awesome--MM--RAG-blue.svg" alt="Project Badge" />
  <img src="https://img.shields.io/github/stars/INTREBID/Awesome-MM-RAG?style=social" alt="GitHub Stars" />
  <img src="https://img.shields.io/github/forks/INTREBID/Awesome-MM-RAG?style=social" alt="GitHub Forks" />
  <img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg" alt="PRs Welcome" />
  <img src="https://img.shields.io/badge/Made%20with-%F0%9F%A4%96%20AI-red.svg" alt="Made with AI" />
  <a href="https://doi.org/10.36227/techrxiv.176341513.38473003/v1">
    <img src="https://img.shields.io/badge/DOI-10.36227%2Ftechrxiv.176341513.38473003%2Fv1-orange?logo=doi" alt="DOI" />
  </a>
</p>

<div align="center">
[<a href="https://doi.org/10.36227/techrxiv.176341513.38473003/v1">TechRxiv</a>]
</div>
This repository is for our survey paper:

> **[A Comprehensive Survey on Multimodal RAG: All Combinations of Modalities as Input and Output](https://doi.org/10.36227/techrxiv.176046306.66521015/v1)** 
>
> [Rui Zhang](https://www.ruizhang.info/)<sup>1</sup>, [Chen Liu](https://sdnylc.github.io/)<sup>1</sup>, [Yixin Su](https://ethanmock.github.io/yixinsu.github.io/)<sup>1</sup>, [Ruixuan Li](https://idc.hust.edu.cn/rxli/index.htm)<sup>1</sup>, [Xuanjing Huang](https://xuanjing-huang.github.io/)<sup>2</sup>, [Xuelong Li](http://xuelongli.cn/en.php)<sup>3</sup>, Philip S. Yu<sup>4</sup> 
>
> <sup>1</sup>Huazhong University of Science and Technology, <sup>2</sup>Fudan University, <sup>3</sup>Institute of Artificial Intelligence (TeleAI) of China Telecom, <sup>4</sup>University of Illinois at Chicago 


📚 In this paper, we conduct a comprehensive survey of the most recent work on **Multimodal RAG (MM-RAG)** in the sense that it has a full coverage of almost all the combinations of modalities as input and output, whereas existing survey papers typically focus on one or two modalities. Based on different input-output modality combinations, we present a **taxonomy** of MM-RAG methods which gives us a much clearer picture of their key technical components.

⚙️ Facilitated by such a taxonomy, we identify **four essential stages** of the workflow of MM-RAG, summarize common approaches to each stage, and discuss **optimization strategies** for each modality.

🌐 To provide a **holistic understanding** and practical guidance for building MM-RAG systems, we also discuss **training strategies** and **evaluation methods** of MM-RAG. Finally, we discuss various **MM-RAG applications** and **future directions**.

---

<a name="readme-index"></a>

## Quick Index

- [Taxonomy](#Taxonomy) (from a perspective of different input-output modality combinations)


- [Workflow](#Workflow) (including Pre-Retrieval, Retrieval, Augmentation, Generation)

- [Training Strategy](#Training-strategy) (including Parameter-Frozen Strategy, Parameter-Trainable Strategy)

- [Evaluation and Benchmarks](#Evaluation-and-Benchmarks) (including Evaluaton Metrics and Benchmarks)


---

## Taxonomy

<p align="center">
<img src="assets/taxonomy.png" width = "80%" alt="" align=center />
</p>

### Image→Text

| Paper                                                        | Task             | Code                                                         |
| ------------------------------------------------------------ | ---------------- | ------------------------------------------------------------ |
| [![Publish](https://img.shields.io/badge/Conference-EMNLP_2023-blue)]()<br/>Re-vilm: Retrievalaugmented visual language model for  zero and few-shot image captioning [[paper]](https://arxiv.org/abs/2302.04858) | Image Captioning |                                                              |
| Cross-modal retrieval and semantic refinement for  remote sensing image captioning [[paper]](https://www.mdpi.com/2072-4292/16/1/196) | Image Captioning |                                                              |
| [![Publish](https://img.shields.io/badge/Conference-CVPR_2023-blue)]()<br/>Smallcap: lightweight image captioning prompted with  retrieval augmentation [[paper]](https://arxiv.org/abs/2209.15323) | Image Captioning | ![](https://img.shields.io/github/stars/RitaRamo/smallcap)<br/>[[Code]](https://github.com/RitaRamo/smallcap) |
| [![Publish](https://img.shields.io/badge/Conference-ICML_2023-blue)]()<br/>Retrieval-augmented multimodal language modeling [[paper]](https://arxiv.org/abs/2211.12561) | Image Captioning |                                                              |
| [![Publish](https://img.shields.io/badge/Conference-CBMI_2022-blue)]()<br/>Retrieval-augmented transformer for image captioning [[paper]](https://arxiv.org/abs/2207.13162) | Image Captioning |                                                              |
| [![Publish](https://img.shields.io/badge/Conference-AAAI_2021-blue)]()<br/>Memory-augmented image captioning [[paper]](https://arxiv.org/abs/2403.03715) | Image Captioning |                                                              |
| [![Publish](https://img.shields.io/badge/Conference-EACL_2023-blue)]()<br/>Retrieval-augmented image captioning [[paper]](https://arxiv.org/abs/2302.08268) | Image Captioning |                                                              |
| [![Publish](https://img.shields.io/badge/Conference-COLING_2022-blue)]()<br/>Deltanet: Conditional medical report generation for  COVID-19 diagnosis [[paper]](https://aclanthology.org/2022.coling-1.261/) | Image Captioning |                                                              |
| Retrieval-enhanced adversarial training with dynamic  memory-augmented attention for image paragraph captioning [[paper]](https://www.sciencedirect.com/science/article/abs/pii/S0950705120308595) | Image Captioning | ![](https://img.shields.io/github/stars/anonymous-caption/RAMP)<br/>[[Code]](https://github.com/anonymous-caption/RAMP) |
| [![Publish](https://img.shields.io/badge/Conference-NAACL_2025-blue)]()<br/>Fact-aware multimodal retrieval augmentation for  accurate medical radiology report generation [[paper]](https://arxiv.org/abs/2407.15268) | Image Captioning | ![](https://img.shields.io/github/stars/cxcscmu/FactMM-RAG)<br/>[[Code]](https://github.com/cxcscmu/FactMM-RAG) |
| [![Publish](https://img.shields.io/badge/Conference-EMNLP_2021-blue)]()<br/>Retrieval, analogy, and composition: A framework for  compositional generalization in image captioning [[paper]](https://aclanthology.org/2021.findings-emnlp.171/) | Image Captioning |                                                              |

<p align="right" style="font-size: 14px; color: #555; margin-top: 20px;">
    <a href="#readme-index" style="text-decoration: none; color: #007bff; font-weight: bold;">
        ↑ Back to Index ↑
    </a>
</p>

### Text→Image

| Paper                                                        | Task             | Code                                                         |
| ------------------------------------------------------------ | ---------------- | ------------------------------------------------------------ |
| [![Publish](https://img.shields.io/badge/Conference-ECCV_2020-blue)]()<br/>RetrieveGAN:   Image Synthesis via Differentiable Patch Retrieval  [[paper]](https://arxiv.org/abs/2007.08513) | Image Generation |                                                              |
| [![Publish](https://img.shields.io/badge/Conference-COLING_2025-blue)]()<br/>FineRAG:   Fine-grained Retrieval-Augmented Text-to-Image Generation [[paper]](https://aclanthology.org/2025.coling-main.741.pdf) | Image Generation |                                                              |
| ImageRAG:   Dynamic Image Retrieval for Reference-Guided Image Generation [[paper]](https://arxiv.org/abs/2502.09411) | Image Generation | ![](https://img.shields.io/github/stars/rotem-shalev/ImageRAG)<br/>[[Code]](https://github.com/rotem-shalev/ImageRAG) |
| X&Fuse:   Fusing Visual Information in Text-to-Image Generation [[paper]](https://arxiv.org/abs/2303.01000) | Image Generation |                                                              |
| [![Publish](https://img.shields.io/badge/Conference-ICLR_2025-blue)]()<br/>TIGeR:   Unifying Text-to-Image Generation and Retrieval with Large Multimodal Models  [[paper]](https://arxiv.org/abs/2406.05814) | Image Generation | ![](https://img.shields.io/github/stars/LgQu/TIGeR)<br/>[[Code]](https://github.com/LgQu/TIGeR) |
| [![Publish](https://img.shields.io/badge/Conference-ICLR_2023-blue)]()<br/>Re-Imagen:   Retrieval-Augmented Text-to-Image Generator  [[paper]](https://arxiv.org/abs/2209.14491) | Image Generation |                                                              |
| [![Publish](https://img.shields.io/badge/Conference-NIPS_2022-blue)]()<br/>Retrieval-augmented   diffusion models [[paper]](https://proceedings.neurips.cc/paper_files/paper/2022/file/62868cc2fc1eb5cdf321d05b4b88510c-Paper-Conference.pdf) | Image Generation | ![](https://img.shields.io/github/stars/CompVis/retrieval-augmented-diffusion-models)<br/>[[Code]](https://github.com/CompVis/retrieval-augmented-diffusion-models) |
| [![Publish](https://img.shields.io/badge/Conference-ICLR_2023-blue)]()<br/>KNN-Diffusion:   Image Generation via Large-Scale Retrieval [[paper]](https://arxiv.org/abs/2204.02849) | Image Generation |                                                              |
| [![Publish](https://img.shields.io/badge/Conference-BMVC_2022-blue)]()<br/>Memory-Driven Text-to-Image Generation [[paper]](https://arxiv.org/abs/2208.07022) | Image Generation |                                                              |

<p align="right" style="font-size: 14px; color: #555; margin-top: 20px;">
    <a href="#readme-index" style="text-decoration: none; color: #007bff; font-weight: bold;">
        ↑ Back to Index ↑
    </a>
</p>

### Text+Image→Text

| Paper                                                        | Task          | Code                                                         |
| ------------------------------------------------------------ | ------------- | ------------------------------------------------------------ |
| [![Publish](https://img.shields.io/badge/Journal-TACL-blue)]()<br/>Augmenting Transformers with KNN-Based Composite  Memory for Dialog [[paper]](https://arxiv.org/abs/2004.12744) | Visual Dialog |                                                              |
| [![Publish](https://img.shields.io/badge/Conference-ACL_2021-blue)]()<br/>Maria: A Visual Experience Powered Conversational  Agent [[paper]](https://arxiv.org/abs/2105.13073) | Visual Dialog | ![](https://img.shields.io/github/stars/jokieleung/Maria)<br/>[[Code]](https://github.com/jokieleung/Maria) |
| [![Publish](https://img.shields.io/badge/Conference-EMNLP_2022-blue)]()<br/>Murag: Multimodal retrieval-augmented generator for  open question answering over images and text [[paper]](https://arxiv.org/abs/2210.02928) | Visual QA     |                                                              |
| [![Publish](https://img.shields.io/badge/Conference-EMNLP_2022-blue)]()<br/>Retrieval Augmented Visual Question Answering with  Outside Knowledge [[paper]](https://arxiv.org/abs/2210.03809) | Visual QA     | ![](https://img.shields.io/github/stars/LinWeizheDragon/Retrieval-Augmented-Visual-Question-Answering)<br/>[[Code]](https://github.com/LinWeizheDragon/Retrieval-Augmented-Visual-Question-Answering) |
| [![Publish](https://img.shields.io/badge/Conference-ACM MM_2023-blue)]()<br/>RAMM: Retrieval-augmented Biomedical Visual Question  Answering with Multi-modal Pre-training [[paper]](https://arxiv.org/abs/2303.00534) | Visual QA     | [![](https://img.shields.io/github/stars/GanjinZero/RAMM)<br/>[Code]](http://github.com/GanjinZero/RAMM) |
| [![Publish](https://img.shields.io/badge/Conference-NAACL_2022-blue)]()<br/>KAT: A Knowledge Augmented Transformer for  Vision-and-Language [[paper]](https://arxiv.org/abs/2112.08614) | Visual QA     | ![](https://img.shields.io/github/stars/guilk/KAT)<br/>[[Code]](https://github.com/guilk/KAT) |
| [![Publish](https://img.shields.io/badge/Conference-AAAI_2022-blue)]()<br/>An empirical study of gpt-3 for few-shot  knowledge-based vqa [[paper]](https://arxiv.org/abs/2109.05014) | Visual QA     | ![](https://img.shields.io/github/stars/microsoft/PICa)<br/>[[Code]](https://github.com/microsoft/PICa) |
| [![Publish](https://img.shields.io/badge/Conference-EMNLP_2021-blue)]()<br/>Cross-modal retrieval augmentation for multi-modal  classification [[paper]](https://arxiv.org/abs/2104.08108) | Visual QA     |                                                              |
| Mllm is a strong reranker: Advancing multimodal  retrieval-augmented generation via knowledge-enhanced reranking and  noise-injected training [[paper]](https://arxiv.org/abs/2407.21439) | Visual QA     | [![](https://img.shields.io/github/stars/DataArcTech/RagVL)<br/>[Code]](https://github.com/DataArcTech/RagVL) |
| Learning to compress contexts for efficient  knowledge-based visual question answering [[paper]](https://arxiv.org/abs/2409.07331) | Visual QA     |                                                              |
| [![Publish](https://img.shields.io/badge/Conference-CVPR_2023-blue)]()<br/>Reveal: Retrievalaugmented visual-language  pre-training with multi-source multimodal knowledge memory [[paper]](https://arxiv.org/abs/2212.05221) | Visual QA     | [[Code]](https://github.com/google-research/scenic/tree/main/scenic/projects/knowledge_visual_language) |
| [![Publish](https://img.shields.io/badge/Conference-ACL_2025-blue)]()<br/> Visa: Retrieval augmented generation with visual  source attribution [[paper]](https://arxiv.org/abs/2412.14457) | Visual QA     | ![](https://img.shields.io/github/stars/castorini/visa)<br/>[[Code]](https://github.com/castorini/visa) |
| M3DOCRAG: Multi-modal Multi-page Document RAG System [[paper]](https://arxiv.org/abs/2411.04952) | Visual QA     | ![](https://img.shields.io/github/stars/bloomberg/m3docrag)<br/>[[Code]](https://github.com/bloomberg/m3docrag) |
| [![Publish](https://img.shields.io/badge/Conference-EMNLP_2024-blue)]()<br/>Echosight: Advancing visual-language models with wiki  knowledge [[paper]](https://arxiv.org/abs/2407.12735) | Visual QA     | ![](https://img.shields.io/github/stars/Go2Heart/EchoSight)<br/>[[Code]](https://github.com/Go2Heart/EchoSight) |
| Visrag: Vision-based retrieval-augmented generation on  multi-modality documents [[paper]](https://arxiv.org/abs/2410.10594) | Visual QA     | ![](https://img.shields.io/github/stars/OpenBMB/VisRAG)<br/>[[Code]](https://github.com/OpenBMB/VisRAG) |
| [![Publish](https://img.shields.io/badge/Conference-NIPS_2023-blue)]()<br/>Fine-grained late-interaction multi-modal retrieval  for retrieval augmented visual question answering [[paper]](https://arxiv.org/abs/2309.17133) | Visual QA     | ![](https://img.shields.io/github/stars/LinWeizheDragon/Retrieval-Augmented-Visual-Question-Answering)<br/>[[Code]](https://github.com/LinWeizheDragon/Retrieval-Augmented-Visual-Question-Answering) |
| [![Publish](https://img.shields.io/badge/Conference-ICLR_2025-blue)]()<br/>MMed-RAG: Versatile Multimodal RAG System for Medical  Vision Language Models [[paper]](https://arxiv.org/abs/2410.13085) | Visual QA     | ![](https://img.shields.io/github/stars/richard-peng-xia/MMed-RAG)<br/>[[Code]](https://github.com/richard-peng-xia/MMed-RAG) |

<p align="right" style="font-size: 14px; color: #555; margin-top: 20px;">
    <a href="#readme-index" style="text-decoration: none; color: #007bff; font-weight: bold;">
        ↑ Back to Index ↑
    </a>
</p>

### Audio→Text

| Paper                                                        | Task             | Code                                                         |
| ------------------------------------------------------------ | ---------------- | ------------------------------------------------------------ |
| [![Publish](https://img.shields.io/badge/Conference-ICASSP_2024-blue)]()<br/>RECAP:   Retrieval-Augmented Audio Captioning [[paper]](https://arxiv.org/abs/2309.09836) | Audio Captioning | ![](https://img.shields.io/github/stars/Sreyan88/RECAP)<br/>[[Code]](https://github.com/Sreyan88/RECAP) |
| [![Publish](https://img.shields.io/badge/Conference-ICASSP_2021-blue)]()<br/>Audio   Captioning using Pre-Trained Large-Scale Language Model Guided by Audio-based   Similar Caption Retrieval [[paper]](https://arxiv.org/abs/2012.07331) | Audio Captioning |                                                              |

<p align="right" style="font-size: 14px; color: #555; margin-top: 20px;">
    <a href="#readme-index" style="text-decoration: none; color: #007bff; font-weight: bold;">
        ↑ Back to Index ↑
    </a>
</p>

### Text→Audio

| Paper                                                        | Task             | Code                                                         |
| ------------------------------------------------------------ | ---------------- | ------------------------------------------------------------ |
| [![Publish](https://img.shields.io/badge/Conference-ICML_2023-blue)]()<br/>Make-An-Audio:   Text-To-Audio Generation with Prompt-Enhanced Diffusion Models [[paper]](https://arxiv.org/abs/2301.12661) | Audio Generation | ![](https://img.shields.io/github/stars/Text-to-Audio/Make-An-Audio)<br/>[[Code]](https://github.com/Text-to-Audio/Make-An-Audio) |
| [![Publish](https://img.shields.io/badge/Conference-ICASSP_2024-blue)]()<br/>Retrieval-Augmented   Text-to-Audio Generation [[paper]](https://arxiv.org/abs/2309.08051) | Audio Generation |                                                              |
| [![Publish](https://img.shields.io/badge/Conference-Interspeech_2025-blue)]()<br/>Audiobox   TTA-RAG: Improving Zero-Shot and Few-Shot Text-To-Audio with   Retrieval-Augmented Generation [[paper]](https://arxiv.org/abs/2411.05141) | Audio Generation | [[Code]](https://tta-rag-is25.github.io/)                    |
| [![Publish](https://img.shields.io/badge/Conference-Interspeech_2024-blue)]()<br/>Retrieval   augmented generation in prompt-based text-to-speech synthesis with   context-aware contrastive language-audio pretraining [[paper]](https://arxiv.org/abs/2406.03714) | Audio Generation | [[Code]](https://happylittlecat2333.github.io/interspeech2024-RAG/) |
| [![Publish](https://img.shields.io/badge/Conference-Interspeech_2024-blue)]()<br/>Retrieval-augmented classifier guidance for audio generation | Audio Generation |                                                              |

<p align="right" style="font-size: 14px; color: #555; margin-top: 20px;">
    <a href="#readme-index" style="text-decoration: none; color: #007bff; font-weight: bold;">
        ↑ Back to Index ↑
    </a>
</p>

### Video→Text

| Paper                                                        | Task             | Code                                                         |
| ------------------------------------------------------------ | ---------------- | ------------------------------------------------------------ |
| [![Publish](https://img.shields.io/badge/Conference-CVPR_2024-blue)]()<br/>Retrieval-augmented   egocentric video captioning [[paper]](https://arxiv.org/abs/2401.00789) | Video Captioning | [![](https://img.shields.io/github/stars/Jazzcharles/Egoinstructor)<br/>[Code]](https://github.com/Jazzcharles/Egoinstructor/) |
| [![Publish](https://img.shields.io/badge/Conference-EMNLP_2018-blue)]()<br/>Incorporating   background knowledge into video description generation [[paper]](https://aclanthology.org/D18-1433/) | Video Captioning |                                                              |

<p align="right" style="font-size: 14px; color: #555; margin-top: 20px;">
    <a href="#readme-index" style="text-decoration: none; color: #007bff; font-weight: bold;">
        ↑ Back to Index ↑
    </a>
</p>

### Text→Video

| Paper                                                        | Task             | Code                                                         |
| ------------------------------------------------------------ | ---------------- | ------------------------------------------------------------ |
| [![Publish](https://img.shields.io/badge/Conference-ECCV_2024-blue)]()<br/>Animate-A-Story:   Storytelling with Retrieval-Augmented Video Generation [[paper]](https://arxiv.org/abs/2307.06940) | Video Generation | ![](https://img.shields.io/github/stars/AILab-CVC/Animate-A-Story)<br/>[[Code]](https://github.com/AILab-CVC/Animate-A-Story) |

<p align="right" style="font-size: 14px; color: #555; margin-top: 20px;">
    <a href="#readme-index" style="text-decoration: none; color: #007bff; font-weight: bold;">
        ↑ Back to Index ↑
    </a>
</p>

### Image→Video

| Paper                                                        | Task                      | Code                                                         |
| ------------------------------------------------------------ | ------------------------- | ------------------------------------------------------------ |
| [![Publish](https://img.shields.io/badge/Conference-NIPS_2025-blue)]()<br/>MotionRAG:   Motion Retrieval-Augmented Image-to-Video Generation [[paper]](https://arxiv.org/abs/2509.26391) | Image-to-Video Generation | ![](https://img.shields.io/github/stars/MCG-NJU/MotionRAG)<br/>[[Code]](https://github.com/MCG-NJU/MotionRAG) |

<p align="right" style="font-size: 14px; color: #555; margin-top: 20px;">
    <a href="#readme-index" style="text-decoration: none; color: #007bff; font-weight: bold;">
        ↑ Back to Index ↑
    </a>
</p>

### Video+Text→Text

| Paper                                                        | Task     | Code                                                         |
| ------------------------------------------------------------ | -------- | ------------------------------------------------------------ |
| [![Publish](https://img.shields.io/badge/Conference-CVPRW_2024-blue)]()<br/>ViTA:   An Efficient Video-to-Text Algorithm using VLM for RAG-based Video Analysis   System [[paper]](https://openaccess.thecvf.com/content/CVPR2024W/MAR/papers/Arefeen_ViTA_An_Efficient_Video-to-Text_Algorithm__using_VLM_for_RAG-based_CVPRW_2024_paper.pdf) | Video QA |                                                              |
| [![Publish](https://img.shields.io/badge/Conference-CVPR_2023-blue)]()<br/>Retrieving-to-Answer:   Zero-Shot Video Question Answering with Frozen Large Language Models [[paper]](https://arxiv.org/abs/2306.11732) | Video QA |                                                              |
| [![Publish](https://img.shields.io/badge/Conference-CIKM_2024-blue)]()<br/>iRAG:   Advancing RAG for Videos with an Incremental Approach [[paper]](https://arxiv.org/abs/2404.12309) | Video QA |                                                              |
| [![Publish](https://img.shields.io/badge/Conference-TOMCCAP_2023-blue)]()<br/>Retrieval   augmented convolutional encoder-decoder networks for video captioning [[paper]](https://dl.acm.org/doi/10.1145/3539225) | Video QA |                                                              |
| [![Publish](https://img.shields.io/badge/Conference-ACL_2025-blue)]()<br/>VideoRAG:   Retrieval-Augmented Generation over Video Corpus [[paper]](https://arxiv.org/abs/2501.05874) | Video QA | ![](https://img.shields.io/github/stars/starsuzi/VideoRAG)<br/>[[Code]](https://github.com/starsuzi/VideoRAG) |
| [![Publish](https://img.shields.io/badge/Conference-NIPS_2025-blue)]()<br/>Video-RAG:   Visually-aligned Retrieval-Augmented Long Video Comprehension [[paper]](https://arxiv.org/abs/2411.13093) | Video QA | ![](https://img.shields.io/github/stars/Leon1207/Video-RAG-master)<br/>[[Code]](http://github.com/Leon1207/Video-RAG-master) |
| VideoRAG:   Retrieval-Augmented Generation with Extreme Long-Context Videos [[paper]](https://arxiv.org/abs/2502.01549) | Video QA | ![](https://img.shields.io/github/stars/HKUDS/VideoRAG)<br/>[[Code]](https://github.com/HKUDS/VideoRAG) |

<p align="right" style="font-size: 14px; color: #555; margin-top: 20px;">
    <a href="#readme-index" style="text-decoration: none; color: #007bff; font-weight: bold;">
        ↑ Back to Index ↑
    </a>
</p>

### Text→3D

| Paper                                                        | Task       | Code                                                         |
| ------------------------------------------------------------ | ---------- | ------------------------------------------------------------ |
| [![Publish](https://img.shields.io/badge/Conference-ICCV_2023-blue)]()<br/>ReMoDiffuse:   Retrieval-Augmented Motion Diffusion Model [[paper]](https://arxiv.org/abs/2304.01116) | Text-to-3D | ![](https://img.shields.io/github/stars/mingyuan-zhang/ReMoDiffuse)<br/>[[Code]](https://github.com/mingyuan-zhang/ReMoDiffuse) |
| [![Publish](https://img.shields.io/badge/Conference-ICML_2024-blue)]()<br/>Retrieval-Augmented   Score Distillation for Text-to-3D Generation [[paper]](http://arxiv.org/abs/2402.02972) | Text-to-3D | ![](https://img.shields.io/github/stars/cvlab-kaist/ReDream)<br/>[[Code]](https://github.com/cvlab-kaist/ReDream) |

<p align="right" style="font-size: 14px; color: #555; margin-top: 20px;">
    <a href="#readme-index" style="text-decoration: none; color: #007bff; font-weight: bold;">
        ↑ Back to Index ↑
    </a>
</p>

### Code→Text

| Paper                                                        | Task                              | Code                                                         |
| ------------------------------------------------------------ | --------------------------------- | ------------------------------------------------------------ |
| [![Publish](https://img.shields.io/badge/Conference-ICSE_2020-blue)]()<br/>Retrieval-based neural source code summarization [[paper]](https://dl.acm.org/doi/10.1145/3377811.3380383) | Code Summarization                | [![](https://img.shields.io/github/stars/zhangj111/rencos)<br/>[Code]](https://github.com/zhangj111/rencos) |
| [![Publish](https://img.shields.io/badge/Conference-EMNLP_2021-blue)]()<br/>Retrieval   augmented code generation and summarization [[paper]](https://arxiv.org/abs/2108.11601) | Code Generation and Summarization | ![](https://img.shields.io/github/stars/rizwan09/REDCODER)<br/>[[Code]](https://github.com/rizwan09/REDCODER) |
| [![Publish](https://img.shields.io/badge/Conference-ICLR_2021-blue)]()<br/>Retrieval-Augmented   Generation for Code Summarization via Hybrid GNN [[paper]](https://arxiv.org/abs/2006.05405) | Code Summarization                | [![](https://img.shields.io/github/stars/shangqing-liu/CCSD-benchmark-for-code-summarization)<br/>[Code]](https://github.com/shangqing-liu/CCSD-benchmark-for-code-summarization) |
| [![Publish](https://img.shields.io/badge/Conference-EMNLP_2022-blue)]()<br/>RACE:   Retrieval-Augmented Commit Message Generation [[paper]](https://arxiv.org/abs/2203.02700) | Commit Message Generation         | [![](https://img.shields.io/github/stars/DeepSoftwareAnalytics/RACE)<br/>[Code]](http://github.com/DeepSoftwareAnalytics/RACE) |

<p align="right" style="font-size: 14px; color: #555; margin-top: 20px;">
    <a href="#readme-index" style="text-decoration: none; color: #007bff; font-weight: bold;">
        ↑ Back to Index ↑
    </a>
</p>

### Text→Code

| Paper                                                        | Task                              | Code                                                         |
| ------------------------------------------------------------ | --------------------------------- | ------------------------------------------------------------ |
| [![Publish](https://img.shields.io/badge/Conference-ICSE_2023-blue)]()<br/>Retrieval-Based Prompt Selection for Code-Related Few-Shot Learning [[paper]](https://dl.acm.org/doi/10.1109/icse48619.2023.00205) | Code Generation                   | ![](https://img.shields.io/github/stars/prompt-learning/cedar)<br/>[[Code]](https://github.com/prompt-learning/cedar) |
| [![Publish](https://img.shields.io/badge/Conference-EMNLP_2023-blue)]()<br/>RepoCoder:   Repository-Level Code Completion Through Iterative Retrieval and Generation [[paper]](https://arxiv.org/abs/2303.12570) | Code Completion                   | [[Code]](https://github.com/microsoft/CodeT/tree/main/RepoCoder) |
| [![Publish](https://img.shields.io/badge/Conference-EMNLP_2021-blue)]()<br/>Retrieval augmented code generation and summarization [[paper]](https://arxiv.org/abs/2108.11601) | Code Generation and Summarization | ![](https://img.shields.io/github/stars/rizwan09/REDCODER)<br/>[[Code]](https://github.com/rizwan09/REDCODER) |
| CoCoMIC:   Code Completion By Jointly Modeling In-file and Cross-file Context [[paper]](https://arxiv.org/abs/2212.10007) | Code Generation                   | ![](https://img.shields.io/github/stars/amazon-science/cocomic)<br/>[[Code]](https://github.com/amazon-science/cocomic) |
| [![Publish](https://img.shields.io/badge/Conference-EMNLP_2024-blue)]()<br/>EVOR:   Evolving Retrieval for Code Generation [[paper]](https://arxiv.org/abs/2402.12317) | Code Generation                   | [[Code]](https://arks-codegen.github.io/)                    |
| [![Publish](https://img.shields.io/badge/Conference-ICLR_2022-blue)]()<br/>Synchromesh:   Reliable code generation from pre-trained language models [[paper]](https://arxiv.org/abs/2201.11227) | Code Generation                   | ![](https://img.shields.io/github/stars/kanishkg/synchromesh)<br/>[[Code]](https://github.com/kanishkg/synchromesh) |
| [![Publish](https://img.shields.io/badge/Conference-NIPS_2018-blue)]()<br/>A Retrieve-and-Edit Framework for Predicting Structured Outputs [[paper]](https://arxiv.org/abs/1812.01194) | Code Generation                   |                                                              |
| [![Publish](https://img.shields.io/badge/Conference-ACL_2022-blue)]()<br/>ReACC: A Retrieval-Augmented Code Completion Framework [[paper]](https://arxiv.org/abs/2203.07722) | Code Completion                   | [![](https://img.shields.io/github/stars/microsoft/ReACC)<br/>[Code]](https://github.com/microsoft/ReACC) |
| [![Publish](https://img.shields.io/badge/Conference-ICLR_2023-blue)]()<br/>DocPrompting:   Generating Code by Retrieving the Docs [[paper]](https://arxiv.org/abs/2207.05987) | Code Generation                   | [![](https://img.shields.io/github/stars/shuyanzhou/docprompting)<br/>[Code]](https://github.com/shuyanzhou/docprompting) |
| [![Publish](https://img.shields.io/badge/Conference-EMNLP_2022-blue)]()<br/>XRICL:   Cross-lingual Retrieval-Augmented In-Context Learning for Cross-lingual Text-to-SQL Semantic Parsing [[paper]](https://arxiv.org/abs/2210.13693) | Text-to-SQL                       |                                                              |

<p align="right" style="font-size: 14px; color: #555; margin-top: 20px;">
    <a href="#readme-index" style="text-decoration: none; color: #007bff; font-weight: bold;">
        ↑ Back to Index ↑
    </a>
</p>

### Text+Structured Data→Text

| Paper                                                        | Task     | Code                                                         |
| ------------------------------------------------------------ | -------- | ------------------------------------------------------------ |
| KnowledGPT:  Enhancing Large Language Models with Retrieval and Storage Access on Knowledge Bases [[paper]](https://arxiv.org/abs/2308.11761) | KBQA     |                                                              |
| [![Publish](https://img.shields.io/badge/Conference-NIPS_2024-blue)]()<br/>G-Retriever:   Retrieval-Augmented Generation for Textual Graph Understanding and Question   Answering [[paper]](https://arxiv.org/abs/2402.07630) | KBQA     | [![](https://img.shields.io/github/stars/XiaoxinHe/G-Retriever)<br/>[Code]](https://github.com/XiaoxinHe/G-Retriever) |
| [![Publish](https://img.shields.io/badge/Conference-ACL_2021-blue)]()<br/>ReTraCk:   A Flexible and Efficient Framework for Knowledge Base Question Answering[[paper]](https://aclanthology.org/2021.acl-demo.39.pdf) | KBQA     | [[Code]](https://github.com/microsoft/KC/tree/main/papers/ReTraCk) |
| [![Publish](https://img.shields.io/badge/Conference-WWW_2025-blue)]()<br/>KAG:   Boosting LLMs in Professional Domains via Knowledge Augmented Generation [[paper]](https://arxiv.org/abs/2409.13731) | KBQA     | ![](https://img.shields.io/github/stars/OpenSPG/KAG)<br/>[[Code]](https://github.com/OpenSPG/KAG) |
| [![Publish](https://img.shields.io/badge/Conference-ACL_2023-blue)]()<br/>LI-RAGE: Late   Interaction Retrieval Augmented Generation with Explicit Signals for   Open-Domain Table Question Answering [[paper]](https://aclanthology.org/2023.acl-short.133.pdf) | Table QA | ![](https://img.shields.io/github/stars/amazon-science/robust-tableqa)<br/>[[Code]](https://github.com/amazon-science/robust-tableqa) |
| End-to-End Table Question Answering via Retrieval-Augmented Generation [[paper]](https://arxiv.org/abs/2203.16714) | Table QA |                                                              |
| RAG over Tables: Hierarchical Memory Index, Multi-Stage Retrieval, and Benchmarking [[paper]](https://arxiv.org/abs/2504.01346) | Table QA | ![](https://img.shields.io/github/stars/jiaruzouu/T-RAG)<br/>[[Code]](https://github.com/jiaruzouu/T-RAG) |
| [![Publish](https://img.shields.io/badge/Conference-ACL_2021-blue)]()<br/>Dual Reader-Parser on Hybrid Textual and Tabular Evidence for Open Domain Question Answering [[paper]](https://arxiv.org/abs/2108.02866) | Table QA | [![](https://img.shields.io/github/stars/awslabs/durepa-hybrid-qa)<br/>[Code]](https://github.com/awslabs/durepa-hybrid-qa) |

<p align="right" style="font-size: 14px; color: #555; margin-top: 20px;">
    <a href="#readme-index" style="text-decoration: none; color: #007bff; font-weight: bold;">
        ↑ Back to Index ↑
    </a>
</p>

## Workflow

For a functional MM-RAG system, we identify four essential stages of its workflow:  ***pre-retrieval, retrieval, augmentation and generation*** . Retrieval and generation involve the retriever and generator, respectively. Pre-retrieval involves knowledge base and query preparation. Augmentation involves the preprocessing of the query and retrieved documents before they are fed into the generator. For each stage, we discuss common approaches and modality-specific optimization strategies, and summarize representative studies.

<p align="center">
<img src="assets/workflow.png" width = "80%" alt="" align=center />
</p>

<p align="center">
<img src="assets/workflow-tree.png" width = "80%" alt="" align=center />
</p>

## Training Strategy

There are mainly two strategies: parameter-frozen strategies and parameter-trainable strategies. We summarize training methods and commonly used training datasets 4 per input-output modality combination in the following Tables.

<p align="center">
<img src="assets/training.png" width = "80%" alt="" align=center />
</p>

<p align="center">
<img src="assets/datasets.png" width = "80%" alt="" align=center />
</p>

## Evaluation and Benchmarks

We discussed the evaluation metrics and benchmarks of the retriever and the generator as they are the two core components that affect the performance of MM-RAG.

<p align="center">
<img src="assets/evaluation.png" width = "80%" alt="" align=center />
</p>

| Modality                    | Benchmark                                                    | Evaluation Targets                                           |
| --------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| Text + Image → Text         | [![Publish](https://img.shields.io/badge/Conference-CVPR_2022-blue)]()<br/>WebQA [[Paper]](https://arxiv.org/abs/2109.00590) [[Resource]](https://webqna.github.io/) | Textual knowledge retrieval and reasoning.                   |
|                             | [![Publish](https://img.shields.io/badge/Conference-CVPR_2019-blue)]()<br/>OK-VQA [[Paper]](https://arxiv.org/abs/1906.00067)  [[Resource]](https://okvqa.allenai.org/) |                                                              |
|                             | [![Publish](https://img.shields.io/badge/Conference-ECCV_2022-blue)]()<br/>A-OKVQA [[Paper]](https://arxiv.org/abs/2206.01718) [[Resource]](https://github.com/allenai/aokvqa) |                                                              |
|                             | [![Publish](https://img.shields.io/badge/Conference-ICLR_2025-blue)]()<br/>MRAG-BENCH  [[Paper]](https://arxiv.org/abs/2410.08182) [[Resource]](https://mragbench.github.io/) | Visual knowledge retrieval and reasoning.                    |
|                             | Visual-RAG [[Paper]](https://arxiv.org/abs/2502.16636) [[Resource]](https://github.com/visual-rag/visual-rag) |                                                              |
|                             | $M^2$RAG [[Paper]](https://arxiv.org/abs/2411.16365) [[Resource]](https://github.com/maziao/M2RAG) | Document retrieval and generation with interleaved text-image content. |
|                             | [![Publish](https://img.shields.io/badge/Conference-SIGIR_2025-blue)]()<br/>MRAMG-Bench  [[Paper]](https://arxiv.org/abs/2502.04176) [[Resource]](https://github.com/MRAMG-Bench/MRAMG) |                                                              |
|                             | Dyn-VQA [[Paper]](https://arxiv.org/abs/2411.02937) [[Resource]](https://github.com/Alibaba-NLP/OmniSearch) | Ability of adapting to rapidly changing multimodal knowledge; multi-hop and multimodal reasoning. |
|                             | [![Publish](https://img.shields.io/badge/Conference-SIGIR_2025-blue)]()<br/>CogBench [[Paper]](https://arxiv.org/abs/2501.15470) | Adaptive information acquisition by recording the entire planning procedure. |
|                             | Liu et al. [[Paper]](https://arxiv.org/abs/2502.17297)  [[Resource]](https://github.com/NEUIR/M2RAG) | Evaluates MM-RAG across four tasks: image captioning, multimodal QA, fact verification, and image reranking. |
| Text + Table + Image → Text | [![Publish](https://img.shields.io/badge/Conference-EMNLP_2024-blue)]()<br/>OMG-QA [[Paper]](https://aclanthology.org/2024.emnlp-industry.75/) | Retrieval and reasoning over complex document structures.    |
|                             | [![Publish](https://img.shields.io/badge/Conference-IJCAI_2024-blue)]()<br/>PDF-MVQA [[Paper] [[Resource]](https://github.com/adlnlp/mmvqa) |                                                              |
|                             | Real-MM-RAG [[Paper]](https://arxiv.org/abs/2502.12342)      |                                                              |
| Text → Text                 | [![Publish](https://img.shields.io/badge/Conference-EACL_2024-blue)]()<br/>RAGAS [[Paper]](https://arxiv.org/abs/2309.15217) [[Resource]](https://github.com/explodinggradients/ragas) | Context relevance, answer faithfulness, and answer relevance. |
|                             | [![Publish](https://img.shields.io/badge/Conference-NAACL_2024-blue)]()<br/>ARES [[Paper]](https://arxiv.org/abs/2311.09476) [[Resource]](https://github.com/stanford-futuredata/ARES) |                                                              |
|                             | [![Publish](https://img.shields.io/badge/Conference-AAAI_2024-blue)]()<br/>RGB [[Paper]](https://arxiv.org/abs/2309.01431) [[Resource]](https://github.com/chen700564/RGB) | Noise robustness, negative rejection, information integration, and counterfactual robustness |

<p align="right" style="font-size: 14px; color: #555; margin-top: 20px;">
    <a href="#readme-index" style="text-decoration: none; color: #007bff; font-weight: bold;">
        ↑ Back to Index ↑
    </a>
</p>

## Contributing and Citation

The survey and the repository are **still work in progress** and will be updated regularly. 

🙋 If you would like to include your paper in this survey and repository, please feel free to submit a pull request or open an issue with the paper's title and a brief summary highlighting its key techniques. You can also contact us via email. Please let us know if you find out a mistake or have any suggestions! We greatly appreciate your feedback regarding this repository or survey!

🌟 If you find this resource helpful for your work, please consider citing our research.
```
@article{Zhang_2025,
	title={A Comprehensive Survey on Multimodal RAG: All Combinations of Modalities as Input and Output},
	url={http://dx.doi.org/10.36227/techrxiv.176341513.38473003/v2},
	DOI={10.36227/techrxiv.176341513.38473003/v2},
	publisher={IEEE},
	author={Rui Zhang and Chen Liu and Yixin Su and Ruixuan Li and Xuanjing Huang and Xuelong Li and Philip S Yu},
	year={2025},
	month=nov
}
```

