# wine-cultivator-app

A beginner-friendly machine-learning project that predicts one of three classes in scikit-learn's built-in Wine dataset from 13 chemical measurements.

Requirements
Python 3.10 or newer
VS Code with the Python extension
Run in VS Code
Extract the ZIP and open the wine-cultivar-app folder in VS Code.

Open Terminal → New Terminal.

Create a virtual environment (recommended):

Windows

py -m venv .venv
.venv\Scripts\activate
macOS/Linux

python3 -m venv .venv
source .venv/bin/activate
Install dependencies:

python -m pip install -r requirements.txt
Start the web app:

streamlit run app.py
Open the local URL printed in the terminal, usually http://localhost:8501.

Train/evaluate from the terminal
python train_model.py
Project structure
app.py — Streamlit interface and interactive predictions.
train_model.py — model training and evaluation script.
requirements.txt — Python dependencies.
Dataset and limitations
The app uses the Wine recognition dataset included with scikit-learn, so no separate CSV download is required. It has 178 samples, 13 numeric features, and three target classes. The class labels are shown as Cultivar 1–3 for clarity. The displayed test accuracy is measured on a held-out split; results may vary if the split or model changes. Predictions are educational demonstrations and should not be used for real-world wine authentication.
