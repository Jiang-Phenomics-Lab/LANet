# LANet a low-cost, high-accuracy method for estimating flag leaf angle in wheat
## Introduction
- We defined flag leaf angle measurement as a keypoint-based pose detection task and proposed a lightweight deep learning model, LANet, to accurately detect these keypoints. 
- The flag leaf angle in a 2D image can be calculated based on the positions of three keypoints: the flag leaf center (Point L), the junction between the flag leaf and stem (Point J), and the stem center (Point S). These keypoints define the geometric and topological relationships necessary for angle computation. 
- To reduce the effects of minor annotation errors on model training when using discrete keypoints as targets, we transformed keypoint prediction into a heatmap regression task. 


## Installation

### Clone the Repository: 
```
git clone https://github.com/Jiang-Phenomics-Lab/LANet.git
cd LANet
```

## Requirements
Install dependencies using pip
```
pip install -r requirements.txt
```

## Train:
`train.py` is used to train segmentation models
```bash
python train.py
```
## Predict
`predict.py` is used to segment wheat plants from images
```bash
python predict.py
```
## Phenotyping:
The phenotyping method is in the `phenotypying.ipynb` 







