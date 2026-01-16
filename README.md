# 🌿 Plant Disease Recognition System

---

### 🌱 Deep Learning–Based Plant Disease Detection using CNN & Flask

![Python](https://img.shields.io/badge/Python-3.10-blue)
![Flask](https://img.shields.io/badge/Flask-WebApp-black)
![Deep Learning](https://img.shields.io/badge/Deep%20Learning-CNN-green)
![Status](https://img.shields.io/badge/Status-Completed-success)

A web-based Plant Disease Recognition System built using Flask, Deep Learning, and Computer Vision.
The application allows users to upload an image of a plant leaf and get disease-related information such as disease name, cause, and cure.

🚀 Features

🌱 Upload plant leaf images through a clean UI

🧠 Deep Learning–based disease prediction

📋 Displays disease name, cause, and cure

🎨 Modern animated UI using HTML, CSS & Bootstrap

🖥️ Flask-based backend

🛠️ Tech Stack

Frontend: HTML, CSS, Bootstrap

Backend: Flask (Python)

Machine Learning: TensorFlow / Keras

Others: NumPy, JSON

📂 Project Structure
Plant-Disease-Recognition-System
│
├── app.py
├── README.md
├── plant_disease.json
├── templates/
│   └── home.html
├── static/
│   ├── css/
│   ├── js/
│   └── images/
├── uploadimages/
├── model_training_code/
│   └── plant.ipynb
└── .gitignore

⚠️ Model File Notice

❗ The trained deep learning model (.keras file) is not included in this repository.

Reason:
GitHub has a file size limit of 100 MB, and the trained model exceeds this limit.

You can:

Train the model using the notebook in model_training_code/

Or load your own trained .keras model

▶️ How to Run the Project
1️⃣ Clone the Repository
git clone https://github.com/Pratikkumar11/Plant-Disease-Recognition-System.git
cd Plant-Disease-Recognition-System

2️⃣ Create Virtual Environment
python -m venv venv


Activate it:

Windows

venv\Scripts\activate


Linux / macOS

source venv/bin/activate

3️⃣ Install Dependencies
pip install flask tensorflow numpy

4️⃣ Run the Application
python app.py

5️⃣ Open in Browser
http://127.0.0.1:5000

📸 Screenshots

UI includes animated background, upload section, and result display
(Screenshots can be added here later)

📌 Future Improvements

Add real-time camera support

Improve model accuracy

Deploy on cloud (Render / AWS / HuggingFace)

Add multi-language support

👨‍💻 Author

Pratik Kumar
📌 GitHub: Pratikkumar11
