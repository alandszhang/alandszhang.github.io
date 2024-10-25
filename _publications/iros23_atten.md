---
title: "Training-free attentive-patch selection for visual place recognition"
collection: publications
category: conferences
permalink: /publication/iros23_atten
date: 2023-10-01
venue: 'IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)'
paperurl: 'https://dr.ntu.edu.sg/bitstream/10356/178533/2/IROS_23____Training_Free_Attentive_Patch_Selection_for_Visual_Place_Recognition.pdf'
citation: 'Zhang, D., Wu, M. & Lam, S. (2023). &quot;Training-free attentive-patch selection for visual place recognition.&quot; <i>2023 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)</i>. 9169‑9174.'
---

Visual Place Recognition (VPR) utilizing patch descriptors from Convolutional Neural Networks (CNNs) has shown impressive performance in recent years. Existing works either perform exhaustive matching of all patch descriptors, or employ complex networks to select good candidate patches for further geometric verification. In this work, we develop a novel two-step training-free patch selection method that is fast, while being robust to large occlusions and extreme viewpoint variations. In the first step, a self-attention mechanism is used to select sparse and evenly distributed discriminative patches in the query image. Next, a novel spatial-matching method is used to rapidly select corresponding patches with high similar appearances between the query and each reference image. The proposed method is inspired by how humans perform place recognition by first identifying prominent regions in the query image, and then relying on back-and-forth visual inspection of the query and reference image to attentively identify similar regions while ignoring dissimilar ones. Extensive experiment results show that our proposed method outperforms state-of-the-art (SOTA) methods in both place recognition precision and runtime, on various challenging conditions.
