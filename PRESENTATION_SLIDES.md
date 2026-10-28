
# CAPSTONE 51 — Image Classification Mini-Project with Hugging Face

## Slide 1: Title

**Image Classification Mini-Project with Hugging Face**

- Capstone Project 51
- Technology: Python, Hugging Face Transformers, PyTorch
- Model: CLIP (openai/clip-vit-base-patch32)
- Dataset: Oxford-IIIT Pet Dataset

Presenter: [Archina]

## Slide 2: Introduction and Objectives

**Introduction**

Image classification uses machine learning to assign labels to images. This project explores CLIP, a model that compares images with text descriptions.

**Objectives**
- Build an image classification experiment.
- Explore zero-shot classification using text prompts.
- Evaluate predictions against dataset labels.
- Analyse incorrect predictions and limitations.

## Slide 3: Tools and Dataset

**Tools**
- Python
- Google Colab
- Hugging Face Transformers
- PyTorch
- GitHub

**Dataset**
- Oxford-IIIT Pet Dataset
- Contains cat and dog images across 37 breeds.
- The test split contains 3,669 images.
- A sample of 20 images was used for this experiment.

## Slide 4: Methodology

1. Set up the Google Colab environment.
2. Load the pretrained CLIP model and processor.
3. Load images from the Oxford-IIIT Pet Dataset.
4. Compare images with candidate text labels.
5. Record predictions and compare them with actual breed labels.
6. Test an alternative prompt template.
7. Save the results and document the findings.

## Slide 5: Results

**Recorded experiment results**

- Images evaluated: 20
- Correct predictions: 19
- Incorrect predictions: 1
- Sample accuracy: 95%

**Prompt comparison**

- Original prompt accuracy: 95%
- Alternative prompt accuracy: 95%
- Measured change: 0 percentage points

These figures describe the selected sample, not the model's overall accuracy.

## Slide 6: Failure Analysis and Limitations

**Incorrect prediction**
- Actual breed: Beagle
- Predicted breed: Basset Hound
- Image index: 419
- Reported CLIP score: 52.34%

**Limitations**
- Only 20 images were evaluated.
- The result may not represent the full dataset.
- CLIP scores depend on candidate labels and prompts.
- The alternative prompt did not improve sample accuracy.

## Slide 7: Conclusion and Future Work

**Conclusion**
- The experiment demonstrated image classification using CLIP.
- The selected sample achieved 95% accuracy.
- One incorrect prediction was documented.
- Prompt changes did not improve the measured result.

**Future Work**
- Evaluate a larger, documented sample.
- Analyse additional incorrect predictions.
- Compare alternative prompts and models.
- Report results with appropriate limitations.

**Thank You**
