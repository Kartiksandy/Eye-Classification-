## Preprocessing Eye Images for Gender Classification

This project involves the preprocessing of eye images for the purpose of gender classification using various machine learning models, including SVM, MLP, and CNN. The goal is to determine the most effective model for accurately classifying gender based on eye images.

### Project Overview:
1. **Data Preparation:**
   - **Dataset Path:** The notebook begins by specifying the paths to the dataset folders containing images for classification.
   - **Target Variable Distribution:** Analyzes the distribution of the target variable (gender) to understand the balance of the dataset.

2. **Data Preprocessing:**
   - Involves steps to preprocess the eye images, ensuring they are correctly formatted and standardized for input into the models.
   - Preprocessing may include resizing images, normalization, and converting images to grayscale if necessary.

3. **Model Implementation:**
   - **SVM Model:** 
     - A Support Vector Machine (SVM) model is trained on the preprocessed data.
     - Evaluation metrics include precision, recall, F1-score, and accuracy.
     - Results indicate moderate performance with a 77% overall accuracy.
   - **MLP Model:** 
     - A Multi-Layer Perceptron (MLP) model is also trained, providing an improved performance with an overall accuracy of 83%.
     - This model shows a balanced F1-score of 83% for both male and female classifications.
   - **CNN Model:**
     - A Convolutional Neural Network (CNN) model is implemented, achieving the best results with an overall accuracy of 89%.
     - The CNN model excels in capturing complex patterns within the images, leading to the highest precision, recall, and F1-scores among the three models.

4. **Observations:**
   - The notebook provides a detailed comparison of the three models based on their performance metrics:
     - **SVM Model:** Precision (78% male, 76% female), Recall (75% male, 79% female), F1-Score (76% male, 78% female), Accuracy (77%).
     - **MLP Model:** Precision (84% male, 82% female), Recall (81% male, 85% female), F1-Score (83% male, 83% female), Accuracy (83%).
     - **CNN Model:** Precision (88% male, 91% female), Recall (91% male, 88% female), F1-Score (90% male, 89% female), Accuracy (89%).

5. **Conclusion:**
   - The CNN model outperformed both the SVM and MLP models, making it the most effective model for this classification task.
   - The MLP model provided a good balance between simplicity and performance, while the SVM model, though less complex, still offered reasonable results.

### How to Use:
1. **Clone the Repository:**
   - Clone the repository to your local machine using `git clone`.
   
2. **Install Dependencies:**
   - Install the required Python libraries listed in the `requirements.txt` file using `pip install -r requirements.txt`.

3. **Run the Notebook:**
   - Open the notebook in Jupyter and execute the cells sequentially to perform the preprocessing and run the classification models.

### Conclusion:
This project demonstrates the effectiveness of different machine learning models in classifying gender based on eye images. The CNN model, with its ability to capture intricate patterns in image data, emerges as the best-performing model, making it a valuable tool for image-based classification tasks.
