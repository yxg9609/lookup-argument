# lookup-argument论文管理仓库

## 📌 目录
- [1. 底层数学原理分类](#1-底层数学原理分类)
  - [1.1 基于 multiset equality](#11-基于-multiset-equality)
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
  - [2.1 元素查找element lookup](#21-元素查找element-lookup)
  - [2.2 向量查找vector lookup](#22-向量查找vector-lookup)
  - [2.3 矩阵查找matrix lookup](#23-矩阵查找matrix-lookup)

---

## 1. 底层数学原理分类
### 1.1 基于 multiset equality
Halo 2 lookup,      Plookup 
- [plookup](https://eprint.iacr.org/2020/315.pdf)
- [halo2](https://zcash.github.io/halo2/design/proving-system/lookup.html)

### 1.2 基于 memory checking
(spartan),     GKR version in lasso
- [Spartan](https://eprint.iacr.org/2019/550.pdf)
- [Lasso](https://eprint.iacr.org/2023/1216.pdf)
- [Scalable Zero-knowledge Proofs for Non-linear Functions in Machine Learning](https://www.usenix.org/system/files/usenixsecurity24-hao-meng-scalable.pdf)
### 1.3 基于 logarithmic derivatives
Logup, cq,
cq+  （Lookup Arguments: Improvements, Extensions and Applications to Zero-Knowledge Decision Trees论文）
cqlin   
Locq  Efficient KZG-based Univariate Sum-check and Lookup Argument论文
logup+GKR（Improving logarithmic derivative lookups using GKR论文）
μ-seek（Natively Compatible Super-Efficient Lookup Arguments and How to Apply Them论文）
Tlookup（zkLLM: Zero Knowledge Proofs for Large Language Models论文）
- [Logup](https://eprint.iacr.org/2022/1530.pdf)
- [cq: Cached quotients for fast lookups](https://eprint.iacr.org/2022/1763.pdf)
- [cq+ Lookup Arguments: Improvements, Extensions and Applications to Zero-Knowledge Decision Trees](https://eprint.iacr.org/2023/1518.pdf)
- [cqlin: Efficient linear operations on KZG commitments with cached quotients](https://eprint.iacr.org/2023/393.pdf)
- [Locq Efficient KZG-based Univariate Sum-check and Lookup Argument](https://eprint.iacr.org/2024/618.pdf)
- [Improving logarithmic derivative lookups using GKR](https://eprint.iacr.org/2023/1284.pdf)
- [Natively Compatible Super-Efficient Lookup Arguments and How to Apply Them](https://eprint.iacr.org/2024/1058.pdf)
- [zkLLM: Zero Knowledge Proofs for Large Language Models](https://arxiv.org/pdf/2404.16109)CCS 24
- [MuxProofs: Succinct Arguments for Machine Computation from Vector Lookups](papers/MuxProofs_Succinct_Arguments_for_Machine_Computation_from_Vector_Lookups.pdf)
- [SublonK: Sublinear Prover PlonK](papers/SublonK_Sublinear_Prover_PlonK.pdf)
### 1.4 基于 Matrix vector multiplication
Part of Lasso， Baloo，  FLI（FLI: Folding Lookup Instances论文）
- [Folding lookup](papers/FLI_Folding_Lookup_Instances.pdf)
- [Baloo](papers/Baloo_Nearly_Optimal_Lookup_Arguments.pdf)
- [Lasso](papers/Unlocking_the_lookup_singularity_with_Lasso.pdf)
### 1.5 基于 vanishing polynomial
基于vanishing polynomial：caulk，caulk+，flookup
Batching-Efficient RAM using Updatable Lookup Arguments论文基于的lookup是Caulk+
- [Caulk](papers/Caulk_Lookup_Arguments_in_Sublinear_Time.pdf)
- [Caulk+](papers/Caulk+Table-independent_lookup_arguments.pdf)
- [flookup](papers/flookup_Fractional_decomposition-based_lookups_in_quasi-linear_time_independent_of_table_size.pdf)
- [Batching-Efficient RAM using Updatable Lookup Arguments](papers/Batching-Efficient_RAM_using_Updatable_Lookup_Arguments.pdf)
## 2. 查找对象分类
### 2.1 元素查找element lookup
如何上传新的论文 PDF。

### 2.2 向量查找vector lookup
如何添加 BibTeX 文件。

### 2.3 矩阵查找matrix lookup
如何记录阅读笔记。


## 3. 零知识分类
### 3.1 非零知识
如何上传新的论文 PDF。

### 3.2 部分零知识
如何添加 BibTeX 文件。

### 3.3 完全零知识
如何记录阅读笔记。
