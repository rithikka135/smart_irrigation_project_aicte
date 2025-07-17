🌿 Smart Irrigation Recommendation System A machine learning-based system that helps farmers and agricultural professionals make smarter decisions about irrigation method, fertilizer type, and crop selection based on environmental conditions.

📁 Project Structure

📦 Smart_Irrigation/ ├── irrigation_machine.csv # Dataset ├── Irrigation_System.ipynb # Jupyter Notebook (model training + analysis) ├── smart_irrigation_model.pkl # Trained ML model (saved) ├── scaler.pkl # Scaler for input normalization 📄 Dataset: irrigation_machine.csv This dataset includes real or simulated environmental parameters and corresponding recommended outputs.

Feature Description

Temperature Temperature in Celsius Humidity Humidity percentage Soil_Moisture Soil moisture level (sensor reading or %) Rainfall Expected or recorded rainfall (in mm) Irrigation Recommended irrigation method (e.g., Drip) Fertilizer Suggested fertilizer (e.g., Urea) Crop Best crop to grow under the conditions

🔗 The dataset is used to train a multi-output classification model that can predict all three recommendations simultaneously.

📓 Notebook: Irrigation_System.ipynb This Jupyter Notebook contains the full workflow of:

Importing and visualizing the dataset

Correlation heatmap for feature relationships

Data preprocessing and normalization

Splitting into training and testing sets

Training a Random Forest MultiOutputClassifier

Model evaluation with classification report

Saving the model and scaler using joblib

📌 To run the notebook locally:

pip install pandas matplotlib seaborn scikit-learn joblib

🧠 Model Output The model predicts:

✅ Optimal Irrigation Method (e.g., Drip, Sprinkler)

✅ Recommended Fertilizer (e.g., Urea, Compost)

✅ Suitable Crop Type (e.g., Wheat, Rice)

🧪 Example prediction:

model.predict([[30, 60, 6, 85]]) # Sample inputs

Output: ['Drip', 'Urea', 'Wheat']
🚀 How to Run

✅ In VS Code (Recommended) Install Python + Jupyter extension

Open Irrigation_System.ipynb

Run cell by cell using Shift + Enter

✅ In Google Colab Visit: https://colab.research.google.com

Upload the notebook and dataset

Run in the browser with no installation

💡 Future Scope Integrate with IoT sensors for live input

Build a mobile or web app for farmers

Add support for more crop regions and seasons

Deploy as an API for agriculture tech platforms

🙋‍♀️ Developed By Rithikka A. 👩‍💻 Computer Science Engineer | AI & ML Enthusiast 📫 rithikka91@gmail.com
