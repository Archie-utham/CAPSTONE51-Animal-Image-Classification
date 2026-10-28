
# Dataset Documentation

## 1. Dataset Name
Oxford-IIIT Pet Dataset

## 2. Dataset Purpose
This dataset is used to evaluate image classification using a
pre-trained CLIP model from Hugging Face Transformers.

## 3. Dataset Contents
The dataset contains images of cats and dogs across 37 pet breeds.

## 4. Dataset Source
Official dataset website:
https://www.robots.ox.ac.uk/~vgg/data/pets/

## 5. Dataset Split Used
The test split was used for the project experiment.

- Total test images loaded: 3,669
- Images selected for evaluation: 20
- Image dimensions observed: 300 × 225 pixels for the first image

## 6. Model Used
- Model: openai/clip-vit-base-patch32
- Framework: Hugging Face Transformers
- Deep learning framework: PyTorch

## 7. Evaluation Method
The model compared each selected image with text descriptions of
the 37 candidate pet breeds. The highest-scoring breed was
recorded as the prediction.

## 8. Limitations
Only 20 images were evaluated in the reported experiment.
Therefore, the measured 95% sample accuracy must not be treated
as the model's overall accuracy on the complete dataset.

The prediction score is relative to the candidate breed labels
and is not necessarily a calibrated probability.

## 9. Responsible Use
The results describe performance on this small sample only.
Additional testing across more images is needed before drawing
broader conclusions about model performance.
