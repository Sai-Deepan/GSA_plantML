# GSA PlantML: ML based Plant Disease Detection

**GSA PlantML** is a lightweight desktop application that uses Google Vision Pro model and Trained ML model to detect plant diseases from leaf images.  
Built with a simple and elegant GUI, it allows users to upload or capture images, analyze plant health, and receive instant disease predictions with confidence scores.

---

## Features

* Detects plant diseases from leaf images using a trained ML model.
* Built in Google vision pro model to suggest possible cure.
* Interactive **CustomTkinter** GUI for smooth user experience.
* Displays **confidence percentage** for predictions.
* Supports both **image upload** and **camera capture**.
* 
---

## Project Structure

* `main.py` – Core plant disease detection logic using TensorFlow / Keras.
* `app.py` – GUI built with CustomTkinter integrating image upload, camera, and prediction display.
* `camera_module.py` – Handles live image capture from webcam.
* `plant_classes.txt` – List of supported plant disease classes.
* `dataset/` – Dataset used for training and fine-tuning.
* `images/` – GUI assets, icons, and example plant images.

---

## Project Images

**GSA PlantML GUI:**

---

## Tech Stack

### Frontend (User Interface)

* **CustomTkinter** — Modern Python GUI framework.
* **Pillow (PIL)** — For image handling and display.

### Backend (Core Logic & Model)

* **Python 3.10+**
* **TensorFlow / Keras** — CNN-based plant disease detection model.
* **NumPy** — Data preprocessing and numerical operations.
* **OpenCV** — Camera and image input.

---

## Getting Started

### Prerequisites

* Python 3.10+
* Install packages listed in `requirements.txt`.

---

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/Sai-Deepan/GSA_plantML.git
   cd GSA_plantML
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Ensure the trained model and class list file (`plant_classes.txt`) are in the project directory.

---

### Usage

### 🔑 Setting Up Gemini API Key

1. Go to [Google AI Studio](https://aistudio.google.com/app/apikey) and create an API key.
2. Open Bash and type
```bash
export GOOGLE_API_KEY="YOUR_API_KEY"
```
3. Be careful not to commit your API Key to Github
   
#### Run the Application

```bash
python app.py
```

* Upload or capture a leaf image.
* View the predicted disease and confidence percentage instantly.

---

## Supported Plant Diseases

* Tomato Leaf Blight
* Corn Leaf Spot
* Potato Early Blight
* Healthy Leaf (No Disease)

And 23 other diseases listed in plant_classes.txt file

*(Easily extendable by retraining the model with new datasets.)*

---

## Why GSA PlantML?

GSA PlantML helps farmers and researchers identify plant diseases quickly and accurately — without needing complex lab tools.
It runs offline, making it practical for rural and low-connectivity areas, and can be expanded for various crop types.

## Contributors

* **Deepan Sai** ([skdeepan.sai@gmail.com](mailto:skdeepan.sai@gmail.com))

---

## Contact & Support

For questions, suggestions, or contributions:
Open an issue on GitHub or reach out via email.

---

## License

**GPL-3.0 License**
Copyright (c) 2025 **Deepan Sai**

This project is licensed under the GPL-3.0 License — see the [LICENSE](LICENSE) file for details.
