
# Prompt Library — CAPSTONE 51

## Project
Image Classification Mini-Project with Hugging Face

## Model
openai/clip-vit-base-patch32

## 1. Initial Prediction Prompts

The initial single-image demonstration compared the image with
these five candidate labels:

- a photo of a parrot
- a photo of a rabbit
- a photo of a dog
- a photo of a cat
- a photo of a horse

Observed result for the sample parrot image:
- Predicted label: parrot
- CLIP score among the five labels: 99.88%

This score is relative to the five candidate labels, not a
general measure of model accuracy.

## 2. Breed Classification — Original Prompt

Template:

a photo of a {breed} pet

The template was applied to the 37 candidate pet breeds.

Observed sample accuracy:
- Correct predictions: 19 out of 20
- Accuracy: 95%

## 3. Breed Classification — Alternative Prompt

Template:

a clear photograph of a {breed}, showing its distinctive breed features

Observed sample accuracy:
- Correct predictions: 19 out of 20
- Accuracy: 95%

## 4. Comparison

Changing the prompt wording produced no measured accuracy
improvement on the selected 20-image sample.

Accuracy change: 0 percentage points.

## 5. Example Failure

- Actual breed: Beagle
- Predicted breed: Basset Hound
- Image index: 419

The model may have confused visual features between these breeds.
This explanation is a hypothesis, not a confirmed cause.

## 6. Responsible Prompting Notes

- Use clear and consistent descriptions.
- Compare prompts on the same evaluation images.
- Record actual results rather than assuming a prompt improves accuracy.
- Do not interpret CLIP scores as calibrated probabilities.
- Test a larger sample before drawing broader conclusions.
