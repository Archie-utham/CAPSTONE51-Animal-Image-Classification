
# Failure Analysis Report

## Project
Image Classification Mini-Project with Hugging Face

## Model
CLIP: openai/clip-vit-base-patch32

## Dataset
Oxford-IIIT Pet Dataset

## Test Results
- Images tested: 20
- Correct predictions: 19
- Incorrect predictions: 1
- Sample accuracy: 95%

## Incorrect Prediction

- Image index: 419
- Actual breed: Beagle
- Predicted breed: Basset Hound
- Prediction score: 52.34%

## Possible Explanation
The model may have confused the Beagle with the Basset Hound
because of visual similarities. This is a hypothesis and requires
further image inspection to confirm.

## Prompt Improvement Experiment

- Original prompt accuracy: 95%
- Alternative prompt accuracy: 95%
- Accuracy change: 0 percentage points

The alternative prompt did not improve accuracy on this
20-image sample.

## Limitations
- Only 20 test images were evaluated.
- Results may vary on a larger or different sample.
- Prediction scores are relative to the candidate breed labels;
  they are not guaranteed to represent calibrated confidence.
- The experiment does not establish overall dataset accuracy.

## Conclusion
The model correctly classified 19 of the 20 selected images.
Changing the prompt wording did not improve the measured accuracy.
Further testing is needed to evaluate other improvement methods.
