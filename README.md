# CMNet
Machine-oriented multi-scale feature compression seeks to eliminate task-insensitive redundancy while preserving task-critical semantic and structural information. However, existing methods primarily focus on reducing cross-scale redundancy among multi-scale features, while largely neglecting intra-scale redundancy within individual feature maps, which limits overall coding efficiency. To address this problem, we propose CMNet, a compression-efficient collaborative mining network for multi-scale feature compression, which jointly exploits intra-scale and cross-scale correlations to more comprehensively reduce task-irrelevant redundancy. Specifically, an intra-scale redundancy-aware module is proposed to suppress redundancy within each single-scale feature map. In this module, a swin transformer block and a multi-receptive-field local perception block are introduced to capture global and diverse local contextual correlations, respectively, while an attention-driven selective aggregation block is developed to preserve task-essential feature representations. In addition, a context-guided adaptive fusion module is designed to dynamically mine spatial and channel correlations across multi-scale features, thereby reducing cross-scale redundancy. Experimental results on multiple downstream machine vision tasks demonstrate that the proposed CMNet achieves superior rate-accuracy performance over state-of-the-art multi-scale feature compression methods.
# Training and Testing
## (1) Training Stage
python train.py
## (2) Finetuning Stage
python train_finetune.py
## (3) Testing Stage
python test_and_results_all_in_folder_seg.py
# Requirements
(1) torch==2.4.1  
(2) compressai==1.2.6  
(3) detectron2==0.6  
(4) tensorboard=2.14.0  
(5) numpy==1.22.4  

# Data availability
(1) OpenImagesV6:[....], Extraction Code:[....]

(2) COCO2017:[....], Extraction Code:[....]

(3) SFU:[....], Extraction Code:[....]
