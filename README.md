# Brain Tumor Classification using CNN

## Project Description
Classify brain tumors using a CNN on MRI images. Includes data preprocessing, augmentation, CNN training, and performance evaluation.

---

## Dataset
The dataset used in this project is from kaggle:
[Dataset Link](https://www.kaggle.com/datasets/rm1000/brain-tumor-mri-scans)

---

## Project Structure
- notebook.ipynb : Main notebook file
- results/ : Output images including:
    - classification report
    - loss accuracy curve
    - confusion matrix
- docs/ : Presentation slides (presentation.pdf)
- README.md : Project documentation  

---

## Requirements
- Python >= 3.8  
- Libraries: numpy, opencv-python, matplotlib, tensorflow, scikit-learn  
- GPU recommended  

---

## Steps
1. Load & Clean Data: Read images per class, ignore corrupted files.  
2. Preprocessing: Resize (128x128), grayscale, normalize, apply CLAHE (contrast) and optional sharpening.  
3. Encode Labels: Convert class names to numbers.  
4. Split Dataset: 80% train, 20% test (stratified).  
5. Augmentation & Balance: Use ImageDataGenerator to balance classes.  
6. CNN Model: 3 Conv+MaxPool blocks, Flatten, Dense+Dropout, Softmax output.  
7. Train & Evaluate: Adam optimizer, categorical_crossentropy, EarlyStopping, test accuracy, confusion matrix, precision/recall/F1.

---

## Notes
- CLAHE improves contrast better than median/sharpening.  
- Augmentation is important for class balance.  
- Adjust image size and epochs as needed.  

---

## Contributors

- Aya Ahmed 
- Esraa Nasser
- Amina Amer
- Habiba Mohamed
- Roaa Mohamed


