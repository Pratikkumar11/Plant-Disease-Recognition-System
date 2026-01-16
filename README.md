# Plant-Disease-Recognition-System
Plant Disease Recognition System

# Model Setup Instructions

To use this project, you need to download a pre-trained model from the given Google Drive link and place it in the `models` directory. Follow the steps below to set it up correctly:

## Steps to Download and Place the Model

1. **Download the Model**
   - Click [here](https://drive.google.com/file/d/1Ond7UzrNOfdAXWedjlZr2sDXYU6MRBuj/view?usp=sharing) to open the Google Drive link.
   - Click the **Download** button to save the file to your local system.

2. **Create the Models Folder**
   - Navigate to the root directory of this project.
   - Create a folder named `models` if it does not already exist.
     ```bash
     mkdir models
     ```

3. **Place the Model in the Folder**
   - Move the downloaded file into the `models` directory.
     ```bash
     mv /path/to/downloaded/model models/
     ```
     Replace `/path/to/downloaded/model` with the actual path where you downloaded the file.

4. **Verify the Setup**
   - Ensure that the model file is correctly placed in the `models` directory by listing the folder's contents:
     ```bash
     ls models
     ```
     You should see the downloaded model file in the output.

## Usage

1. **Specify the Model File Location**
   - Open the `app.py` file in a text editor.
   - Locate line 8, which contains the following code:
     ```python
     tf.keras.models.load_model("")
     ```
   - Update the empty string with the relative path to the model file. For example:
     ```python
     tf.keras.models.load_model("models/your_model_file.keras")
     ```
     Replace `your_model_file.keras` with the actual name of the model file you downloaded.

2. **Run the Server**
   - Open a terminal and navigate to the root directory of this project.
   - Run the following command to start the server:
     ```bash
     python app.py
     ```

3. **Access the Application**
   - Once the server is running, follow the instructions displayed in the terminal to access the application in your web browser.
🌱 Plant Disease Recognition System
AI-Based Leaf Disease Detection Using Deep Learning (Flask Web App)

This project is a web-based plant disease detection system built using Flask, TensorFlow, and a CNN deep learning model.
Users can upload a leaf image, and the system predicts the disease, its cause, and cure using a pretrained .keras model.



🚀 Features
✔ AI-Based Disease Prediction

Upload a plant leaf image

CNN model predicts the disease

Displays:

Disease Name

Cause

Treatment / Cure

✔ Modern UI

Clean and responsive user interface

Upload section + result card

Smooth navigation

About section

Contact section

✔ 38+ Disease Classes

The model supports detection of many diseases across crops such as:

Tomato

Apple

Potato

Corn

Grape

Pepper

Soybean

Strawberry
and more.

📁 Project Folder Structure
Plant-Disease-Recognition-System/
│
├── app.py
├── plant_disease.json
│
├── model/
│   └── plant_disease_recog_model_pwp.keras
│
├── templates/
│   └── home.html
│
├── static/
│   ├── css/
│   │   └── style.css
│   ├── images/
│   └── js/
│
├── uploadimages/
│   └── (Uploaded images stored temporarily)
│
└── README.md

⚠️ Important Note: Avoid the Double-Folder Error

Sometimes ZIP extraction creates a folder inside another folder with the same name:

Plant-Disease-Recognition-System-main/
    Plant-Disease-Recognition-System-main/
        app.py


If you open the outer folder, the command:

python app.py


will give error:

python: can't open file 'app.py'

✅ Fix

Always open this folder:

Plant-Disease-Recognition-System-main\Plant-Disease-Recognition-System-main\


You must see app.py inside the folder you run.

🛠 How to Run the Project (Step-by-Step Guide)
✅ 1. Install Python

Install Python 3.9+ from:
https://www.python.org/downloads/

✔ Check “Add Python to PATH” during installation.

✅ 2. Extract the Project ZIP

Right-click ZIP → Extract All.

Open the inner folder containing app.py.

✅ 3. Open Project in VS Code

Open VS Code

Click File → Open Folder

Select the folder containing app.py

✅ 4. Open Terminal

Press:

Ctrl + `


Or:

Terminal → New Terminal

✅ 5. Install Required Libraries

Run in terminal:

pip install flask tensorflow numpy

✅ 6. Run Flask App
python app.py


You will see:

Running on http://127.0.0.1:5000/

✅ 7. Open Web Browser

Go to:

http://127.0.0.1:5000/


Your web application is now running.

🌿 How the System Works

User uploads a leaf image

Image resized to 160×160

Passed into CNN model

Highest probability class is selected

Disease details fetched from plant_disease.json

UI displays:

Disease Name

Cause

Cure

🔧 Troubleshooting
❗ 1. app.py not found

Fix:

cd "Your/Correct/Project/Folder"
python app.py

❗ 2. TensorFlow not installed

Install again:

pip install tensorflow

❗ 3. Model file not found

Make sure your model is in:

model/plant_disease_recog_model_pwp.keras

❗ 4. Blank page / CSS not loading

Ensure folder names are exactly:

templates/
static/css/
static/images/

👨‍💻 Author

Pratik Kumar Bhagat Mca/10033/24
MCA Final Year Minor Project — Plant Disease Detection Using CNN