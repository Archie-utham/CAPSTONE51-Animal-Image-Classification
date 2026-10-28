
# AI Output Verification Report — CAPSTONE 51

## 1. Project Details

- **Project:** Image Classification Mini-Project with Hugging Face
- **Model:** openai/clip-vit-base-patch32
- **Dataset:** Oxford-IIIT Pet Dataset
- **Framework:** Hugging Face Transformers and PyTorch
- **Environment:** Google Colab

## 2. Purpose

This report documents how the model's image classification outputs were checked against the dataset labels and how the results were interpreted.

## 3. Verification Method

1. Selected 20 images from the Oxford-IIIT Pet test dataset.
2. Recorded each image's actual breed from its dataset filename.
3. Compared the actual breed with the model's predicted breed.
4. Counted matching and incorrect predictions.
5. Compared the original prompts with the alternative prompts.
6. Recorded the observed results without claiming unmeasured improvements.

## 4. Verification Results

- **Images evaluated:** 20
- **Correct predictions:** 19
- **Incorrect predictions:** 1
- **Sample accuracy:** 95%
- **Original prompt accuracy:** 95%
- **Alternative prompt accuracy:** 95%
- **Measured improvement:** 0 percentage points

These results apply only to the selected 20-image sample. They do not establish the model's overall accuracy on the full dataset.

## 5. Incorrect Prediction Review

- **Image index:** 419
- **Actual breed:** Beagle
- **Predicted breed:** Basset Hound
- **Reported CLIP score:** 52.34%

The model confused two dog breeds in this example. Their visual similarities may be a possible explanation, but further image inspection and testing would be needed to confirm the cause.

## 6. Limitations

- Only 20 images were evaluated for this experiment.
- Results may differ when another set of images is selected.
- CLIP scores depend on the candidate labels and prompts provided.
- A CLIP score is not a calibrated probability that the prediction is correct.
- The prompt experiment did not improve accuracy in this sample.

## 7. Responsible Use

The outputs were checked against the dataset labels instead of being accepted without verification. The report distinguishes measured results from possible explanations and avoids claiming that the experiment proves general model performance.

## 8. Conclusion

The verification process identified one incorrect prediction among 20 evaluated images. Both prompt approaches achieved 95% sample accuracy. A larger evaluation with a documented sample-selection method is needed to draw stronger conclusions.
