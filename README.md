Scratch Detection on Text Images
Author: Rahul Gour
Email: gaurr210@gmail.com
Date: December 2, 2024
Objective:
This project aims to develop a machine learning model to classify text images into two categories:
1. Good Images: Text is clear and free of scratches.
2. Bad Images: Text has visible scratches.
The trained model can also be extended to detect scratches on other surfaces, such as metal or
glass.
Setup Instructions:
1. Clone the Repository:
 git clone <your-repo-link>
 cd <your-repo-directory>
2. Install Dependencies:
 pip install tensorflow numpy matplotlib
3. Dataset Preparation:
 Ensure the dataset follows this structure:
 dataset/
 good/
 bad/
 Extract the zipped dataset and ensure the good and bad folders are in the same directory.
4. Run the Training Script:
 python train_and_evaluate.py
5. Test the Model on a Single Image:
 python test_model.py --image_path path/to/your/image.jpg
Files in the Repository:
1. train_and_evaluate.py: Script for dataset preparation, model training, and evaluation.
2. test_model.py: Script for testing the model on individual images.
3. scratch_detection_model.h5: Pre-trained model file.
4. README.pdf: Project documentation.
5. Detailed_Report_Scratch_Detection.pdf: Detailed explanation of the project.
Code Explanation:
Dataset Handling:
- The dataset is extracted from a zipped file and verified to ensure it contains good and bad folders.
- Images are resized and normalized during preprocessing.
Model Architecture:
- The CNN model includes convolutional layers for feature extraction, max-pooling layers for
dimensionality reduction, dense layers for classification, and dropout for regularization.
Training Process:
- The model uses 'adam' optimizer and 'binary_crossentropy' loss function.
- Early stopping monitors validation loss to avoid overfitting.
Evaluation and Visualization:
- Training and validation accuracy and loss are plotted over epochs.
- Random samples from the dataset are displayed with their labels (Good or Bad).
Testing:
- A single image can be tested to predict whether it has scratches or not.
Acknowledgments:
This project was authored by Rahul Gour. Special thanks to resources and communities that
supported the implementation of machine learning techniques and dataset handling.
