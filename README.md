# lookup-argument论文管理仓库

## 📌 目录
- [1. Classification Based on Fundamental Mathematical Principles](#1-Classification-Based-on-Fundamental-Mathematical-Principles)
  - [1.1 Based on multiset equality](#11-Based_on_multiset_equality)
  - [1.2 基于 memory checking](#12-基于-memory-checking)
  - [1.3 基于 logarithmic derivatives](#13-基于-logarithmic-derivatives)
  - [1.4 基于 Matrix vector multiplication](#14-基于-Matrix-vector-multiplication)
  - [1.5 基于 vanishing polynomial](#15-基于-vanishing-polynomial)
- [2. 查找对象分类](#2-查找对象分类)
  - [2.1 元素查找element lookup](#21-元素查找element-lookup)
  - [2.2 向量查找vector lookup](#22-向量查找vector-lookup)
  - [2.3 矩阵查找matrix lookup](#23-矩阵查找matrix-lookup)
- [3. 零知识分类](#3-零知识分类)
  - [3.1 非零知识](#31-非零知识)
  - [3.2 部分零知识](#32-部分零知识)
  - [3.3 完全零知识](#33-完全零知识)
- [4. 需要预处理/可更新分类](#4-需要预处理/可更新分类)
  - [4.1 需要预处理/不可更新](#41-需要预处理/不可更新)
  - [4.2 不需预处理/可更新](#42-不需预处理/可更新)
  - [4.3 需要预处理/可更新](#43-需要预处理/可更新)

---

## 1. Classification Based on Fundamental Mathematical Principles
### 1.1 基于 multiset equality
Halo 2 lookup,      Plookup 
- [plookup: A simplified polynomial protocol for lookup tables](https://eprint.iacr.org/2020/315.pdf)
- [halo2](https://zcash.github.io/halo2/design/proving-system/lookup.html)

### 1.2 基于 memory checking
(spartan),     GKR version in lasso
- [Spartan:Efficient and general-purpose zkSNARKs without trusted setup](https://eprint.iacr.org/2019/550.pdf)CRYPTO 2020
- [Unlocking_the_lookup_singularity_with_Lasso](https://eprint.iacr.org/2023/1216.pdf)EUROCRYPT 2024
- [Scalable Zero-knowledge Proofs for Non-linear Functions in Machine Learning](https://www.usenix.org/system/files/usenixsecurity24-hao-meng-scalable.pdf)USENIX 2024
### 1.3 基于 logarithmic derivatives
Logup, cq,
cq+  （Lookup Arguments: Improvements, Extensions and Applications to Zero-Knowledge Decision Trees论文）
cqlin   
Locq  Efficient KZG-based Univariate Sum-check and Lookup Argument论文
logup+GKR（Improving logarithmic derivative lookups using GKR论文）
μ-seek（Natively Compatible Super-Efficient Lookup Arguments and How to Apply Them论文）
Tlookup（zkLLM: Zero Knowledge Proofs for Large Language Models论文）
- [Multivariate lookups based on logarithmic derivatives(Logup)](https://eprint.iacr.org/2022/1530.pdf)
- [cq: Cached quotients for fast lookups](https://eprint.iacr.org/2022/1763.pdf)
- [cq+ Lookup Arguments: Improvements, Extensions and Applications to Zero-Knowledge Decision Trees](https://eprint.iacr.org/2023/1518.pdf)PKC 2024
- [cqlin: Efficient linear operations on KZG commitments with cached quotients](https://eprint.iacr.org/2023/393.pdf)
- [Locq Efficient KZG-based Univariate Sum-check and Lookup Argument](https://eprint.iacr.org/2024/618.pdf)PKC 2024
- [Improving logarithmic derivative lookups using GKR](https://eprint.iacr.org/2023/1284.pdf)
- [Natively Compatible Super-Efficient Lookup Arguments and How to Apply Them](https://eprint.iacr.org/2024/1058.pdf)IACR in JOC 2024
- [zkLLM: Zero Knowledge Proofs for Large Language Models](https://arxiv.org/pdf/2404.16109)CCS 2024
- [MuxProofs: Succinct Arguments for Machine Computation from Vector Lookups](https://eprint.iacr.org/2023/974.pdf)ASIACRYPT 2024
- [SublonK: Sublinear Prover PlonK](https://eprint.iacr.org/2023/902.pdf)
### 1.4 基于 Matrix vector multiplication
Part of Lasso， Baloo，  FLI（FLI: Folding Lookup Instances论文）
- [FLI: Folding Lookup Instances](https://eprint.iacr.org/2024/1531.pdf)ASIACRYPT 2024
- [Baloo: Nearly Optimal Lookup Arguments](https://eprint.iacr.org/2022/1565.pdf)
- [Unlocking_the_lookup_singularity_with_Lasso](https://eprint.iacr.org/2023/1216.pdf)EUROCRYPT 2024
### 1.5 基于 vanishing polynomial
基于vanishing polynomial：caulk，caulk+，flookup
Batching-Efficient RAM using Updatable Lookup Arguments论文基于的lookup是Caulk+
- [Caulk: Lookup_Arguments_in_Sublinear_Time](https://eprint.iacr.org/2022/621.pdf)CCS 2022

  [slides](https://www.slideshare.net/AlexPruden/caulk-zkstudyclub-caulk-lookup-arguments-in-sublinear-time-a-zapico?from_search=0)
- [Caulk+: Table-independent_lookup_arguments](https://eprint.iacr.org/2022/957.pdf)
- [flookup: Fractional decomposition-based_lookups_in_quasi-linear_time_independent_of_table_size](https://eprint.iacr.org/2022/1447.pdf)
- [Batching-Efficient RAM using Updatable Lookup Arguments](https://eprint.iacr.org/2024/840.pdf)CCS 2024
## 2. 查找对象分类
### 2.1 元素查找element lookup
- [plookup: A simplified polynomial protocol for lookup tables](https://eprint.iacr.org/2020/315.pdf)
- [halo2](https://zcash.github.io/halo2/design/proving-system/lookup.html)


### 2.2 向量查找vector lookup
- [Multivariate lookups based on logarithmic derivatives(Logup)](https://eprint.iacr.org/2022/1530.pdf)
- [MuxProofs: Succinct Arguments for Machine Computation from Vector Lookups](https://eprint.iacr.org/2023/974.pdf)ASIACRYPT 2024

### 2.3 矩阵查找matrix lookup
- [cq+ Lookup Arguments: Improvements, Extensions and Applications to Zero-Knowledge Decision Trees](https://eprint.iacr.org/2023/1518.pdf)PKC 2024

## 3. 零知识分类
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


## 4. 需要预处理/可更新分类
### 4.1 需要预处理/不可更新
如何上传新的论文 PDF。

### 4.2 不需预处理/可更新
如何添加 BibTeX 文件。

### 4.3 需要预处理/可更新
如何记录阅读笔记。
