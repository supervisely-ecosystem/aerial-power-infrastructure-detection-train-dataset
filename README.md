<div align="center" markdown>

<img src="https://i.imgur.com/UdBujFN.png" width="250"/> <br>
  
<img src="https://github.com/supervisely-ecosystem/aerial-power-infrastructure-detection-train-dataset/assets/119248312/32ba958e-07a8-4509-9a72-f82064f75e9a"/> 

# Train dataset - Aerial Power Infrastructure Detection

</div>

# Overview

Autonomous inspection of power networks with Unmanned Aerial Vehicles (UAVs) has recently gained significant scientific attention mainly due to rapid advances in UAV technology. In this context, the UAV must autonomously navigate across the network acquiring high resolution data in a safe and fast manner, which poses challenges especially in cases where the location of infrastructure components, i.e. poles, is not known. The Aerial Power Infrastructure Detection Dataset is constructed aiming to create a repository available to the research community, which can be used for training online detection models, which in turn facilitate UAV localization across the network.

Specifically, this dataset is used for implementing the “Pole Detection” process of ICARUS toolkit, which is a vision-based UAV monitoring platform for autonomous inspection of Medium Voltage (MV) power distribution network. Specifically, the UAV is supplied with the best-known coordinates of poles and navigates to the designated location searching for the pole. As soon as the pole is detected, using an one-class detection model, the UAV applies a control procedure to correct its position by aligning directly above the pole. For the training, we used samples containing the T-shaped bar of the pole with the insulators and the top of pole [1].

The dataset consists of top-view images of MV poles from various locations across Cyprus. Images were captured across different seasons to account for a variety of background conditions, such as grass or ground, as well as at different heights to account for variations in the UAV’s height during inspection. Additionally, all annotations were converted into VOC and COCO formats for training in numerous frameworks. The dataset consists of the following images and detection objects (t-bars):

| Subset       | Images  | T-Bars  |
| ------------ | ------- | ------- |
| Training     | 10760   | 10012   |
| Validation   | 2587    | 2370    |
| Testing      | 1572    | 1449    |

## Download
Direct download: [tar archive](https://github.com/supervisely-ecosystem/aerial-power-infrastructure-detection-train-dataset/releases/download/v0.9.0/Train.tar) (136 MB)

# Data-Example

<img src="https://github.com/supervisely-ecosystem/aerial-power-infrastructure-detection-train-dataset/assets/119248312/452d1126-7521-4830-b791-4f080a80d024"/>

> Examples of images labeled with three classes of objects: insulator, pollution flashover, broken.
