# CGPRNet: Cross-Scale Graph Prototype Refinement for Robust Few-Shot Semantic Segmentation
# Introduction
Few-shot semantic segmentation (FSS) learns to segment novel classes with only a few annotated support images. Despite the promising results of recent methods, there remain three critical limitations: (1) current FSS methods do not explicitly model the cross-scale semantic dependencies between support and query; (2) they generate prototypes by simple embedding statistics while disregarding the progressive refinement ability of graph; (3) they fuse the multi-scale information in a principled manner. To address these challenges, we propose CGPR, a Cross-Scale Graph Prototype Refinement framework that explicitly models cross-scale dependencies by iteratively refining prototypes with graph neural networks. Concretely, we design a Cross-Attention Graph Prototype Generator to iteratively refine the prototypes by aggregating the cross-scale support-query relationships, and a Multi-Scale Prototype Matching module to compute the similarity at different receptive fields in an adaptive way. Additionally, we introduce a dual-branch feature encoder with frozen generic features and trainable task-specific features to prevent overfitting while maintaining discriminative power. We conduct extensive experiments on PASCAL-5i, COCO-20i and FSS-1000 datasets to show the superiority of CGPRNet over the previous state-of-the024 art methods. Under both 1-shot and 5-shot settings, our CGPRNet obtains better mIoU, FB-IoU and Dice scores on these three benchmarks, demonstrating the effectiveness of cross-scale and query-conditioned prototype refinement learning for robust few-shot segmentation.

# Pipeline Architecture
![Architecture](https://github.com/proloy190902/CGPRNet/blob/de919e29b1f674e3c26e73bccec5e4a4e33235aa/CGPRNet%20Architecture.png)



# Dataset: 
