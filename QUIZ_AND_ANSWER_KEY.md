
# Quiz and Answer Key — CAPSTONE 51

## Part A: Quiz Questions

### 1. What is image classification?
A. Compressing an image  
B. Assigning a label to an image  
C. Editing image colours  
D. Converting an image to text  

### 2. Which model was used in this project?
A. BERT  
B. YOLO  
C. CLIP  
D. ResNet  

### 3. What does CLIP stand for?
A. Contrastive Language–Image Pre-training  
B. Computer Learning Image Processing  
C. Classification Language Input Program  
D. Common Label Identification Process  

### 4. Which dataset was used?
A. MNIST  
B. CIFAR-10  
C. Oxford-IIIT Pet Dataset  
D. ImageNet only  

### 5. Which libraries were used for the project?
A. Hugging Face Transformers and PyTorch  
B. Django and Flask only  
C. NumPy only  
D. Selenium and BeautifulSoup  

### 6. What is a prompt in this project?
A. A computer password  
B. Text describing a candidate image label  
C. A dataset folder  
D. A type of image file  

### 7. How many images were evaluated in the sample experiment?
A. 10  
B. 20  
C. 100  
D. 3,669  

### 8. How many predictions were correct?
A. 15  
B. 18  
C. 19  
D. 20  

### 9. What was the sample accuracy?
A. 50%  
B. 75%  
C. 95%  
D. 100%  

### 10. What happened when the alternative prompt was tested?
A. Accuracy increased by 20 percentage points  
B. Accuracy decreased to 50%  
C. Sample accuracy remained 95%  
D. The model stopped working  

### 11. What was the incorrect prediction in the recorded sample?
A. Cat predicted as dog  
B. Beagle predicted as Basset Hound  
C. Rabbit predicted as horse  
D. Parrot predicted as cat  

### 12. Does a CLIP score of 99% always mean there is a 99% probability that the prediction is correct?
A. Yes, always  
B. No, the score depends on the candidate labels and scoring method  
C. Only for dogs  
D. Only when using Google Colab  

### 13. Why should model predictions be verified?
A. To identify errors and understand limitations  
B. To make every result correct automatically  
C. To avoid recording results  
D. To remove the dataset  

### 14. What is one limitation of evaluating only 20 images?
A. The model cannot process images  
B. The results may not represent performance on the full dataset  
C. The dataset becomes larger  
D. Prompts cannot be changed  

### 15. What is a responsible conclusion from this experiment?
A. The model is perfect  
B. The model will always achieve 95% accuracy  
C. The sample achieved 95% accuracy, but larger evaluation is needed  
D. The alternative prompt definitely improved the model  

---

## Part B: Answer Key

1. **B** — Assigning a label to an image.
2. **C** — CLIP.
3. **A** — Contrastive Language–Image Pre-training.
4. **C** — Oxford-IIIT Pet Dataset.
5. **A** — Hugging Face Transformers and PyTorch.
6. **B** — Text describing a candidate image label.
7. **B** — 20 images.
8. **C** — 19 correct predictions.
9. **C** — 95% sample accuracy.
10. **C** — Sample accuracy remained 95%.
11. **B** — Beagle predicted as Basset Hound.
12. **B** — The score depends on candidate labels and the scoring method; it is not a calibrated probability.
13. **A** — To identify errors and understand limitations.
14. **B** — The sample may not represent the full dataset.
15. **C** — The sample achieved 95% accuracy, but a larger evaluation is needed.

---

## Part C: Short-Answer Questions

### 1. What is the purpose of the Oxford-IIIT Pet Dataset?
It provides images of cats and dogs across 37 breeds for computer vision tasks, including image classification.

### 2. What is the difference between actual and predicted labels?
The actual label is the dataset's reference label, while the predicted label is the category selected by the model.

### 3. Why did the model's incorrect prediction matter?
It demonstrated that visually similar breeds can be confused and that model outputs need verification.

### 4. Did the alternative prompt improve the measured result?
No. Both prompt approaches achieved 95% accuracy on the selected 20-image sample.

### 5. How could the evaluation be improved?
Evaluate more images, document the selection method, inspect errors systematically, and compare approaches under the same conditions.
