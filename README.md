# Lookup Arguments

## 📌 Contents
- [Foundations of Lookup Arguments](#-Foundations-of-Lookup-Arguments)
  - [Sumcheck](#-SumCheck)
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
  - [3.2 Partial Zero-Knowledge](#32-Partial-Zero-Knowledge)
  - [3.3 Fully Zero-Knowledge](#33-Fully-Zero-Knowledge)
- [4. Classification Based on Preprocessing and Updatability](#4-Classification-Based-on-Preprocessing-and-Updatability)
  - [4.1 Need preprocessing_Non-Updatable](#41-Need-preprocessing_Non-Updatable)
  - [4.2 No_preprocessing_Updatable](#42-No-preprocessing_Updatable)
  - [4.3 Need preprocessing_Updatable](#43-Need-preprocessing_Updatable)
- [5. Applications of Lookup Arguments](#5-Applications-of-Lookup-Arguments)
  - [5.1 zk-SNARK](#51-zk-SNARK)
  - [5.2 Blockchain zkVM zkEVM](#52-Blockchain-zkVM-zkEVM)
  - [5.3 ZKML](#53-ZKML)


- [6. Other Resources](#6-Other-Resources)
  - Lookup Overviews
---

## Foundations of Lookup Arguments
### SumCheck

### Polynomial Commitments

### Offline Memory Checking


## 1. Classification Based on Fundamental Mathematical Principles
### 1.1 Based on multiset equality
Halo 2 lookup,      Plookup 
- [plookup: A simplified polynomial protocol for lookup tables](https://eprint.iacr.org/2020/315.pdf)&nbsp;&nbsp;&nbsp;&nbsp;eprint version
  - [note by GuoYu](https://github.com/sec-bit/learning-zkp/blob/master/plonk-intro-zh/7-plonk-lookup.md)
  - [note by Ariel Gabizon](https://hackmd.io/@relgabizon/ByFgSDA7D)
  - [slides](https://aztec.slides.com/suyashbagad_aztec/plookup-and-plonk#/2/0/16)
  - [video](https://www.youtube.com/watch?v=Vdlc1CmRYRY)
  - [implementation](https://github.com/kevaundray/plookup)
- [halo2](https://zcash.github.io/halo2/design/proving-system/lookup.html)
  - [note by GuoYu](https://github.com/sec-bit/learning-zkp/blob/master/plonk-intro-zh/7-plonk-lookup.md)
  - [video](https://www.youtube.com/watch?v=3ie2yZ7CT5A)
  - [implementation](https://github.com/DoHoonKim8/halo2-lasso)
- [DUPLEX: Scalable Zero-Knowledge Lookup Arguments over RSA Group](https://eprint.iacr.org/2024/1509.pdf)

### 1.2 Based on memory checking
(spartan),     GKR version in lasso
- [Spartan:Efficient and general-purpose zkSNARKs without trusted setup](https://eprint.iacr.org/2019/550.pdf)&nbsp;&nbsp;(full version)&nbsp;&nbsp;&nbsp;&nbsp;CRYPTO 2020
  - [short version](https://link.springer.com/content/pdf/10.1007/978-3-030-56877-1_25.pdf)
  - [slides](https://iacr.org/submit/files/slides/2020/crypto/crypto2020/304/slides.pptx)
  - [video](https://www.youtube.com/watch?v=FPQs7T7f_AU)
  - [implementation](https://github.com/microsoft/Spartan)
- [Unlocking_the_lookup_singularity_with_Lasso](https://eprint.iacr.org/2023/1216.pdf)&nbsp;&nbsp;(full version)&nbsp;&nbsp;&nbsp;&nbsp;EUROCRYPT 2024
  - [short version](https://link.springer.com/content/pdf/10.1007/978-3-031-58751-1_7)
  - [note by GuoYu](https://github.com/sec-bit/learning-zkp/tree/master/lookup-arguments/lasso-zh)
  - [video](https://youtu.be/_WsCQc9Elcg)
  - [slides](https://iacr.org/submit/files/slides/2024/eurocrypt/eurocrypt2024/346/slides.pptx)
  - [implementation](https://github.com/zkp-learning/Lasso)
- [Scalable Zero-knowledge Proofs for Non-linear Functions in Machine Learning](https://eprint.iacr.org/2025/507.pdf)&nbsp;&nbsp;(full version)&nbsp;&nbsp;&nbsp;&nbsp;USENIX 2024
  - [short version](https://www.usenix.org/system/files/usenixsecurity24-hao-meng-scalable.pdf)
  - [video](https://youtu.be/OXOcq4avvP8)
  - [slides](https://www.usenix.org/system/files/usenixsecurity24_slides-hao-meng-scalable.pdf)
  - [implementation](https://github.com/CryptMatrix/ZKMath)
- [(zklasso)SNARKs for Virtual Machines are Non-Malleable](https://eprint.iacr.org/2024/1551.pdf)&nbsp;&nbsp;(full version)&nbsp;&nbsp;&nbsp;&nbsp;EUROCRYPT 2025
  - [short version](https://hal.science/hal-04991788v1/file/publi-8049.pdf)
  - [video](https://www.youtube.com/watch?v=gPV0T9YIrH4)
- [TaSSLE: Lasso for the commitment-phobic](https://eprint.iacr.org/2024/1075.pdf)
  - [blog](https://www.lita.foundation/blog/tassle-tensors-and-sumcheck-for-structured-lookup-efficiency)
- [Twist and Shout: Faster memory checking arguments via one-hot addressing and increments](https://eprint.iacr.org/2025/105.pdf)
### 1.3 Based on logarithmic derivatives
Logup, cq,
cq+  （Lookup Arguments: Improvements, Extensions and Applications to Zero-Knowledge Decision Trees）
cqlin   
Locq  Efficient KZG-based Univariate Sum-check and Lookup Argument
logup+GKR（Improving logarithmic derivative lookups using GKR）
μ-seek（Natively Compatible Super-Efficient Lookup Arguments and How to Apply Them）
Tlookup（zkLLM: Zero Knowledge Proofs for Large Language Models）
- [Multivariate lookups based on logarithmic derivatives(Logup)](https://eprint.iacr.org/2022/1530.pdf)
  - [notes 1](https://georgwiese.github.io/crypto-summaries/Concepts/Protocols/Lookup-Arguments/LogUp--and--cq)
  - [notes 2](https://blog.csdn.net/mutourend/article/details/127745883)
  - [video](https://www.youtube.com/watch?v=qv_5dF2_C4g)
  - [implementation](https://github.com/yugocabrio/oreno-lookup)
- [cq: Cached quotients for fast lookups](https://eprint.iacr.org/2022/1763.pdf)
  - [notes](https://georgwiese.github.io/crypto-summaries/Concepts/Protocols/Lookup-Arguments/LogUp--and--cq)
  - [video 1](https://www.youtube.com/watch?v=HJPOfkBcldE&t=357s)
  - [video 2](https://youtu.be/KQi3WdZvI6w)
  - [implementation](https://github.com/geometryxyz/cq)
- [cq+ Lookup Arguments: Improvements, Extensions and Applications to Zero-Knowledge Decision Trees](https://eprint.iacr.org/2023/1518.pdf)&nbsp;&nbsp;(full version)&nbsp;&nbsp;&nbsp;&nbsp;PKC 2024
  - [short version](https://link.springer.com/content/pdf/10.1007/978-3-031-57722-2_11.pdf)
  - [slides](https://iacr.org/submit/files/slides/2024/pkc/pkc2024/48/slides.pdf)
- [cqlin: Efficient linear operations on KZG commitments with cached quotients](https://eprint.iacr.org/2023/393.pdf)
  - [slides](https://www.slideshare.net/slideshow/zkstudyclub-cqlin-efficient-linear-operations-on-kzg-commitments/258231653)
  - [video](https://www.youtube.com/watch?v=mxvaThCgU9c)
- [Locq Efficient KZG-based Univariate Sum-check and Lookup Argument](https://eprint.iacr.org/2024/618.pdf)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;PKC 2024
  - [slides](https://iacr.org/submit/files/slides/2024/pkc/pkc2024/99/slides.pdf)
- [Improving logarithmic derivative lookups using GKR](https://eprint.iacr.org/2023/1284.pdf)
  - [video](https://www.youtube.com/watch?v=DCEg61ExwK4&t=139s)
- [Natively Compatible Super-Efficient Lookup Arguments and How to Apply Them](https://eprint.iacr.org/2024/1058.pdf)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;JOC 2024
  - [video](https://www.youtube.com/watch?v=eRKn5uFK0V0)
- [zkLLM: Zero Knowledge Proofs for Large Language Models](https://arxiv.org/pdf/2404.16109)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;CCS 2024  
  - [implementation](https://github.com/jvhs0706/zkllm-ccs2024)
- [MuxProofs: Succinct Arguments for Machine Computation from Vector Lookups](https://eprint.iacr.org/2023/974.pdf)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ASIACRYPT 2024
  - [slides](https://iacr.org/submit/files/slides/2024/asiacrypt/asiacrypt2024/313/313_slides.pdf)
  - [implementation](https://github.com/lucasxia01/mux-proofs-impl)
- [SublonK: Sublinear Prover PlonK](https://eprint.iacr.org/2023/902.pdf)
  - [implementation](https://github.com/txaty/ark-segmentlookup)
- [Soloist: Distributed SNARKs for Rank-One Constraint System](https://eprint.iacr.org/2025/557.pdf)&nbsp;&nbsp;&nbsp;&nbsp;distributed lookup based on logup
- [ProtoStar: Generic Efficient Accumulation/Folding for Special Sound Protocols](https://eprint.iacr.org/2023/620.pdf)&nbsp;&nbsp;&nbsp;&nbsp;ASIACRYPT 2023&nbsp;&nbsp;&nbsp;&nbsp;adapt logarithmic derivatives in folding
### 1.4 Based on Matrix vector multiplication
Part of Lasso， Baloo，  FLI（FLI: Folding Lookup Instances）
- [FLI: Folding Lookup Instances](https://eprint.iacr.org/2024/1531.pdf)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ASIACRYPT 2024
  - [slides](https://iacr.org/submit/files/slides/2024/asiacrypt/asiacrypt2024/197/197_slides.pdf)
- [Baloo: Nearly Optimal Lookup Arguments](https://eprint.iacr.org/2022/1565.pdf)
  - [notes](https://github.com/sec-bit/learning-zkp/tree/master/lookup-arguments/baloo-en)
  - [implementation](https://github.com/geometryxyz/baloo?tab=readme-ov-file)
- [Unlocking_the_lookup_singularity_with_Lasso](https://eprint.iacr.org/2023/1216.pdf)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;EUROCRYPT 2024
  - [note by GuoYu](https://github.com/sec-bit/learning-zkp/tree/master/lookup-arguments/lasso-zh)
  - [video](https://youtu.be/_WsCQc9Elcg)
  - [slides](https://iacr.org/submit/files/slides/2024/eurocrypt/eurocrypt2024/346/slides.pptx)
  - [implementation](https://github.com/zkp-learning/Lasso)
- [(zklasso)SNARKs for Virtual Machines are Non-Malleable](https://eprint.iacr.org/2024/1551.pdf)&nbsp;&nbsp;&nbsp;&nbsp;EUROCRYPT 2025
- [TaSSLE: Lasso for the commitment-phobic](https://eprint.iacr.org/2024/1075.pdf)
### 1.5 Based on vanishing polynomial
Based on vanishing polynomial：caulk，caulk+，flookup
"Batching-Efficient RAM using Updatable Lookup Argumentslookup" is based on Caulk+
- [Caulk: Lookup_Arguments_in_Sublinear_Time](https://eprint.iacr.org/2022/621.pdf)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;CCS 2022
  - [notes](https://asdavinci.ing/post/caulk-caulk+note/)
  - [slides](https://www.slideshare.net/AlexPruden/caulk-zkstudyclub-caulk-lookup-arguments-in-sublinear-time-a-zapico?from_search=0)
  - [video](https://www.youtube.com/watch?v=uEssF2WzIeU)
  - [implementation](https://github.com/caulk-crypto/caulk)
- [Caulk+: Table-independent_lookup_arguments](https://eprint.iacr.org/2022/957.pdf)
  - [notes](https://asdavinci.ing/post/caulk-caulk+note/)
  - [implementation](https://github.com/CPerezz/caulk_plus)
- [flookup: Fractional decomposition-based_lookups_in_quasi-linear_time_independent_of_table_size](https://eprint.iacr.org/2022/1447.pdf)
- [Batching-Efficient RAM using Updatable Lookup Arguments](https://eprint.iacr.org/2024/840.pdf)&nbsp;&nbsp;(full version)&nbsp;&nbsp;&nbsp;&nbsp;CCS 2024
  - [short version](https://dl.acm.org/doi/pdf/10.1145/3658644.3670356)
## 2. Classification Based on Lookup Objects
### 2.1 Element Lookup
- [plookup: A simplified polynomial protocol for lookup tables](https://eprint.iacr.org/2020/315.pdf)
  - [note by GuoYu](https://github.com/sec-bit/learning-zkp/blob/master/plonk-intro-zh/7-plonk-lookup.md)
  - [note by Ariel Gabizon](https://hackmd.io/@relgabizon/ByFgSDA7D)
  - [slides](https://aztec.slides.com/suyashbagad_aztec/plookup-and-plonk#/2/0/16)
  - [video](https://www.youtube.com/watch?v=Vdlc1CmRYRY)
- [halo2](https://zcash.github.io/halo2/design/proving-system/lookup.html)
  - [notes](https://github.com/sec-bit/learning-zkp/blob/master/plonk-intro-zh/7-plonk-lookup.md)
  - [video](https://www.youtube.com/watch?v=3ie2yZ7CT5A)

### 2.2 Vector lookup
- [Multivariate lookups based on logarithmic derivatives(Logup)](https://eprint.iacr.org/2022/1530.pdf)
  - [notes 1](https://georgwiese.github.io/crypto-summaries/Concepts/Protocols/Lookup-Arguments/LogUp--and--cq)
  - [notes 2](https://blog.csdn.net/mutourend/article/details/127745883)
  - [video](https://www.youtube.com/watch?v=qv_5dF2_C4g)
- [MuxProofs: Succinct Arguments for Machine Computation from Vector Lookups](https://eprint.iacr.org/2023/974.pdf)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ASIACRYPT 2024
  - [slides](https://iacr.org/submit/files/slides/2024/asiacrypt/asiacrypt2024/313/313_slides.pdf)
### 2.3 Matrix lookup
- [cq+ Lookup Arguments: Improvements, Extensions and Applications to Zero-Knowledge Decision Trees](https://eprint.iacr.org/2023/1518.pdf)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;PKC 2024
  - [slides](https://iacr.org/submit/files/slides/2024/pkc/pkc2024/99/slides.pdf)

## 3. Classification Based on Zero-Knowledge Property
### 3.1 Non-Zero-Knowledge
- [flookup: Fractional decomposition-based_lookups_in_quasi-linear_time_independent_of_table_size](https://eprint.iacr.org/2022/1447.pdf)
- [Baloo: Nearly Optimal Lookup Arguments](https://eprint.iacr.org/2022/1565.pdf)
  - [notes](https://github.com/sec-bit/learning-zkp/tree/master/lookup-arguments/baloo-en)
- [cq: Cached quotients for fast lookups](https://eprint.iacr.org/2022/1763.pdf)
  - [notes](https://georgwiese.github.io/crypto-summaries/Concepts/Protocols/Lookup-Arguments/LogUp--and--cq)
  - [video 1](https://www.youtube.com/watch?v=HJPOfkBcldE&t=357s)
  - [video 2](https://youtu.be/KQi3WdZvI6w)

### 3.2 Partial Zero-Knowledge
- [cq+ Lookup Arguments: Improvements, Extensions and Applications to Zero-Knowledge Decision Trees](https://eprint.iacr.org/2023/1518.pdf)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;PKC 2024
  - [slides](https://iacr.org/submit/files/slides/2024/pkc/pkc2024/99/slides.pdf)

### 3.3 Fully Zero-Knowledge
- [Caulk: Lookup_Arguments_in_Sublinear_Time](https://eprint.iacr.org/2022/621.pdf)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;CCS 2022
  - [notes](https://asdavinci.ing/post/caulk-caulk+note/)
  - [slides](https://www.slideshare.net/AlexPruden/caulk-zkstudyclub-caulk-lookup-arguments-in-sublinear-time-a-zapico?from_search=0)
  - [video](https://www.youtube.com/watch?v=uEssF2WzIeU)
- [Caulk+: Table-independent_lookup_arguments](https://eprint.iacr.org/2022/957.pdf)
  - [notes](https://asdavinci.ing/post/caulk-caulk+note/)
- [cq+ Lookup Arguments: Improvements, Extensions and Applications to Zero-Knowledge Decision Trees](https://eprint.iacr.org/2023/1518.pdf)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;PKC 2024
  - [slides](https://iacr.org/submit/files/slides/2024/pkc/pkc2024/48/slides.pdf)
- [zkcq+ Locq Efficient KZG-based Univariate Sum-check and Lookup Argument](https://eprint.iacr.org/2024/618.pdf)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;PKC 2024
  - [slides](https://iacr.org/submit/files/slides/2024/pkc/pkc2024/99/slides.pdf)
- [(zklasso)SNARKs for Virtual Machines are Non-Malleable](https://eprint.iacr.org/2024/1551.pdf)&nbsp;&nbsp;&nbsp;&nbsp;EUROCRYPT 2025
- [DUPLEX: Scalable Zero-Knowledge Lookup Arguments over RSA Group](https://eprint.iacr.org/2024/1509.pdf)



## 4. Classification Based on Preprocessing and Updatability
### 4.1 Need preprocessing_Non-Updatable
- [Multivariate lookups based on logarithmic derivatives(Logup)](https://eprint.iacr.org/2022/1530.pdf)
  - [notes 1](https://georgwiese.github.io/crypto-summaries/Concepts/Protocols/Lookup-Arguments/LogUp--and--cq)
  - [notes 2](https://blog.csdn.net/mutourend/article/details/127745883)
  - [video](https://www.youtube.com/watch?v=qv_5dF2_C4g)
- [cq: Cached quotients for fast lookups](https://eprint.iacr.org/2022/1763.pdf)
  - [notes](https://georgwiese.github.io/crypto-summaries/Concepts/Protocols/Lookup-Arguments/LogUp--and--cq)
  - [video 1](https://www.youtube.com/watch?v=HJPOfkBcldE&t=357s)
  - [video 2](https://youtu.be/KQi3WdZvI6w)
- [cq+ Lookup Arguments: Improvements, Extensions and Applications to Zero-Knowledge Decision Trees](https://eprint.iacr.org/2023/1518.pdf)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;PKC 2024
  - [slides](https://iacr.org/submit/files/slides/2024/pkc/pkc2024/48/slides.pdf)
- [cqlin: Efficient linear operations on KZG commitments with cached quotients](https://eprint.iacr.org/2023/393.pdf)
- [Locq Efficient KZG-based Univariate Sum-check and Lookup Argument](https://eprint.iacr.org/2024/618.pdf)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;PKC 2024
  - [slides](https://iacr.org/submit/files/slides/2024/pkc/pkc2024/99/slides.pdf)
- [Improving logarithmic derivative lookups using GKR](https://eprint.iacr.org/2023/1284.pdf)
- [Baloo: Nearly Optimal Lookup Arguments](https://eprint.iacr.org/2022/1565.pdf)
  - [notes](https://github.com/sec-bit/learning-zkp/tree/master/lookup-arguments/baloo-en)
- [Unlocking_the_lookup_singularity_with_Lasso](https://eprint.iacr.org/2023/1216.pdf)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;EUROCRYPT 2024
  - [notes](https://github.com/sec-bit/learning-zkp/tree/master/lookup-arguments/lasso-zh)
  - [video](https://youtu.be/_WsCQc9Elcg)
  - [slides](https://iacr.org/submit/files/slides/2024/eurocrypt/eurocrypt2024/346/slides.pptx)
- [Caulk: Lookup_Arguments_in_Sublinear_Time](https://eprint.iacr.org/2022/621.pdf)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;CCS 2022
  - [notes](https://asdavinci.ing/post/caulk-caulk+note/)
  - [slides](https://www.slideshare.net/AlexPruden/caulk-zkstudyclub-caulk-lookup-arguments-in-sublinear-time-a-zapico?from_search=0)
  - [video](https://www.youtube.com/watch?v=uEssF2WzIeU)
- [Caulk+: Table-independent_lookup_arguments](https://eprint.iacr.org/2022/957.pdf)
  - [notes](https://asdavinci.ing/post/caulk-caulk+note/)
- [flookup: Fractional decomposition-based_lookups_in_quasi-linear_time_independent_of_table_size](https://eprint.iacr.org/2022/1447.pdf)
### 4.2 No preprocessing_Updatable
- [plookup: A simplified polynomial protocol for lookup tables](https://eprint.iacr.org/2020/315.pdf)
  - [note by GuoYu](https://github.com/sec-bit/learning-zkp/blob/master/plonk-intro-zh/7-plonk-lookup.md)
  - [note by Ariel Gabizon](https://hackmd.io/@relgabizon/ByFgSDA7D)
  - [slides](https://aztec.slides.com/suyashbagad_aztec/plookup-and-plonk#/2/0/16)
  - [video](https://www.youtube.com/watch?v=Vdlc1CmRYRY)
- [halo2](https://zcash.github.io/halo2/design/proving-system/lookup.html)
  - [notes](https://github.com/sec-bit/learning-zkp/blob/master/plonk-intro-zh/7-plonk-lookup.md)
  - [video](https://www.youtube.com/watch?v=3ie2yZ7CT5A)

### 4.3 Need preprocessing_Updatable
- [Batching-Efficient RAM using Updatable Lookup Arguments](https://eprint.iacr.org/2024/840.pdf)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;CCS 2024

## 5. Applications of Lookup Arguments
### 5.1 zk-SNARK
- [BabySpartan: Lasso-based SNARK for non-uniform computation](https://eprint.iacr.org/2023/1799.pdf)
### 5.2 Blockchain zkVM zkEVM
- [Jolt: SNARKs for Virtual Machines via Lookups](https://eprint.iacr.org/2023/1217)
- [Proving CPU Executions in Small Space](https://eprint.iacr.org/2025/611.pdf)
- [ZKWASM: A ZKSNARK WASM Emulator](https://ieeexplore.ieee.org/document/10587123)
  - [implementation](https://github.com/CPerezz/caulk_plus)
- [Two Shuffles Make a RAM: Improved Constant Overhead Zero Knowledge RAM](https://eprint.iacr.org/2023/1115.pdf)&nbsp;&nbsp;&nbsp;&nbsp;USENIX 2024
- [Zero Knowledge Memory-Checking Techniques for Stacks and Queues](https://eprint.iacr.org/2024/2084.pdf)
- [Nebula: Efficient read-write memory and switchboard circuits for folding schemes](https://eprint.iacr.org/2024/1605.pdf)&nbsp;&nbsp;&nbsp;&nbsp;based on Lasso
- [Polynomial IOPs for Memory Consistency Checks in Zero-Knowledge Virtual Machines](https://eprint.iacr.org/2023/1555.pdf)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ASIACRYPT 2024

  TODO
- [scroll]
- [zksync]
- [Risc0]
### 5.3 ZKML
- [Scalable Zero-knowledge Proofs for Non-linear Functions in Machine Learning](https://www.usenix.org/system/files/usenixsecurity24-hao-meng-scalable.pdf)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;USENIX 2024
  - [video](https://youtu.be/OXOcq4avvP8)
  - [slides](https://www.usenix.org/system/files/usenixsecurity24_slides-hao-meng-scalable.pdf)
  - [implementation](https://github.com/CryptMatrix/ZKMath)
- [zkLLM: Zero Knowledge Proofs for Large Language Models](https://arxiv.org/pdf/2404.16109)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;CCS 2024  
  - [implementation](https://github.com/jvhs0706/zkllm-ccs2024)
- [An Efficient and Extensible Zero-knowledge Proof Framework for Neural Networks](https://eprint.iacr.org/2024/703.pdf)
- [zkPyTorch: A Hierarchical Optimized Compiler for Zero-Knowledge Machine Learning](https://eprint.iacr.org/2025/535.pdf)


## 6. Other Resources
- [A brief history of lookup arguments](https://github.com/ingonyama-zk/papers/blob/main/lookups.pdf)
