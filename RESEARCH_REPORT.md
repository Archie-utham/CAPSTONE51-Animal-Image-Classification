
# Research Report: Image Classification with Hugging Face

## 1. Abstract

This project evaluates a pre-trained CLIP model for classifying
pet breeds using images from the Oxford-IIIT Pet Dataset.
The experiment compares two text-prompt styles and investigates
an incorrect prediction.

## 2. Introduction

Image classification is a computer vision task in which a model
assigns labels to an image. Pre-trained models can be used to
compare images with text descriptions without training a new
classifier from scratch.

This project uses CLIP, a vision-language model available through
Hugging Face Transformers.

## 3. Objectives

- Understand image classification and zero-shot prediction.
- Use a pre-trained Hugging Face model.
- Evaluate predictions on a sample of pet images.
- Analyse incorrect predictions.
- Compare two text-prompt styles.
- Document limitations and experimental findings.

## 4. Tools and Technologies

- Python
- Google Colab
- Hugging Face Transformers
- CLIP: openai/clip-vit-base-patch32
- PyTorch
- Pandas
- Matplotlib
- Oxford-IIIT Pet Dataset

## 5. Dataset

The Oxford-IIIT Pet Dataset contains images from 37 cat and dog
breeds. The test split loaded for this experiment contained
3,669 images. A fixed sample of 20 images was selected for
evaluation.

## 6. Methodology

1. Load the pre-trained CLIP model and processor.
2. Load the Oxford-IIIT Pet test dataset.
3. Select 20 images using a fixed random seed.
4. Compare each image with text descriptions of the candidate breeds.
5. Record predictions and compare them with the actual breed labels.
6. Change the text-prompt wording and repeat the evaluation.
7. Save the results and investigate the incorrect prediction.

## 7. Results

Initial evaluation:
- Images tested: 20
- Correct predictions: 19
- Incorrect predictions: 1
- Sample accuracy: 95%

Prompt comparison:
- Original prompt accuracy: 95%
- Alternative prompt accuracy: 95%
- Accuracy change: 0 percentage points

One image whose actual breed was Beagle was predicted as
Basset Hound.

## 8. Failure Analysis

The incorrect prediction suggests that the model may have
difficulty distinguishing some visually similar breeds.
Visual similarity is a possible explanation, not a confirmed cause.

The alternative prompt wording did not change the number of
correct predictions in this sample.

## 9. Limitations

- Only 20 images were evaluated.
- The sample accuracy does not establish full-dataset accuracy.
- Prompt wording was the only improvement method tested.
- Prediction scores are relative to the candidate labels and
  should not be interpreted as calibrated probabilities.
- Further experiments are needed to assess generalisation.

## 10. Conclusion

The CLIP model correctly classified 19 of the 20 selected images.
The alternative prompt produced the same measured accuracy.
The experiment demonstrates how a pre-trained vision-language
model can be evaluated and how errors and limitations can be
documented responsibly.

## 11. Result Files

- before_prompt_results.csv
- after_prompt_results.csv
- failure_analysis.md
- DATASET_DOCUMENTATION.md
