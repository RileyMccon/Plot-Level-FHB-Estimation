
# Plot-Level FHB Estimation Workflow

This repository accompanies the manuscript **An End-to-End Computer Vision Workflow for Fusarium Head Blight Phenotyping in Wheat Using Smartphone Images**.

This covers the development and implementation of multiple machine learnings models, used to create and validate this workflow. 

The YOLO_Train file denotes the hyperparameter optimization and training settings used for each object detection model. The hyperparameters used for each model in this study are found in the Hyperparameters folder. 

The Pixel_Classification_Test file shows the training and testing of five different approaches for classifying pixels as healthy or infected. This data stems from 1000 annotated pixels from various different images. The data can be found in the Data folder. The Decision_Boundary_Comparison file generates a 3D artifact to visualize the decision boundary for pixel classification among various models. 

The FHB_Estimation_Combined file applies all five pixel classification approaches to the segmentation masks produced using the YOLO26x detection model and SAM3 segmentation model. The FHB_Estimation_LogReg file then applies this approach to a folder of images, using both SAM3 and MobileSAM for segmentation. 

The Workflow_Visual_Comparison file then shows the Spearman correlation and Deming regression analysis used to compare workflow estimates and traditional visual scores. 

All data used in this study will be uploaded to Dryad, and will be linked here once available. 