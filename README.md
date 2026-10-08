# RCL-GCN-MO

**Integrating Relational Contrastive Learning with Graph Convolutional Networks for Cross-Omic Prediction and Cross-Omics Information Enrichment in Multi-Omics Data Integration**

---

## Overview

RCL-GCN-MO is a framework for multi-omics data integration that combines Graph Convolutional Networks (GCNs) with a Relational Contrastive Learning objective. The key innovation is a contrastive loss that preserves the **relational structure** between patient embeddings across omics layers, enabling both **cross-omic prediction** and **cross-omics information enrichment**.

The framework addresses a critical gap in existing multi-omics integration methods: most approaches learn each omics layer independently and fuse them at the end, losing cross-omic information. RCL-GCN-MO captures this information by aligning pairwise patient relationships across modalities during representation learning.

---

## Key Contributions

- **Relational Contrastive Learning (RCL)**: A novel contrastive loss that aligns difference vectors (pairwise patient relationships) across omics layers, preserving cross-omic relational structure
- **Cross-Omic Prediction**: Enables prediction of one omics layer from others by exploiting learned relational alignment
- **Cross-Omics Information Enrichment**: Each omics layer gains complementary information from other layers, reducing uncertainty and improving downstream performance
- **Multi-Omics Integration**: Handles four omics layers: CNA, Methylation, mRNA, and RPPA
- **Consistent Improvements**: Outperforms state-of-the-art baselines on 8 TCGA cancer datasets

