<h1 align="center">Awesome MM-RAG</h1>

<div align="center">

![](https://awesome.re/badge.svg?logo=stylelint)
![](https://img.shields.io/github/stars/INTREBID/Awesome-MM-RAG)
![](https://img.shields.io/github/watchers/INTREBID/Awesome-MM-RAG)
![](https://img.shields.io/github/last-commit/INTREBID/Awesome-MM-RAG?color=green)
![](https://img.shields.io/badge/PRs-Welcome-blue)
[![DOI](https://img.shields.io/badge/DOI-10.36227%2Ftechrxiv.176341513.38473003%2Fv1-yellow?logo=doi)](https://doi.org/10.36227/techrxiv.176341513.38473003/v1)

</div>

<div align="center">

**[<a href="https://doi.org/10.36227/techrxiv.176341513.38473003/v1">TechRxiv</a>]** 

</div>

This repository is for our survey paper:

> **[A Comprehensive Survey on Multimodal RAG: All Combinations of Modalities as Input and Output](https://doi.org/10.36227/techrxiv.176046306.66521015/v1)**  
> *[Rui Zhang](https://www.ruizhang.info/)<sup>1</sup>, [Chen Liu](https://sdnylc.github.io/)<sup>1</sup>, [Yixin Su](https://ethanmock.github.io/yixinsu.github.io/)<sup>1</sup>, [Ruixuan Li](https://idc.hust.edu.cn/rxli/index.htm)<sup>1</sup>, , [Xuanjing Huang](https://xuanjing-huang.github.io/)<sup>2</sup>, [Xuelong Li](http://xuelongli.cn/en.php)<sup>3</sup>, Philip S. Yu<sup>4</sup>, *  
> <sup>1</sup>Huazhong University of Science and Technology, <sup>2</sup>Fudan University, <sup>3</sup>Institute of Artificial Intelligence (TeleAI) of China Telecom, <sup>4</sup>University of Illinois at Chicago 


📚 In this paper, we conduct a comprehensive survey of the most recent work on **Multimodal RAG (MM-RAG)** in the sense that it has a full coverage of almost all the combinations of modalities as input and output, whereas existing survey papers typically focus on one or two modalities. Based on different input-output modality combinations, we present a **taxonomy** of MM-RAG methods which gives us a much clearer picture of their key technical components.

⚙️ Facilitated by such a taxonomy, we identify **four essential stages** of the workflow of MM-RAG, summarize common approaches to each stage, and discuss **optimization strategies** for each modality.

🌐 To provide a **holistic understanding** and practical guidance for building MM-RAG systems, we also discuss **training strategies** and **evaluation methods** of MM-RAG. Finally, we discuss various **MM-RAG applications** and **future directions**.



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

### Contributing

The survey and the repository are **still work in progress** and will be updated regularly. 

🙋 If you would like to include your paper in this survey and repository, please feel free to submit a pull request or open an issue with the paper's title and a brief summary highlighting its key techniques. You can also contact us via email. Please let us know if you find out a mistake or have any suggestions! We greatly appreciate your feedback regarding this repository or survey!

🌟 If you find this resource helpful for your work, please consider citing our research.
```
 @article{Zhang_2025,
  title={A Comprehensive Survey on Multimodal RAG: All Combinations of Modalities as Input and Output},
  url={http://dx.doi.org/10.36227/techrxiv.176341513.38473003/v1},
  DOI={10.36227/techrxiv.176341513.38473003/v1},
  publisher={Institute of Electrical and Electronics Engineers (IEEE)},
  author={Rui Zhang and Chen Liu and Yixin Su and Ruixuan Li and Xuanjing Huang and Xuelong Li and Philip S Yu},
  year={2025},
  month=nov
}
```

