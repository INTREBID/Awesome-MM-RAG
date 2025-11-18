<h1 align="center">Awesome Multimodal RAG</h1>

<div align='center'>
[![GitHub Stars](https://img.shields.io/github/stars/INTREBID/Awesome-MM-RAG?style=social)](https://github.com/INTREBID/Awesome-MM-RAG/stargazers)[![GitHub Watchers](https://img.shields.io/github/watchers/INTREBID/Awesome-MM-RAG?style=social)](https://github.com/INTREBID/Awesome-MM-RAG/watchers)[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.XXXXXXX.svg)](https://doi.org/10.5281/zenodo.XXXXXXX)
</div>

<div align="center">
[<a href="https://www.techrxiv.org/doi/10.36227/techrxiv.176046306.66521015">TechRxiv</a>]
</div>



This repository is for our survey paper:

> **[A Comprehensive Survey on Multimodal RAG: All Combinations of Modalities as Input and Output](https://doi.org/10.36227/techrxiv.176046306.66521015/v1)**  
> *[Rui Zhang](https://www.ruizhang.info/)<sup>1</sup>, [Chen Liu](https://sdnylc.github.io/)<sup>1</sup>, [Yixin Su](https://ethanmock.github.io/yixinsu.github.io/)<sup>1</sup>, [Ruixuan Li](https://idc.hust.edu.cn/rxli/index.htm)<sup>1</sup>, , [Xuanjing Huang](https://xuanjing-huang.github.io/)<sup>2</sup>, [Xuelong Li](http://xuelongli.cn/en.php)<sup>3</sup>, Philip S. Yu<sup>2</sup>, *  
> <sup>1</sup>Huazhong University of Science and Technology, <sup>2</sup>Fudan University, <sup>3</sup>Institute of Artificial Intelligence (TeleAI) of China Telecom, <sup>4</sup>University of Illinois at Chicago 


In this paper, we conduct a comprehensive survey of the most recent work on Multimodal RAG (MM-RAG) in the sense that it has a full coverage of almost all the combinations of modalities as input and output, whereas existing survey papers typically focus on one or two modalities. Based on different input-output modality combinations, we present a taxonomy of MM-RAG methods which gives us a much clearer picture of their key technical components.

Facilitated by such a taxonomy, we identify four essential stages of the workflow of MM-RAG, summarize common approaches to each stage, and discuss optimization strategies for each modality.

To provide a holistic understanding and practical guidance for building MM-RAG systems, we also discuss training strategies and evaluation methods of MM-RAG. Finally, we discuss various MM-RAG applications and future directions.

### Contributing

The survey and the repository are **still work in progress** and will be updated regularly. 

🙋 If you would like to include your paper in this survey and repository, please feel free to submit a pull request or open an issue with the paper's title and a brief summary highlighting its key techniques. You can also contact us via email. Please let us know if you find out a mistake or have any suggestions! We greatly appreciate your feedback regarding this repository or survey!

🌟 If you find this resource helpful for your work, please consider citing our [research](#citation).


---

<a name="readme-index"></a>

## Quick Index

- [Definition — What's MM-RAG](#definition)
<p align="center">
<img src="assets/definition.png" width = "80%" alt="" align=center />
</p>

- [Taxonomy — MM-RAG Methods](#taxonomy)

<p align="center">
<img src="assets/taxonomy.png" width = "80%" alt="" align=center />
</p>

- [Workflow — MM-RAG Stages](#workflow)
  - [Pre-Retrieval](#pre-retrieval)
  - [Retrieval](#retrieval)
  - [Augmentation](#augmentation)
  - [Generation](#generation)

<p align="center">
<img src="assets/workflow.png" width = "80%" alt="" align=center />
</p>
<p align="center">
<img src="assets/workflow-tree.png" width = "80%" alt="" align=center />
</p>

- [Training Strategy](#training-strategy)
<p align="center">
<img src="assets/training.png" width = "80%" alt="" align=center />
</p>

- [Evaluation](#evaluation)
<p align="center">
<img src="assets/evaluation.png" width = "80%" alt="" align=center />
</p>

---
