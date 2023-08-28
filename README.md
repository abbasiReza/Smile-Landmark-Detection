# Smile Landmark Detection using PIPNet

## Description

This project detects smile landmarks in facial images using the PIPNet model from torchlm library.

PIPNet is trained to predict heatmaps for smile-related landmarks like mouth corners, lips, and teeth. 

The model is trained on a dataset of over 550 smile images collected at Shahid Beheshti University.

## Model

[PIPNet](https://arxiv.org/abs/2104.04218) from [torchlm](https://github.com/tritechpte/torchlm) is used for efficient landmark heatmap prediction.

## Training Data  

- Smile image dataset with over 550 samples
- Collected at Shahid Beheshti University
- Variety of subjects, head poses, smile types

## Training Process

- PIPNet initialized with pretrained weights
- Fine-tuned on smile images
- Adam optimizer for training 
- Trained for multiple epochs with decaying learning rate

## Evaluation

Model is evaluated on test set for:

- Mean Error between predicted and ground-truth landmarks
- Failure Rate at different error thresholds

## Usage

The trained model can be used for:

- Detecting smile landmarks in new images
- Applications like expression recognition, face editing

## References

- [PIPNet Paper](https://arxiv.org/pdf/2003.03771.pdf)
- [torchlm Library](https://github.com/deftruth/torchlm)
