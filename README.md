## Experimental Results

### Dataset
Oxford-IIIT Pet Dataset

### Model
CLIP (`openai/clip-vit-base-patch32`)

### Initial Evaluation
- Images tested: 20
- Correct predictions: 19
- Incorrect predictions: 1
- Sample accuracy: 95%

### Prompt Comparison
- Original prompt accuracy: 95%
- Alternative prompt accuracy: 95%
- Accuracy change: 0 percentage points

### Failure Analysis
One Beagle image was classified as a Basset Hound.
Visual similarity may be a contributing factor, but this
requires further investigation.

### Limitations
The evaluation used only 20 images. These results do not
represent the model's accuracy across the full dataset.
Prediction scores are relative to the candidate labels.

Detailed results are available in:
- `before_prompt_results.csv`
- `after_prompt_results.csv`
- `failure_analysis.md`
