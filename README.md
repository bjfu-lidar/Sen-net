# Sen-net
By Hao Lu,†, Bowen Li,†, Gang Yang, Guangpeng Fan, Han Wang, Yong Pang,*, Zuyuan Wang, Yining Lian, Haifeng Xu, Huan Huang
# Introduction
This is an official release of "Towards a point cloud understanding framework for forest scene semantic segmentation across forest types and sensor platforms"
# Abstract
Foliage, wood (i.e., trunk, branch), ground, and lower objects (i.e., grass, shrubs), are key semantic components of forests that play different roles in the forest ecosystem. For understanding forest ecosystem structure and function, Light Detection And Ranging (LiDAR) point cloud is a valuable form of remote sensing observation. The understanding intensively relies on precisely performing semantic segmentation task to segment semantic components from forest point cloud data. However, the semantic segmentation of massive point cloud data from forest scenes remains a significant challenge. The forest environment is highly heterogeneous and complex due to tree species and terrain conditions. Different climate zones lead to varying canopy characteristics and the diversity of LiDAR platforms delivers inconsistent point cloud properties. Heuristic approaches and conventional machine learning approaches inevitably suffer from poor generalization. Additionally, most deep learning methods lack a dedicated network design to address the characteristics of forests. This paper introduces Sen-net, a point cloud understanding network specifically constructed for semantic component segmentation of forest scene point cloud. Sen-net implements three modules tailored for forest characteristics. First, a spatial context enhancement module (SCEM) is designed for providing both global and dataset-level perspectives to mine geometric information and robust features hidden in heterogeneous forest. Second, a semantic-driven detail enrichment module (SDEM) is incorporated to preserve rich geometric details and semantic information thereby enhancing the learning of complex structures in the forests. Finally, an adaptive guidance flow (AGF) is added to seamlessly fuse the semantic and detailed features. Comprehensive experiments were conducted on both self-built Lin3D dataset and public datasets. Sen-net achieved an OA of 97.6% and 85.1% MIoU on the Lin3D dataset, and an OA of 94.5 and 78.2% MIoU on the public dataset FOR-instance. Results show that Sen-net outperformed the representative forest scene point cloud semantic segmentation approaches and state-of-the-art deep learning networks, and it has the potential to generalize to point cloud data collected by LiDAR from other platforms. It is concluded that Sen-net is a powerful and robust framework with substantial potential for being widely and deeply explored in forest ecosystem studies.
![Fig_5](https://github.com/user-attachments/assets/ee876b74-fe96-4ceb-9e19-60f4c0c5f293)
# Results
<div align="center">
  <img src="https://github.com/user-attachments/assets/a8f6513f-411a-45c7-aa6f-87f4d2e45d36" alt="Confusion matrix for Lin3D dataset" />
  
  Confusion matrix of the four semantic categories, computed over all points of the Lin3D test dataset.
</div>

<br />

<div align="center">
  <img src="https://github.com/user-attachments/assets/4fca9e65-234b-4959-aa07-8b591031bd3b" alt="Confusion matrix for FOR-instance dataset" />
  
  Confusion matrix of the four semantic categories, computed over all points of the FOR-instance test dataset.
</div>


# Data
Please refer to [Lin3D](https://github.com/bjfu-lidar/Lin3D-Large-scale-forest-scene-INterpretation-3D-point-cloud-dataset)

# Installation
This implementation has been tested on: 

Ubuntu 18.04, PyTorch 1.7.0, Python 3.8, Cuda 11.0, Nvidia RTX 3090

Ubuntu 18.04, PyTorch 1.7.0, Python 3.8, Cuda 11.0, Nvidia A40

# Citation

# Acknowledgement
Codes are built based on a series of previous works, including: <br>
[KPConv](https://github.com/HuguesTHOMAS/KPConv), <br>
