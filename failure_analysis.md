
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

## Individual Image Review

The experiment evaluated 20 selected images from the Oxford-IIIT Pet Dataset.
Each image was checked by comparing the model's predicted breed with the actual breed label.

- Correct predictions: 19 images
- Incorrect predictions: 1 image
- Overall sample accuracy: 95%

The incorrect prediction was reviewed separately to identify a possible
reason for the classification error. The remaining 19 images were correctly
classified according to their dataset labels.

A complete image-by-image review should record the image index, actual breed,
predicted breed, prediction score, and whether the prediction was correct.
The available summary does not contain all 20 individual prediction records,
so those details should be taken from the experiment results rather than guessed.

## Possible Explanation
The model may have confused the Beagle with the Basset Hound
because of visual similarities. This is a hypothesis and requires
further image inspection to confirm.

## Prompt Improvement Experiment

- Original prompt accuracy: 95% (19/20 correct)
- Alternative prompt accuracy: 95% (19/20 correct)
- Accuracy change: 0 percentage points

With the original prompt, image index 419 was incorrectly
classified as Basset Hound instead of Beagle.

With the alternative prompt, image index 571 was incorrectly
classified as Abyssinian instead of Bengal.

Although the incorrect prediction changed, the overall accuracy
remained the same. The alternative prompt did not improve accuracy
on this 20-image sample.

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
