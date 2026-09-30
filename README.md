# Efficient Representation Learning for Heterogeneous Systems and Continual Task Adaptation

**SC26 Doctoral Showcase**

**Fatema Siddika** (PhD Candidate) and **Ali Jannesari** (PhD Advisor)
Department of Computer Science, Iowa State University

Collaborators: Md Anwar Hossen¹, Wensheng Zhang¹, Anuj Sharma¹, Tanwi Mallick², Ravi Madduri², Zilinghan Li², J. Pablo Muñoz³, Tanya Roosta⁴

¹Iowa State University ²Argonne National Laboratory ³Intel Labs ⁴UC Berkeley / Amazon / AMD

---

## Abstract

This dissertation addresses two fundamental challenges in distributed machine learning: client heterogeneity and continual adaptation to new tasks. It develops efficient fine-tuning and representation-learning frameworks that let distributed models acquire new knowledge and align it across clients without communication bottlenecks or catastrophic forgetting.

First, we introduce a dual-distilled federated learning framework for clients with heterogeneous systems and data. Trainable global prototypes with adaptive margins align local representations and logits without requiring a shared model architecture, enabling robust knowledge transfer and stable convergence.

Next, we propose a communication-efficient federated framework for large language models (LLMs) based on representation fine-tuning. By intervening on hidden states rather than weights, and combining All-But-Me aggregation with dynamic test-time computing, it reduces communication cost while balancing local personalization and global generalization.

We then present SETA, a mixture of sparse experts for task-agnostic continual learning in LLMs. SETA resolves the plasticity–stability dilemma by structurally decomposing the parameter space into shared and task-specific experts, protecting shared knowledge from semantic drift while preserving task-specific features.

Finally, we introduce FedSEAM, which extends sparse experts to federated continual learning. Clients learn experts on private task streams, and the server merges them through subspace agreement: it combines only the update directions clients share, keeps disagreeing directions as client-private experts, and protects prior-task subspaces from being overwritten.

Together, these contributions chart a path toward scalable, resource-aware machine learning systems that bridge decentralized efficiency and continual real-world deployment, learning new tasks across privacy-constrained environments without forgetting.


## Publications

1. **FedReFT:** Federated Representation Fine-Tuning with All-But-Me Aggregation. *EACL 2026.*
2. **FedProtoKD:** Dual-Distilled Heterogeneous FL with Adaptive Margins for Trainable Global Prototypes. *IEEE CCGrid 2026.*
3. **SETA:** Split-on-Share: Mixture of Sparse Experts for Task-Agnostic Continual Learning. *Under review.*
4. **FedSEAM:** Federated Continual Learning of LLMs via Subspace Expert Agreement Merging. *Under review.*



## Links

- SwAPP Lab: https://github.com/swapp-lab

## Acknowledgments

Joint work with Md Anwar Hossen (equal contribution on FedReFT), Ali Jannesari (advisor, Iowa State University), Wensheng Zhang and Anuj Sharma (Iowa State University), Tanwi Mallick (Argonne National Laboratory), J. Pablo Muñoz (Intel Labs), and Tanya Roosta (UC Berkeley / Amazon / AMD). FedSEAM is joint work with Ravi Madduri and Zilinghan Li (Argonne National Laboratory).


