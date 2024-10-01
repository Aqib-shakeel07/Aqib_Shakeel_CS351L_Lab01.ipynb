Breast Cancer Classification using k-Nearest Neighbors (k-NN)
This project demonstrates how to classify data from the breast cancer dataset using the k-Nearest Neighbors (k-NN) algorithm. It is interactive, allowing you to adjust the value of k and visualize the classification results.

Table of Contents
Overview
Requirements
Installation
Usage
How It Works
Widgets
Visualization
Credits
Overview
The project uses the load_breast_cancer dataset from scikit-learn, applies k-NN classification, and provides interactive control for selecting different k values. It visualizes the results, displaying the classification accuracy and a report based on the model's predictions.

Requirements
The following libraries are required for this project:

NumPy
Pandas
scikit-learn
Matplotlib
Ipywidgets
IPython
You can install the required libraries using pip:

bash
Copy code
pip install numpy pandas scikit-learn matplotlib ipywidgets
Installation
Clone the repository or download the script.
Ensure all required libraries are installed using the command above.
Run the script in a Jupyter Notebook or any environment that supports ipywidgets.
Usage
Load the Breast Cancer Dataset: The script loads the breast cancer dataset from scikit-learn, which includes features and target labels indicating whether a tumor is benign or malignant.

Interactive k-NN Classification: You can adjust the value of k (the number of neighbors) using the slider provided in the widget. After selecting a value, click the "Run k-NN" button to execute the k-NN algorithm with that k value.

Display Results: The script will display:

The accuracy of the model for the test data.
A detailed classification report showing precision, recall, f1-score, and support for each class (malignant or benign).
A scatter plot showing the classification result, using the first two features of the dataset.
How It Works
The dataset is split into training (70%) and testing (30%) sets using train_test_split.
The k-NN classifier is implemented using KNeighborsClassifier from scikit-learn.
Model performance is evaluated on the test set using accuracy_score and classification_report.
A scatter plot visualizes the classification result by plotting the test data and color-coding the predicted classes.
Widgets
The project uses the following interactive widgets from ipywidgets:

Slider: Adjust the k value (from 1 to 10) using a slider.
Button: Click the button to run the classification algorithm with the selected k value.
Visualization
Before Classification: The script first visualizes the dataset using the first two features (e.g., mean radius and mean texture) and colors the points based on their true labels.

After Classification: Once the classification is run, it visualizes the test data with predicted labels, updating the color and showing a color bar that indicates the predicted class (malignant or benign).

Credits
The breast cancer dataset is sourced from the scikit-learn library.
k-NN classifier implemented using scikit-learn.
Plotting and visualizations are handled using matplotlib.
