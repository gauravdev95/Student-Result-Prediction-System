# 🎓 Student Pass/Fail Prediction using Random Forest

This project demonstrates a simple machine learning workflow to predict whether a student will **pass or fail** based on several features like exam score, attendance, and study hours. It uses a **Random Forest Classifier** for the prediction task and includes steps for data generation, exploratory data analysis, model training, and evaluation.

The script also includes an **interactive command-line interface** to get predictions for new student data.

---

## 📁 Project Structure

The project is contained within a single Python script that performs the following steps:

- **Data Generation**: Creates a synthetic dataset of 1000 students.
- **Exploratory Data Analysis (EDA)**: Visualizes correlations and the distribution of the target variable.
- **Data Preprocessing**: Splits the data into training and testing sets and scales the numerical features.
- **Model Training**: Trains a Random Forest Classifier on the preprocessed data.
- **Model Evaluation**: Calculates and prints various performance metrics (accuracy, precision, recall, F1-score) and generates a confusion matrix.
- **Interactive Prediction**: Provides a command-line loop for users to input new student data and receive a pass/fail prediction.
- **Model Serialization**: Saves the trained model and the scaler to `.pkl` files for future use.

---

## 📦 Dependencies

To run this script, you need to have the following Python libraries installed. You can install them using pip:


pip install pandas numpy matplotlib seaborn scikit-learn
The joblib library is also used for saving the model. It is often installed with scikit-learn, but you can install it separately if needed:

bash
Copy
Edit
pip install joblib
🚀 How to Run
The code lives in `app.py` (run it directly — no rename needed).

Open your terminal or command prompt.

Navigate to the directory where you saved the file.

Run the script using the Python interpreter:

bash
Copy
Edit
python app.py
🧾 Output
When you run the script, the console will first print information about the dataset, model evaluation metrics, and feature importance.

The script will also generate three image files in the same directory:

correlation_matrix.png: A heatmap showing the correlation between all features.

pass_fail_distribution.png: A bar chart showing the count of students who passed and failed.

confusion_matrix.png: A heatmap of the model's confusion matrix.

Finally, the script will save two .pkl files:

pass_fail_model.pkl: The trained Random Forest model.

scaler.pkl: The fitted StandardScaler object, which is necessary to preprocess new data for prediction.

💡 Interactive Prediction
The script will then enter an interactive loop where you can input student details to get a prediction.

To exit this loop, simply type exit when prompted.

🧑‍💻 Author
Gaurav Yadav

Feel free to use, modify, and improve this project as needed!



