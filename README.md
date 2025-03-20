# **LSTM-Based Title Generation**

## 📌 Project Overview
This project leverages **Natural Language Processing (NLP)** and **Long Short-Term Memory (LSTM) networks** to generate **titles** based on existing text data. The model is trained on datasets containing video titles from different regions, learning patterns and structures to generate relevant and engaging titles.

## 🚀 Features
- **Dataset Preprocessing**: Cleans and normalizes text, removes punctuation, and maps category names to IDs.
- **Tokenization & Sequence Generation**: Converts text into sequences using n-gram tokenization.
- **LSTM-Based Neural Network**: Uses an LSTM model built with TensorFlow/Keras to learn and generate text sequences.
- **Automated Title Prediction**: Generates new titles based on a given seed word or phrase.

## 📂 Dataset
The model is trained on video title datasets from different regions:
- `USvideos.csv`
- `CAvideos.csv`
- `GBvideos.csv`

Additionally, category mappings are extracted from:
- `US_category_id.json`
- `CA_category_id.json`
- `GB_category_id.json`

## 🛠 Installation & Setup

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/yourusername/lstm-title-generation.git
cd lstm-title-generation
```

### 2️⃣ Install Dependencies
Ensure you have Python **3.8+** installed, then run:
```bash
pip install -r requirements.txt
```

### 3️⃣ Run the Project
To train the model, execute:
```bash
python train.py
```

To generate titles using a trained model:
```bash
python generate.py --seed "Your Seed Text"
```

## 🏗 Project Structure
```
📂 lstm-title-generation
│-- Dataset/
│   ├── USvideos.csv
│   ├── CAvideos.csv
│   ├── GBvideos.csv
│   ├── US_category_id.json
│   ├── CA_category_id.json
│   ├── GB_category_id.json
│-- src/
│   ├── preprocess.py  # Data preprocessing
│   ├── train.py  # Model training
│   ├── generate.py  # Title generation
│-- requirements.txt
│-- README.md
```

## 🔥 Usage Example
To generate a title using the trained model:
```bash
python generate.py --seed "Spiderman"
```
**Output:**
```
Spiderman Returns To The Big Screen
```

## 🛠 Technologies Used
- **Python**
- **TensorFlow/Keras**
- **NumPy & Pandas**
- **LSTM Neural Networks**

## 🤝 Contributing
Pull requests are welcome! For major changes, please open an issue first to discuss what you'd like to change.

---
🚀 **Happy Coding!**
