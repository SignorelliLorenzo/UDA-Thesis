# Thesis Repository: Pseudo-Label Refinement for Unsupervised Domain Adaptation in Semantic Segmentation **USING SAM**

This repository hosts the final documents for my **Bachelor thesis**, where I overhauled the pipeline originally developed by Jonas Frey and integrated the **Segment Anything Model (SAM)** into the semantic segmentation and 3D mapping process. The core contribution is the use of SAM to refine pseudo-labels, improving domain adaptation performance without requiring manual annotations.

---

## Abstract

In the field of robotic visual perception, understanding complex indoor environments remains a fundamental challenge. Semantic segmentation—assigning a class label to each pixel in an image—is essential for enabling fine-grained perception, necessary for tasks such as autonomous navigation and manipulation in cluttered indoor scenes.

However, modern semantic segmentation models often fail to generalize across different environments due to **domain shift**: a mismatch between training data and deployment settings. This severely limits robotic adaptability in unfamiliar spaces. To address this, this thesis proposes a method for **unsupervised domain adaptation (UDA)** by improving the quality of pseudo-labels—automatically generated labels used in place of human annotations.

The proposed system enhances a 3D mapping pipeline built on the Kimera framework, integrating voxel-based semantic predictions with a refinement stage powered by the **Segment Anything Model (SAM)**. Two prompting strategies are introduced—object-centric and grid-based—to guide SAM in generating accurate segmentation masks. These are fused with the original pseudo-labels to improve semantic consistency and boundary accuracy.

Experiments on unseen indoor scenes from the ScanNet dataset show that SAM-refined pseudo-labels outperform original voxel-based labels, especially in low-resolution mesh settings. This refinement improves model supervision with zero manual annotation, showing promise for scalable and cost-effective deployment of adaptable robots.

The approach lays the groundwork for future work in continual domain adaptation, where robots could update their understanding of the world over time without retraining from scratch.

---

## Documents

- 📄 [`thesis.pdf`](./thesis.pdf) — Full thesis document  
- 📄 [`summary.pdf`](./summary.pdf) — Thesis summary

---


