# Lookup Arguments

## 🔄 Keeping Your Fork Updated

If you've forked this repository and want to keep it up-to-date with the latest changes, you can set the original repo as an upstream remote and periodically sync updates using the following commands:

```bash
# Add the original repo as an upstream remote
git remote add upstream https://github.com/yxg9609/lookup-argument.git

# Fetch the latest changes from upstream
git fetch upstream

# Merge the changes into your local branch
git merge upstream/main
```

This will help you stay in sync with the latest papers, summaries, or tools added to this repository.

> 💡 Feel free to open a pull request if you have something useful to contribute!

---
## 📌 Contents <a name="contents"></a>


<details open>
<summary><strong>Foundation Knowledges of Lookup Arguments</strong></summary>

  - [Sumcheck](#sumcheck)
  - [Polynomial Commitments](#polynomial-commitments)
  - [Low Degree and Multilinear Extensions](#low-degree-and-multilinear-extensions)
  - [Logarithmic Derivative](#logarithmic-derivative)
  - [Offline Memory Checking](#offline-memory-checking)
  - [Multiset Euqlity](#multiset-euqlity)
  - [GKR](#gkr)

</details>

<details open>
<summary><strong>1. Classification Based on Fundamental Mathematical Principles</strong></summary>

  - [1.1 Based on multiset equality](#11-Based-on-multiset-equality)
  - [1.2 Based on memory checking](#12-Based-on-memory-checking)
  - [1.3 Based on logarithmic derivatives](#13-Based-on-logarithmic-derivatives)
  - [1.4 Based on Matrix vector multiplication](#14-Based-on-Matrix-vector-multiplication)
  - [1.5 Based on vanishing polynomial](#15-Based-on-vanishing-polynomial)

</details>

<details open>
<summary><strong>2. Classification Based on Lookup Objects</strong></summary>

  - [2.1 Element lookup](#21-Element-lookup)
  - [2.2 Vector lookup](#22-Vector-lookup)
  - [2.3 Matrix lookup](#23-Matrix-lookup)

</details>

<details open>
<summary><strong>3. Classification Based on Zero-Knowledge Property</strong></summary>
  
  - [3.1 Non-Zero-Knowledge](#31-Non-Zero-Knowledge)
  - [3.2 Partial Zero-Knowledge](#32-Partial-Zero-Knowledge)
  - [3.3 Fully Zero-Knowledge](#33-Fully-Zero-Knowledge)

</details>


<details open>
<summary><strong>4. Classification Based on Preprocessing and Updatability</strong></summary>
  
  - [4.1 Need preprocessing_Non-Updatable](#41-Need-preprocessing_Non-Updatable)
  - [4.2 No_preprocessing_Updatable](#42-No-preprocessing_Updatable)
  - [4.3 Need preprocessing_Updatable](#43-Need-preprocessing_Updatable)

</details>

<details open>
  <summary><strong>5. Applications of Lookup Arguments</strong></summary>

  - [5.1 zk-SNARK](#51-zk-SNARK)
  - [5.2 Blockchain](#52-Blockchain)
  - [5.3 zkVM zkEVM](#53-zkVM-zkEVM)
  - [5.4 Privacy Authentication](#54-Privacy-Authentication)
  - [5.5 ZKML](#55-ZKML)
  - [5.6 Verifiable Computation](#56-verifiable-computation)

</details>

<details open>
<summary><strong>6. Other Resources</strong></summary>
  
  - [6.1 Text Resources](#61-Text-Resources)
  - [6.2 Video Resources](#62-Video-Resources)

</details>

<details open>
<summary><strong>7. Lookup Argument Related Papers Collection</strong></summary>

  - [7.1 Lookup Argument Papers](#71-Lookup-Argument-Papers)
  - [7.2 Lookup Argument Application Papers](#72-Lookup-Argument-Application-Papers)

</details>



---

## Foundation Knowledges of Lookup Arguments 
[⬆️ Back to Contents](#Contents)

### SumCheck
- [Multivariate Sum-Check Protocol](https://georgwiese.github.io/crypto-summaries/Concepts/Protocols/multivariate/Multivariate-Sum-Check-Protocol)
- [Univariate Sum-Check Protocol](https://georgwiese.github.io/crypto-summaries/Concepts/Protocols/univariate/Univariate-Sum-Check-Protocol)
### Polynomial Commitments
- [KZG](https://georgwiese.github.io/crypto-summaries/Concepts/Polynomial-Commitment-Schemes/KZG)
- [Spark](https://georgwiese.github.io/crypto-summaries/Concepts/Polynomial-Commitment-Schemes/Spark)
### Low Degree and Multilinear Extensions
- [Low Degree and Multilinear Extensions](https://georgwiese.github.io/crypto-summaries/Concepts/Fundamental-Concepts/Low-Degree-and-Multilinear-Extensions)
### Logarithmic Derivative
- [Logarithmic Derivative](https://building-babylon.net/2024/02/14/a-royal-road-to-logup/)
### Offline Memory Checking
- [Offline Memory Checking](https://georgwiese.github.io/crypto-summaries/Concepts/Protocols/Offline-Memory-Checking)
### Multiset Euqlity
- [Multiset Euqlity](https://georgwiese.github.io/crypto-summaries/Concepts/Protocols/Permutation-Check-via-Product-Check)
### GKR
- [protocol](https://georgwiese.github.io/crypto-summaries/Concepts/Protocols/multivariate/GKR)
## 1. Classification Based on Fundamental Mathematical Principles
[⬆️ Back to Contents](#Contents)
### 1.1 Based on multiset equality
Halo 2 lookup,      Plookup 
- [plookup: A simplified polynomial protocol for lookup tables](#plookup-A-simplified-polynomial-protocol-for-lookup-tables)
- [halo2](#halo2)
- [DUPLEX: Scalable Zero-Knowledge Lookup Arguments over RSA Group](#DUPLEX-Scalable-Zero-Knowledge-Lookup-Arguments-over-RSA-Group)

### 1.2 Based on memory checking
(spartan),     part of lasso
- [Spartan:Efficient and general-purpose zkSNARKs without trusted setup](#Spartan-Efficient-and-general-purpose-zkSNARKs-without-trusted-setup)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;CRYPTO 2020
- [Unlocking the lookup singularity with Lasso](#Unlocking-the-lookup-singularity-with-Lasso)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;EUROCRYPT 2024

  Lasso involves a well-formation check to guarantee the correctness of certain polynomials committed during the protocol. In Lasso, this is done by offline memory checking techniques from Spartan


- [Scalable Zero-knowledge Proofs for Non-linear Functions in Machine Learning](#Scalable-Zero-knowledge-Proofs-for-Non-linear-Functions-in-Machine-Learning)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;USENIX 2024
- [(zklasso)SNARKs for Virtual Machines are Non-Malleable](#zklasso-SNARKs-for-Virtual-Machines-are-Non-Malleable)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;EUROCRYPT 2025
- [TaSSLE: Lasso for the commitment-phobic](#TaSSLE-Lasso-for-the-commitment-phobic)&nbsp;&nbsp;&nbsp;&nbsp;eprint version 2024
  handle the well-formation check using logarithmic derivative techniques from [Logup](#Multivariate-lookups-based-on-logarithmic-derivatives-Logup) to cutting prover cost
- [Twist and Shout: Faster memory checking arguments via one-hot addressing and increments](#Twist-and-Shout-Faster-memory-checking-arguments-via-one-hot-addressing-and-increments)&nbsp;&nbsp;&nbsp;&nbsp;eprint version
### 1.3 Based on logarithmic derivatives
Logup, cq,
cq+   (Lookup Arguments: Improvements, Extensions and Applications to Zero-Knowledge Decision Trees)
Locq  (Efficient KZG-based Univariate Sum-check and Lookup Argument)
logup+GKR (Improving logarithmic derivative lookups using GKR)
μ-seek  (Natively Compatible Super-Efficient Lookup Arguments and How to Apply Them)
Tlookup  (zkLLM: Zero Knowledge Proofs for Large Language Models)
- [Multivariate lookups based on logarithmic derivatives(Logup)](#Multivariate-lookups-based-on-logarithmic-derivatives-Logup)&nbsp;&nbsp;&nbsp;&nbsp;eprint version
- [Bypassing the characteristic bound in logUp](#Bypassing-the-characteristic-bound-in-logUp)&nbsp;&nbsp;&nbsp;&nbsp;eprint version 2024

  describe how to bypass the characteristic bound in [Logup](#Multivariate-lookups-based-on-logarithmic-derivatives-Logup) by abstracting the notion of (pole) multiplicity. The method applies as well to the [Logup+GKR](#improving-logarithmic-derivative-lookups-using-gkr), and it moreover unlocks fractional decomposition lookups over binary fields.
  
- [cq: Cached quotients for fast lookups](#cq-cached-quotients-for-fast-lookups)
- [cq+ Lookup Arguments: Improvements, Extensions and Applications to Zero-Knowledge Decision Trees](#cq-lookup-arguments-improvements-extensions-and-applications-to-zero-knowledge-decision-trees)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;PKC 2024
- [Locq Efficient KZG-based Univariate Sum-check and Lookup Argument](#locq-efficient-kzg-based-univariate-sum-check-and-lookup-argument)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;PKC 2024
- [Improving logarithmic derivative lookups using GKR](#improving-logarithmic-derivative-lookups-using-gkr)

   inspired by [Lasso](#Unlocking-the-lookup-singularity-with-Lasso), GKR is introduced to further enhance Lookup performance. 
- [HyperPianist: Pianist with Linear-Time Prover and Logarithmic Communication Cost](#HyperPianist-Pianist-with-Linear-Time-Prover-and-Logarithmic-Communication-Cost)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;IEEE S&P 2025

  optimization builds on [Lasso](#Unlocking-the-lookup-singularity-with-Lasso). handle the well-formation check using logarithmic derivative techniques from [Logup](#Multivariate-lookups-based-on-logarithmic-derivatives-Logup) to cutting prover cost
- [Natively Compatible Super-Efficient Lookup Arguments and How to Apply Them](#natively-compatible-super-efficient-lookup-arguments-and-how-to-apply-them)
- [(Tlookup)zkLLM: Zero Knowledge Proofs for Large Language Models](#Tlookup-zkllm-zero-knowledge-proofs-for-large-language-models)&nbsp;&nbsp;&nbsp;&nbsp;CCS 2024  
- [MuxProofs: Succinct Arguments for Machine Computation from Vector Lookups](#muxproofs-succinct-arguments-for-machine-computation-from-vector-lookups)&nbsp;&nbsp;based on logup&nbsp;&nbsp;&nbsp;&nbsp;ASIACRYPT 2024
- [SublonK: Sublinear Prover PlonK](#sublonk-sublinear-prover-plonk)
- [Succinct Non-Subsequence Arguments](#succinct-non-subsequence-arguments)&nbsp;&nbsp;&nbsp;&nbsp;Non-Subsequence lookup&nbsp;&nbsp;&nbsp;&nbsp;SCN2024
- [Soloist: Distributed SNARKs for Rank-One Constraint System](#soloist-distributed-snarks-for-rank-one-constraint-system)&nbsp;&nbsp;&nbsp;&nbsp;eprint version&nbsp;&nbsp;&nbsp;&nbsp;distributed lookup based on logup
- [ProtoStar: Generic Efficient Accumulation/Folding for Special Sound Protocols](#protostar-generic-efficient-accumulationfolding-for-special-sound-protocols)&nbsp;&nbsp;&nbsp;&nbsp;ASIACRYPT 2023&nbsp;&nbsp;&nbsp;&nbsp;adapt logarithmic derivatives in folding
- [Proofs for Deep Thought: Accumulation for large memories and deterministic computations](#Proofs-for-Deep-Thought-Accumulation-for-large-memories-and-deterministic-computations)&nbsp;&nbsp;&nbsp;(mem-update)based on LogU&pnbsp;&nbsp;&pnbsp;&nbsp;&nbsp;&nbsp;ASIACRYPT 2024

### 1.4 Based on Matrix vector multiplication
Part of Lasso， Baloo，  FLI（FLI: Folding Lookup Instances）
- [FLI: Folding Lookup Instances](#fli-folding-lookup-instances)&nbsp;&nbsp;&nbsp;&nbsp;ASIACRYPT 2024
- [Baloo: Nearly Optimal Lookup Arguments](#baloo-nearly-optimal-lookup-arguments)
- [Unlocking the lookup singularity with Lasso](#Unlocking-the-lookup-singularity-with-Lasso)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;EUROCRYPT 2024

  main part is based on MVM, the well-formation check to guarantee the correctness of certain polynomials committed during the protocol is done by offline memory checking techniques from Spartan
- [HyperPianist: Pianist with Linear-Time Prover and Logarithmic Communication Cost](#HyperPianist-Pianist-with-Linear-Time-Prover-and-Logarithmic-Communication-Cost)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;IEEE S&P 2025

  optimization builds on [Lasso](#Unlocking-the-lookup-singularity-with-Lasso)，main part is based on MVM. handle the well-formation check using logarithmic derivative techniques from [Logup](#Multivariate-lookups-based-on-logarithmic-derivatives-Logup) to cutting prover cost
- [(zklasso)SNARKs for Virtual Machines are Non-Malleable](#zklasso-SNARKs-for-Virtual-Machines-are-Non-Malleable)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;EUROCRYPT 2025
- [TaSSLE: Lasso for the commitment-phobic](#TaSSLE-Lasso-for-the-commitment-phobic)&nbsp;&nbsp;&nbsp;&nbsp;eprint version

### 1.5 Based on vanishing polynomial
Based on vanishing polynomial：caulk，caulk+，flookup
"Batching-Efficient RAM using Updatable Lookup Argumentslookup" is based on Caulk+
- [Caulk: Lookup Arguments in Sublinear Time](#caulk-lookup-arguments-in-sublinear-time)&nbsp;&nbsp;&nbsp;&nbsp;CCS 2022
- [Caulk+: Table-independent lookup arguments](#caulk-table-independent-lookup-arguments)
- [flookup: Fractional decomposition-based_lookups_in_quasi-linear_time_independent_of_table_size](#flookup-fractional-decomposition-based_lookups_in_quasi-linear_time_independent_of_table_size)
- [Batching-Efficient RAM using Updatable Lookup Arguments](#batching-efficient-ram-using-updatable-lookup-arguments)&nbsp;&nbsp;&nbsp;&nbsp;CCS 2024

## 2. Classification Based on Lookup Objects
[⬆️ Back to Contents](#Contents)
### 2.1 Element Lookup
- [plookup: A simplified polynomial protocol for lookup tables](#plookup-A-simplified-polynomial-protocol-for-lookup-tables)
- [halo2](#halo2)

### 2.2 Vector lookup
- [Multivariate lookups based on logarithmic derivatives(Logup)](#Multivariate-lookups-based-on-logarithmic-derivatives-Logup)&nbsp;&nbsp;&nbsp;&nbsp;eprint version
- [MuxProofs: Succinct Arguments for Machine Computation from Vector Lookups](#muxproofs-succinct-arguments-for-machine-computation-from-vector-lookups)
### 2.3 Matrix lookup
- [cq+ Lookup Arguments: Improvements, Extensions and Applications to Zero-Knowledge Decision Trees](#cq-lookup-arguments-improvements-extensions-and-applications-to-zero-knowledge-decision-trees)


## 3. Classification Based on Zero-Knowledge Property
[⬆️ Back to Contents](#Contents)
### 3.1 Non-Zero-Knowledge
- [plookup: A simplified polynomial protocol for lookup tables](#plookup-A-simplified-polynomial-protocol-for-lookup-tables)
- [halo2](#halo2)
- [flookup: Fractional decomposition-based_lookups_in_quasi-linear_time_independent_of_table_size](#flookup-fractional-decomposition-based_lookups_in_quasi-linear_time_independent_of_table_size)
- [Multivariate lookups based on logarithmic derivatives(Logup)](#Multivariate-lookups-based-on-logarithmic-derivatives-Logup)&nbsp;&nbsp;&nbsp;&nbsp;eprint version
- [Baloo: Nearly Optimal Lookup Arguments](#baloo-nearly-optimal-lookup-arguments)
- [cq: Cached quotients for fast lookups](#cq-cached-quotients-for-fast-lookups)

### 3.2 Partial Zero-Knowledge
- [cq+ Lookup Arguments: Improvements, Extensions and Applications to Zero-Knowledge Decision Trees](#cq-lookup-arguments-improvements-extensions-and-applications-to-zero-knowledge-decision-trees)


### 3.3 Fully Zero-Knowledge
- [Caulk: Lookup Arguments in Sublinear Time](#caulk-lookup-arguments-in-sublinear-time)
- [Caulk+: Table-independent lookup arguments](#caulk-table-independent-lookup-arguments)
- [zkcq+ Lookup Arguments: Improvements, Extensions and Applications to Zero-Knowledge Decision Trees](#cq-lookup-arguments-improvements-extensions-and-applications-to-zero-knowledge-decision-trees)
- [Locq Efficient KZG-based Univariate Sum-check and Lookup Argument](#locq-efficient-kzg-based-univariate-sum-check-and-lookup-argument)
- [(zklasso)SNARKs for Virtual Machines are Non-Malleable](#zklasso-SNARKs-for-Virtual-Machines-are-Non-Malleable)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;EUROCRYPT 2025
- [DUPLEX: Scalable Zero-Knowledge Lookup Arguments over RSA Group](#DUPLEX-Scalable-Zero-Knowledge-Lookup-Arguments-over-RSA-Group)


## 4. Classification Based on Preprocessing and Updatability
[⬆️ Back to Contents](#Contents)
### 4.1 Need preprocessing_Non-Updatable
- [Multivariate lookups based on logarithmic derivatives(Logup)](#Multivariate-lookups-based-on-logarithmic-derivatives-Logup)&nbsp;&nbsp;&nbsp;&nbsp;eprint version
- [cq: Cached quotients for fast lookups](#cq-cached-quotients-for-fast-lookups)
- [cq+ Lookup Arguments: Improvements, Extensions and Applications to Zero-Knowledge Decision Trees](#cq-lookup-arguments-improvements-extensions-and-applications-to-zero-knowledge-decision-trees)
- [Locq Efficient KZG-based Univariate Sum-check and Lookup Argument](#locq-efficient-kzg-based-univariate-sum-check-and-lookup-argument)
- [Improving logarithmic derivative lookups using GKR](#improving-logarithmic-derivative-lookups-using-gkr)
- [Baloo: Nearly Optimal Lookup Arguments](#baloo-nearly-optimal-lookup-arguments)
- [Unlocking the lookup singularity with Lasso](#Unlocking-the-lookup-singularity-with-Lasso)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;EUROCRYPT 2024
- [Caulk: Lookup Arguments in Sublinear Time](#caulk-lookup-arguments-in-sublinear-time)
- [Caulk+: Table-independent lookup arguments](#caulk-table-independent-lookup-arguments)
- [flookup: Fractional decomposition-based_lookups_in_quasi-linear_time_independent_of_table_size](#flookup-fractional-decomposition-based_lookups_in_quasi-linear_time_independent_of_table_size)



### 4.2 No preprocessing_Updatable
- [plookup: A simplified polynomial protocol for lookup tables](#plookup-A-simplified-polynomial-protocol-for-lookup-tables)
- [halo2](#halo2)

### 4.3 Need preprocessing_Updatable
- [Batching-Efficient RAM using Updatable Lookup Arguments](#batching-efficient-ram-using-updatable-lookup-arguments)
- [DUPLEX: Scalable Zero-Knowledge Lookup Arguments over RSA Group](#DUPLEX-Scalable-Zero-Knowledge-Lookup-Arguments-over-RSA-Group)

## 5. Applications of Lookup Arguments
[⬆️ Back to Contents](#Contents)
### 5.1 zk-SNARK
- [BabySpartan: Lasso-based SNARK for non-uniform computation](#BabySpartan-Lasso-based-SNARK-for-non-uniform-computation)
- [Samaritan: Linear-time Prover SNARK from New Multilinear Polynomial Commitments](#Samaritan-Linear-time-Prover-SNARK-from-New-Multilinear-Polynomial-Commitments)&nbsp;&nbsp;&nbsp;&nbsp;eprint version 202503

  introduces LogSpartan PIOP that uses a lookup argument based on logarithmic derivatives of polynomials [LogUp](#Multivariate-lookups-based-on-logarithmic-derivatives-Logup) and reduces the proof size of the Spartan PIOP from O(log2 n) to O(log n) while retaining the same prover efficiency.
- [Zinc: Succinct Arguments with Small Arithmetization Overheads from IOPs of Proximity to the Integers](#Zinc-Succinct-Arguments-with-Small-Arithmetization-Overheads-from-IOPs-of-Proximity-to-the-Integers)&nbsp;&nbsp;&nbsp;&nbsp;eprint version 202502

  one can use a lookup argument over the rationals to ensure that the witness contains only integer elements.
- [On the Power of Polynomial Preprocessing: Proving Computations in Sublinear Time, and More](https://eprint.iacr.org/2025/238.pdf)&nbsp;&nbsp;&nbsp;&nbsp;eprint version 202502

  based on Lasso. yields the first lookup argument for unstructured tables in which the prover is sublinear in the size of the table, while making only black-box use of a VC and thus allowing instantiations from generic assumptions such as collision-resistant hash functions. Prior lookup arguments with sublinear provers were only known with non-black-box use of cryptographic primitives, or from pairings. 
### 5.2 Blockchain
  blockchain scable zkrollup cross-chain bridge
- [Cross-chain bridges via backwards-compatible SNARKs](#Cross-chain-bridges-via-backwards-compatible-SNARKs)


### 5.3 zkVM zkEVM
  Express logical operations, memory consistency checking, and control flow structures at a low constraint cost（e.g. XOR, AND, range）
  Memory models and lookup arguments play a role in defining how memory is accessed and verified.
- [Jolt: SNARKs for Virtual Machines via Lookups](#Jolt-SNARKs-for-Virtual-Machines-via-Lookups)
- [Proving CPU Executions in Small Space](#Proving-CPU-Executions-in-Small-Space)
- [ZKWASM: A ZKSNARK WASM Emulator](#ZKWASM-A-ZKSNARK-WASM-Emulator)
- [Two Shuffles Make a RAM: Improved Constant Overhead Zero Knowledge RAM](#Two-Shuffles-Make-a-RAM-Improved-Constant-Overhead-Zero-Knowledge-RAM)
- [Zero Knowledge Memory-Checking Techniques for Stacks and Queues](#Zero-Knowledge-Memory-Checking-Techniques-for-Stacks-and-Queues)
- [Nebula: Efficient read-write memory and switchboard circuits for folding schemes](#Nebula-Efficient-read-write-memory-and-switchboard-circuits-for-folding-schemes)
- [Polynomial IOPs for Memory Consistency Checks in Zero-Knowledge Virtual Machines](#Polynomial-IOPs-for-Memory-Consistency-Checks-in-Zero-Knowledge-Virtual-Machines)

- [scroll zkEVM](#scroll-zkEVM)
- [zksync zkEVM](#zksync-zkEVM)
- [polygon zkEVM](#polygon-zkEVM)
  LogUp is crucial for performance in the Polygon ZKEVM, where they need to split the whole table into several STARK modules. These modules have to be linked correctly, and cross-table lookups enforce this.
### 5.4 Privacy Authentication
  zkDID zkLogin

- [zkLogin: Privacy-Preserving Blockchain Authentication with Existing Credentials](#zkLogin-Privacy-Preserving-Blockchain-Authentication-with-Existing-Credentials)
### 5.5 ZKML
  Efficiently verify nonlinear calculations in neural networks using lookup argument
- [ZKML: An Optimizing System for ML Inference in Zero-Knowledge Proofs](#ZKML-An-Optimizing-System-for-ML-Inference-in-Zero-Knowledge-Proofs)
- [Scalable Zero-knowledge Proofs for Non-linear Functions in Machine Learning](#Scalable-Zero-knowledge-Proofs-for-Non-linear-Functions-in-Machine-Learning)
- [zkLLM: Zero Knowledge Proofs for Large Language Models](#zkLLM-Zero-Knowledge-Proofs-for-Large-Language-Models)
- [An Efficient and Extensible Zero-knowledge Proof Framework for Neural Networks](#An-Efficient-and-Extensible-Zero-knowledge-Proof-Framework-for-Neural-Networks)
- [Scaling up Trustless DNN Inference with Zero-Knowledge Proofs](#Scaling-up-Trustless-DNN-Inference-with-Zero-Knowledge-Proofs)
- [zkPyTorch: A Hierarchical Optimized Compiler for Zero-Knowledge Machine Learning](#zkPyTorch-A-Hierarchical-Optimized-Compiler-for-Zero-Knowledge-Machine-Learning)

### 5.6 Verifiable Computation
zkDatabase zcash 


## 6. Other Resources
[⬆️ Back to Contents](#Contents)
### 6.1 Text Resources
- [A brief history of lookup arguments](https://github.com/ingonyama-zk/papers/blob/main/lookups.pdf)
- [Lookup review blog](https://eigenlab.medium.com/a-review-of-lookup-arguments-edecf6aa73cb)
- [An Overview of SNARKs Including Lookup](https://www.alpenlabs.io/blog/current-state-of-snarks)
### 6.2 Video Resources

## 7. Lookup Argument Related Papers Collection
[⬆️ Back to Contents](#Contents)
### 7.1 Lookup Argument Papers

#### plookup: A simplified polynomial protocol for lookup tables
  - [eprint version](https://eprint.iacr.org/2020/315.pdf)
  - [note by GuoYu](https://github.com/sec-bit/learning-zkp/blob/master/plonk-intro-zh/7-plonk-lookup.md)
  - [note by Ariel Gabizon](https://hackmd.io/@relgabizon/ByFgSDA7D)
  - [slides](https://aztec.slides.com/suyashbagad_aztec/plookup-and-plonk#/2/0/16)
  - [video](https://www.youtube.com/watch?v=Vdlc1CmRYRY)
  - [implementation](https://github.com/kevaundray/plookup)

#### halo2
  - [halo2 book](https://zcash.github.io/halo2/design/proving-system/lookup.html)
  - [note by GuoYu](https://github.com/sec-bit/learning-zkp/blob/master/plonk-intro-zh/7-plonk-lookup.md)
  - [video](https://www.youtube.com/watch?v=3ie2yZ7CT5A)
  - [implementation](https://github.com/DoHoonKim8/halo2-lasso)

#### DUPLEX: Scalable Zero-Knowledge Lookup Arguments over RSA Group
  - [eprint version](https://eprint.iacr.org/2024/1509.pdf)

#### Spartan: Efficient and general-purpose zkSNARKs without trusted setup
  - [full version](https://eprint.iacr.org/2019/550.pdf)&nbsp;&nbsp;&nbsp;&nbsp;CRYPTO 2020
  - [conference version](https://link.springer.com/content/pdf/10.1007/978-3-030-56877-1_25.pdf)
  - [slides](https://iacr.org/submit/files/slides/2020/crypto/crypto2020/304/slides.pptx)
  - [video](https://www.youtube.com/watch?v=FPQs7T7f_AU)
  - [implementation](https://github.com/microsoft/Spartan)

#### Unlocking the Lookup Singularity with Lasso
  - [full version](https://eprint.iacr.org/2023/1216.pdf)&nbsp;&nbsp;&nbsp;&nbsp;EUROCRYPT 2024
  - [conference version](https://link.springer.com/content/pdf/10.1007/978-3-031-58751-1_7)
  - [note by GuoYu](https://github.com/sec-bit/learning-zkp/tree/master/lookup-arguments/lasso-zh)
  - [video](https://youtu.be/_WsCQc9Elcg)
  - [slides](https://iacr.org/submit/files/slides/2024/eurocrypt/eurocrypt2024/346/slides.pptx)
  - [implementation](https://github.com/zkp-learning/Lasso)

#### HyperPianist: Pianist with Linear-Time Prover and Logarithmic Communication Cost
  - [full version](https://eprint.iacr.org/2024/1273.pdf)

#### Scalable Zero-knowledge Proofs for Non-linear Functions in Machine Learning
  - [full version](https://eprint.iacr.org/2025/507.pdf)&nbsp;&nbsp;&nbsp;&nbsp;USENIX 2024
  - [conference version](https://www.usenix.org/system/files/usenixsecurity24-hao-meng-scalable.pdf)
  - [video](https://youtu.be/OXOcq4avvP8)
  - [slides](https://www.usenix.org/system/files/usenixsecurity24_slides-hao-meng-scalable.pdf)
  - [implementation](https://github.com/CryptMatrix/ZKMath)

#### (zklasso) SNARKs for Virtual Machines are Non-Malleable
  - [full version](https://eprint.iacr.org/2024/1551.pdf)&nbsp;&nbsp;&nbsp;&nbsp;EUROCRYPT 2025
  - [conference version](https://hal.science/hal-04991788v1/file/publi-8049.pdf)
  - [video](https://www.youtube.com/watch?v=gPV0T9YIrH4)

#### TaSSLE: Lasso for the commitment-phobic
  - [eprint version](https://eprint.iacr.org/2024/1075.pdf)
  - [blog](https://www.lita.foundation/blog/tassle-tensors-and-sumcheck-for-structured-lookup-efficiency)

#### Twist and Shout: Faster memory checking arguments via one-hot addressing and increments
  - [eprint version](https://eprint.iacr.org/2025/105.pdf)

#### Multivariate lookups based on logarithmic derivatives (Logup)
  - [eprint version](https://eprint.iacr.org/2022/1530.pdf)
  - [notes 1](https://georgwiese.github.io/crypto-summaries/Concepts/Protocols/Lookup-Arguments/LogUp--and--cq)
  - [notes 2](https://blog.csdn.net/mutourend/article/details/127745883)
  - [video](https://www.youtube.com/watch?v=qv_5dF2_C4g)
  - [implementation](https://github.com/yugocabrio/oreno-lookup)

#### Bypassing the characteristic bound in logUp
  - [eprint version](https://eprint.iacr.org/2024/2067.pdf)

#### cq: Cached quotients for fast lookups
  - [eprint version](https://eprint.iacr.org/2022/1763.pdf)
  - [notes](https://georgwiese.github.io/crypto-summaries/Concepts/Protocols/Lookup-Arguments/LogUp--and--cq)
  - [slides](https://aztec.slides.com/suyashbagad_aztec/cq-lookup)
  - [video 1](https://www.youtube.com/watch?v=HJPOfkBcldE&t=357s)
  - [video 2](https://youtu.be/KQi3WdZvI6w)
  - [implementation](https://github.com/geometryxyz/cq)

#### cq+ Lookup Arguments: Improvements, Extensions and Applications to Zero-Knowledge Decision Trees
  - [full version](https://eprint.iacr.org/2023/1518.pdf)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;PKC 2024
  - [conference version](https://link.springer.com/content/pdf/10.1007/978-3-031-57722-2_11.pdf)
  - [slides](https://iacr.org/submit/files/slides/2024/pkc/pkc2024/48/slides.pdf)

#### Locq Efficient KZG-based Univariate Sum-check and Lookup Argument
  - [full version](https://eprint.iacr.org/2024/618.pdf)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;PKC 2024
  - [conference version](https://link.springer.com/content/pdf/10.1007/978-3-031-57722-2_13.pdf?pdf=inline%20link)
  - [slides](https://iacr.org/submit/files/slides/2024/pkc/pkc2024/99/slides.pdf)

#### Improving logarithmic derivative lookups using GKR
  - [eprint version](https://eprint.iacr.org/2023/1284.pdf)
  - [video](https://www.youtube.com/watch?v=DCEg61ExwK4&t=139s)
  - [blog](https://blog.kroma.network/from-halo2-lookup-logup-to-logup-gkr-4af3bf143d38)

#### Natively Compatible Super-Efficient Lookup Arguments and How to Apply Them
- [full version](https://eprint.iacr.org/2024/1058.pdf)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;JOC 2024
  - [journal version](https://link.springer.com/content/pdf/10.1007/s00145-024-09535-0.pdf)
  - [video](https://www.youtube.com/watch?v=eRKn5uFK0V0)

#### (Tlookup)zkLLM: Zero Knowledge Proofs for Large Language Models
  - [full version](https://arxiv.org/pdf/2404.16109)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;CCS 2024  
  - [conference version](https://dl.acm.org/doi/pdf/10.1145/3658644.3670334)
  - [implementation](https://github.com/jvhs0706/zkllm-ccs2024)

#### MuxProofs: Succinct Arguments for Machine Computation from Vector Lookups
  - [full version](https://eprint.iacr.org/2023/974.pdf)&nbsp;&nbsp;&nbsp;&nbsp;based on logup&nbsp;&nbsp;&nbsp;&nbsp;ASIACRYPT 2024
  - [conference version](https://link.springer.com/chapter/10.1007/978-981-96-0935-2_8)
  - [slides](https://iacr.org/submit/files/slides/2024/asiacrypt/asiacrypt2024/313/313_slides.pdf)
  - [implementation](https://github.com/lucasxia01/mux-proofs-impl)

#### SublonK: Sublinear Prover PlonK
  - [eprint version](https://eprint.iacr.org/2023/902.pdf)
  - [implementation](https://github.com/txaty/ark-segmentlookup)

#### Succinct Non-Subsequence Arguments
  - [full version](https://eprint.iacr.org/2024/1264.pdf)&nbsp;&nbsp;&nbsp;&nbsp;Non-Subsequence lookup&nbsp;&nbsp;&nbsp;&nbsp;SCN2024
  - [conference version](https://link.springer.com/content/pdf/10.1007/978-3-031-71070-4_2.pdf?pdf=inline%20link)

#### Soloist: Distributed SNARKs for Rank-One Constraint System
  - [eprint version](https://eprint.iacr.org/2025/557.pdf)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;distributed lookup based on logup

#### ProtoStar: Generic Efficient Accumulation/Folding for Special Sound Protocols
  - [full version](https://eprint.iacr.org/2023/620.pdf)&nbsp;&nbsp;&nbsp;&nbsp;ASIACRYPT 2023&nbsp;&nbsp;&nbsp;&nbsp;adapt logarithmic derivatives in folding
  - [conference version](https://link.springer.com/content/pdf/10.1007/978-981-99-8724-5_3.pdf?pdf=inline%20link)
  - [video](https://www.youtube.com/watch?v=wtxVYiZh7zc)
  - [slides](https://iacr.org/submit/files/slides/2023/asiacrypt/asiacrypt2023/84/slides.pptx)
  - [implementation](https://github.com/geometryxyz/protostar)

#### Proofs for Deep Thought: Accumulation for large memories and deterministic computations
  - [full version](https://eprint.iacr.org/2024/325.pdf)&pnbsp;&nbsp;&nbsp;&nbsp;ASIACRYPT 2024
  - [conference version](https://link.springer.com/content/pdf/10.1007/978-981-96-0935-2_9.pdf?pdf=inline%20link)
  - [slides](https://iacr.org/submit/files/slides/2024/asiacrypt/asiacrypt2024/16/16_slides.pptx)

#### FLI: Folding Lookup Instances
  - [full version](https://eprint.iacr.org/2024/1531.pdf)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ASIACRYPT 2024
  - [conference version](https://link.springer.com/chapter/10.1007/978-981-96-0935-2_13)
  - [slides](https://iacr.org/submit/files/slides/2024/asiacrypt/asiacrypt2024/197/197_slides.pdf)

#### Baloo: Nearly Optimal Lookup Arguments
  - [eprint version](https://eprint.iacr.org/2022/1565.pdf)
  - [notes](https://github.com/sec-bit/learning-zkp/tree/master/lookup-arguments/baloo-en)
  - [implementation](https://github.com/geometryxyz/baloo?tab=readme-ov-file)

#### Caulk: Lookup Arguments in Sublinear Time
  - [full version](https://eprint.iacr.org/2022/621.pdf)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;CCS 2022
  - [conference version](https://dl.acm.org/doi/pdf/10.1145/3548606.3560646)
  - [notes](https://asdavinci.ing/post/caulk-caulk+note/)
  - [slides](https://www.slideshare.net/AlexPruden/caulk-zkstudyclub-caulk-lookup-arguments-in-sublinear-time-a-zapico?from_search=0)
  - [video](https://www.youtube.com/watch?v=uEssF2WzIeU)
  - [implementation](https://github.com/caulk-crypto/caulk)

#### Caulk+: Table-independent lookup arguments
  - [eprint version](https://eprint.iacr.org/2022/957.pdf)
  - [notes](https://asdavinci.ing/post/caulk-caulk+note/)
  - [implementation](https://github.com/CPerezz/caulk_plus)

#### flookup: Fractional decomposition-based lookups in quasi-linear time independent of table size
  - [eprint version](https://eprint.iacr.org/2022/1447.pdf)

#### Batching-Efficient RAM using Updatable Lookup Arguments
  - [full version](https://eprint.iacr.org/2024/840.pdf)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;CCS 2024
  - [conference version](https://dl.acm.org/doi/pdf/10.1145/3658644.3670356)

### 7.2 Lookup Argument Application Papers
[⬆️ Back to Contents](#Contents)
#### BabySpartan: Lasso-based SNARK for non-uniform computation
  - [eprint version](https://eprint.iacr.org/2023/1799.pdf)

#### Samaritan: Linear-time Prover SNARK from New Multilinear Polynomial Commitments
  - [eprint version](https://eprint.iacr.org/2025/419.pdf)

#### On the Power of Polynomial Preprocessing: Proving Computations in Sublinear Time, and More
  - [eprint version](https://eprint.iacr.org/2025/238.pdf)

#### Cross-chain bridges via backwards-compatible SNARKs
  - [eprint version](https://eprint.iacr.org/2024/995.pdf)&nbsp;&nbsp;uses cq lookup&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;

#### Jolt: SNARKs for Virtual Machines via Lookups
  - [full version](https://eprint.iacr.org/2023/1217)&nbsp;&nbsp;&nbsp;&nbsp;uses Lasso&nbsp;&nbsp;EUROCRYPT 2024
  - [conference version](https://link.springer.com/content/pdf/10.1007/978-3-031-58751-1_1.pdf?pdf=inline%20link)
  - [slides](https://iacr.org/submit/files/slides/2024/eurocrypt/eurocrypt2024/297/slides.pdf)
  - [video](https://www.youtube.com/watch?v=ebN-mt-P-Qw)
  - [implementation](https://github.com/a16z/jolt)

#### Proving CPU Executions in Small Space
  - [eprint version](https://eprint.iacr.org/2025/611.pdf)

#### ZKWASM: A ZKSNARK WASM Emulator
  - [full version](https://ieeexplore.ieee.org/document/10587123)
  - [implementation](https://github.com/CPerezz/caulk_plus)

#### Two Shuffles Make a RAM: Improved Constant Overhead Zero Knowledge RAM
  - [full version](https://eprint.iacr.org/2023/1115.pdf)&nbsp;&nbsp;&nbsp;&nbsp;USENIX 2024
  - [conference version](https://www.usenix.org/system/files/sec24summer-prepub-208-yang-yibin.pdf)
  - [implementation](https://github.com/gconeice/improved-zk-ram)
#### Zero Knowledge Memory-Checking Techniques for Stacks and Queues
  - [eprint version](https://eprint.iacr.org/2024/2084.pdf)

#### Nebula: Efficient read-write memory and switchboard circuits for folding schemes
  - [eprint version](https://eprint.iacr.org/2024/1605.pdf)&nbsp;&nbsp;&nbsp;&nbsp;based on Lasso

#### Polynomial IOPs for Memory Consistency Checks in Zero-Knowledge Virtual Machines
  - [full version](https://eprint.iacr.org/2023/1555.pdf)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ASIACRYPT 2024
  - [conference version](https://link.springer.com/content/pdf/10.1007/978-981-99-8724-5_4.pdf?pdf=inline%20link)
  - [slides](https://iacr.org/submit/files/slides/2023/asiacrypt/asiacrypt2023/344/slides.pdf)
#### scroll zkEVM
  - [scroll zkEVM](https://www.slideshare.net/slideshow/zkevm-circuit-arithmetization-by-ye-zhang/267299055)

#### zksync zkEVM
  - [zksync zkEVM](https://docs.zksync.io/zksync-protocol/circuits/zk-terminology)

#### polygon zkEVM
  - [polygon zkEVM](https://docs.polygon.technology/zkEVM/architecture/proving-system/secondary-sms-lookup-tables/?h=lookup)

#### zkLogin: Privacy-Preserving Blockchain Authentication with Existing Credentials
  - [full version](https://arxiv.org/pdf/2401.11735)
  - [conference version](https://dl.acm.org/doi/pdf/10.1145/3658644.3690356)
  - [slides](https://mahdi171.github.io/files/zkLogin_O1Labs.pdf)

#### ZKML: An Optimizing System for ML Inference in Zero-Knowledge Proofs
  - [conference version](https://dl.acm.org/doi/pdf/10.1145/3627703.3650088)&nbsp;&nbsp;&nbsp;uses halo2 lookup&nbsp;&nbsp;&nbsp;EuroSys 2024

#### Scalable Zero-knowledge Proofs for Non-linear Functions in Machine Learning
  - [full version](https://www.usenix.org/system/files/usenixsecurity24-hao-meng-scalable.pdf)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;USENIX 2024
  - [video](https://youtu.be/OXOcq4avvP8)
  - [slides](https://www.usenix.org/system/files/usenixsecurity24_slides-hao-meng-scalable.pdf)
  - [implementation](https://github.com/CryptMatrix/ZKMath)

#### zkLLM: Zero Knowledge Proofs for Large Language Models
  - [full version](https://arxiv.org/pdf/2404.16109)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;CCS 2024  
  - [conference version](https://dl.acm.org/doi/pdf/10.1145/3658644.3670334)
  - [implementation](https://github.com/jvhs0706/zkllm-ccs2024)

#### An Efficient and Extensible Zero-knowledge Proof Framework for Neural Networks
  - [eprint version](https://eprint.iacr.org/2024/703.pdf)

#### Scaling up Trustless DNN Inference with Zero-Knowledge Proofs
  - [eprint version](https://arxiv.org/abs/2210.08674)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;uses halo2 lookupn
  - [video](https://www.youtube.com/watch?v=Co5gNoHnMhs)

#### zkPyTorch: A Hierarchical Optimized Compiler for Zero-Knowledge Machine Learning
  - [eprint version](https://eprint.iacr.org/2025/535.pdf)


[⬆️ Back to Contents](#Contents)
