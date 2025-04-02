# Lookup Arguments

## 📌 Contents
- [1. Classification Based on Fundamental Mathematical Principles](#1-Classification-Based-on-Fundamental-Mathematical-Principles)
  - [1.1 Based on multiset equality](#11-Based-on-multiset-equality)
  - [1.2 Based on memory checking](#12-Based-on-memory-checking)
  - [1.3 Based on logarithmic derivatives](#13-Based-on-logarithmic-derivatives)
  - [1.4 Based on Matrix vector multiplication](#14-Based-on-Matrix-vector-multiplication)
  - [1.5 Based on vanishing polynomial](#15-Based-on-vanishing-polynomial)
- [2. Classification Based on Lookup Objects](#2-Classification-Based-on-Lookup-Objects)
  - [2.1 Element lookup](#21-Element-lookup)
  - [2.2 Vector lookup](#22-Vector-lookup)
  - [2.3 Matrix lookup](#23-Matrix-lookup)
- [3. Classification Based on Zero-Knowledge Property](#3-Classification-Based-on-Zero-Knowledge-Property)
  - [3.1 Non-Zero-Knowledge](#31-Non-Zero-Knowledge)
  - [3.2 部分零知识](#32-部分零知识)
  - [3.3 完全零知识](#33-完全零知识)
- [4. Classification Based on Preprocessing and Updatability](#4-Classification-Based-on-Preprocessing-and-Updatability)
  - [4.1 Need preprocessing, Non-Updatable](#41-Need-preprocessing,-Non-Updatable)
  - [4.2 No preprocessing, Updatable](#42-No-preprocessing,-Updatable)
  - [4.3 Need preprocessing, Updatable](#43-Need-preprocessing,-Updatable)

---

## 1. Classification Based on Fundamental Mathematical Principles
### 1.1 Based on multiset equality
Halo 2 lookup,      Plookup 
- [plookup: A simplified polynomial protocol for lookup tables](https://eprint.iacr.org/2020/315.pdf)
  - [notes](https://github.com/sec-bit/learning-zkp/blob/master/plonk-intro-zh/7-plonk-lookup.md)   
  - [slides](https://aztec.slides.com/suyashbagad_aztec/plookup-and-plonk#/2/0/16)
  
- [halo2](https://zcash.github.io/halo2/design/proving-system/lookup.html)
  - [notes](https://github.com/sec-bit/learning-zkp/blob/master/plonk-intro-zh/7-plonk-lookup.md)

### 1.2 Based on memory checking
(spartan),     GKR version in lasso
- [Spartan:Efficient and general-purpose zkSNARKs without trusted setup](https://eprint.iacr.org/2019/550.pdf)CRYPTO 2020
  - [slides](https://iacr.org/submit/files/slides/2020/crypto/crypto2020/304/slides.pptx)
  - [video](https://www.youtube.com/watch?v=FPQs7T7f_AU)
- [Unlocking_the_lookup_singularity_with_Lasso](https://eprint.iacr.org/2023/1216.pdf)EUROCRYPT 2024
  - [notes](https://github.com/sec-bit/learning-zkp/tree/master/lookup-arguments/lasso-zh))
  - [video](https://youtu.be/_WsCQc9Elcg)
  - [slides](https://iacr.org/submit/files/slides/2024/eurocrypt/eurocrypt2024/346/slides.pptx)
- [Scalable Zero-knowledge Proofs for Non-linear Functions in Machine Learning](https://www.usenix.org/system/files/usenixsecurity24-hao-meng-scalable.pdf)USENIX 2024
  - [video](https://youtu.be/OXOcq4avvP8)
  - [slides](https://www.usenix.org/system/files/usenixsecurity24_slides-hao-meng-scalable.pdf)
### 1.3 Based on logarithmic derivatives
Logup, cq,
cq+  （Lookup Arguments: Improvements, Extensions and Applications to Zero-Knowledge Decision Trees论文）
cqlin   
Locq  Efficient KZG-based Univariate Sum-check and Lookup Argument论文
logup+GKR（Improving logarithmic derivative lookups using GKR论文）
μ-seek（Natively Compatible Super-Efficient Lookup Arguments and How to Apply Them论文）
Tlookup（zkLLM: Zero Knowledge Proofs for Large Language Models论文）
- [Multivariate lookups based on logarithmic derivatives(Logup)](https://eprint.iacr.org/2022/1530.pdf)
  - [notes 1](https://georgwiese.github.io/crypto-summaries/Concepts/Protocols/Lookup-Arguments/LogUp--and--cq)
  - [notes 2](https://blog.csdn.net/mutourend/article/details/127745883)
  - [video](https://www.youtube.com/watch?v=qv_5dF2_C4g)
- [cq: Cached quotients for fast lookups](https://eprint.iacr.org/2022/1763.pdf)
  - [notes](https://georgwiese.github.io/crypto-summaries/Concepts/Protocols/Lookup-Arguments/LogUp--and--cq)
  - [video 1](https://www.youtube.com/watch?v=HJPOfkBcldE&t=357s)
  - [video 2](https://youtu.be/KQi3WdZvI6w)
- [cq+ Lookup Arguments: Improvements, Extensions and Applications to Zero-Knowledge Decision Trees](https://eprint.iacr.org/2023/1518.pdf)PKC 2024
  - [slides](https://iacr.org/submit/files/slides/2024/pkc/pkc2024/48/slides.pdf)
- [cqlin: Efficient linear operations on KZG commitments with cached quotients](https://eprint.iacr.org/2023/393.pdf)
- [Locq Efficient KZG-based Univariate Sum-check and Lookup Argument](https://eprint.iacr.org/2024/618.pdf)PKC 2024
  - [slides](https://iacr.org/submit/files/slides/2024/pkc/pkc2024/99/slides.pdf)
- [Improving logarithmic derivative lookups using GKR](https://eprint.iacr.org/2023/1284.pdf)
- [Natively Compatible Super-Efficient Lookup Arguments and How to Apply Them](https://eprint.iacr.org/2024/1058.pdf)IACR in JOC 2024
- [zkLLM: Zero Knowledge Proofs for Large Language Models](https://arxiv.org/pdf/2404.16109)CCS 2024
- [MuxProofs: Succinct Arguments for Machine Computation from Vector Lookups](https://eprint.iacr.org/2023/974.pdf)ASIACRYPT 2024
  - [slides](https://iacr.org/submit/files/slides/2024/asiacrypt/asiacrypt2024/313/313_slides.pdf)
- [SublonK: Sublinear Prover PlonK](https://eprint.iacr.org/2023/902.pdf)
### 1.4 Based on Matrix vector multiplication
Part of Lasso， Baloo，  FLI（FLI: Folding Lookup Instances论文）
- [FLI: Folding Lookup Instances](https://eprint.iacr.org/2024/1531.pdf)ASIACRYPT 2024
  - [slides](https://iacr.org/submit/files/slides/2024/asiacrypt/asiacrypt2024/197/197_slides.pdf)
- [Baloo: Nearly Optimal Lookup Arguments](https://eprint.iacr.org/2022/1565.pdf)
  - [notes](https://github.com/sec-bit/learning-zkp/tree/master/lookup-arguments/baloo-en)
- [Unlocking_the_lookup_singularity_with_Lasso](https://eprint.iacr.org/2023/1216.pdf)EUROCRYPT 2024
  - [notes](https://github.com/sec-bit/learning-zkp/tree/master/lookup-arguments/lasso-zh)
### 1.5 Based on vanishing polynomial
基于vanishing polynomial：caulk，caulk+，flookup
Batching-Efficient RAM using Updatable Lookup Arguments论文基于的lookup是Caulk+
- [Caulk: Lookup_Arguments_in_Sublinear_Time](https://eprint.iacr.org/2022/621.pdf)CCS 2022
  - [notes](https://asdavinci.ing/post/caulk-caulk+note/)
  - [slides](https://www.slideshare.net/AlexPruden/caulk-zkstudyclub-caulk-lookup-arguments-in-sublinear-time-a-zapico?from_search=0)
  - [video](https://www.youtube.com/watch?v=uEssF2WzIeU)
- [Caulk+: Table-independent_lookup_arguments](https://eprint.iacr.org/2022/957.pdf)
  - [notes](https://asdavinci.ing/post/caulk-caulk+note/)
- [flookup: Fractional decomposition-based_lookups_in_quasi-linear_time_independent_of_table_size](https://eprint.iacr.org/2022/1447.pdf)
- [Batching-Efficient RAM using Updatable Lookup Arguments](https://eprint.iacr.org/2024/840.pdf)CCS 2024
## 2. Classification Based on Lookup Objects
### 2.1 Element Lookup
- [plookup: A simplified polynomial protocol for lookup tables](https://eprint.iacr.org/2020/315.pdf)
- [halo2](https://zcash.github.io/halo2/design/proving-system/lookup.html)


### 2.2 Vector lookup
- [Multivariate lookups based on logarithmic derivatives(Logup)](https://eprint.iacr.org/2022/1530.pdf)
- [MuxProofs: Succinct Arguments for Machine Computation from Vector Lookups](https://eprint.iacr.org/2023/974.pdf)ASIACRYPT 2024

### 2.3 Matrix lookup
- [cq+ Lookup Arguments: Improvements, Extensions and Applications to Zero-Knowledge Decision Trees](https://eprint.iacr.org/2023/1518.pdf)PKC 2024

## 3. Classification Based on Zero-Knowledge Property
### 3.1 非零知识
- [flookup: Fractional decomposition-based_lookups_in_quasi-linear_time_independent_of_table_size](https://eprint.iacr.org/2022/1447.pdf)
- [Baloo: Nearly Optimal Lookup Arguments](https://eprint.iacr.org/2022/1565.pdf)
- [cq: Cached quotients for fast lookups](https://eprint.iacr.org/2022/1763.pdf)

### 3.2 部分零知识
- [cq+ Lookup Arguments: Improvements, Extensions and Applications to Zero-Knowledge Decision Trees](https://eprint.iacr.org/2023/1518.pdf)PKC 2024

### 3.3 完全零知识
- [Caulk: Lookup_Arguments_in_Sublinear_Time](https://eprint.iacr.org/2022/621.pdf)CCS 2022
- [Caulk+: Table-independent_lookup_arguments](https://eprint.iacr.org/2022/957.pdf)
- [Locq Efficient KZG-based Univariate Sum-check and Lookup Argument](https://eprint.iacr.org/2024/618.pdf)PKC 2024
- [zkcq+ Lookup Arguments: Improvements, Extensions and Applications to Zero-Knowledge Decision Trees](https://eprint.iacr.org/2023/1518.pdf)PKC 2024


## 4. Classification Based on Preprocessing and Updatability
### 4.1 Need preprocessing, Non-Updatable
如何上传新的论文 PDF。

### 4.2 No preprocessing, Updatable
如何添加 BibTeX 文件。

### 4.3 Need preprocessing, Updatable
如何记录阅读笔记。
