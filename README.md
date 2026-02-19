

# 🍕 Food-101 Image Classifier — Powered by ViT & LoRA

Welcome to the **Food-101 Image Classifier**! 🚀

This project leverages the power of **Vision Transformer (ViT)**, fine-tuned with **LoRA (Low-Rank Adaptation)**, to deliver fast and accurate food image classification. Whether you're a food blogger, a developer, or just curious, this tool lets you explore the world of AI-powered food recognition in a fun and interactive way!

---

## ✨ Features

- **Vision Transformer (ViT) Backbone:**
  - Utilizes `google/vit-base-patch16-224` for state-of-the-art image understanding.
- **LoRA Fine-Tuning:**
  - Efficient adaptation with Low-Rank Adaptation (LoRA) for faster, lighter training and inference.
- **101 Food Categories:**
  - Recognizes a wide range of dishes, desserts, and cuisines from the Food-101 dataset.
- **Streamlit Web App:**
  - Modern, interactive UI for easy image upload and instant classification.
- **Top-K Predictions:**
  - Displays the most probable classes with confidence bars for transparency.
- **Auto Model Download:**
  - No manual hassle — the model is fetched automatically on first run.
- **Fast CPU Inference:**
  - Optimized for both CPU and GPU, with quick predictions (2-5 seconds on CPU).

---

---



## 🛠️ Tech Stack

| Model | Training | Dataset | App |
|-------|----------|---------|-----|
| ViT (Hugging Face Transformers) | LoRA (PEFT) | Food-101 | Streamlit |

---

---

## 🚦 **Quick Start Guide**




1️⃣ **Clone the Repo:**
```bash
git clone https://github.com/AsfandAhmed3/FineTunedViT-FoodClassifier.git
cd FineTunedViT-FoodClassifier
```

2️⃣ **Install Requirements:**
```bash
pip install -r requirements.txt
```



3️⃣ **Download the Model:**
*No hassle!* The app auto-downloads the model on first run. Or, grab it from [Releases](https://github.com/AsfandAhmed3/FineTunedViT-FoodClassifier/releases) and place `final_model.pkl` in a `final_model/` folder.

4️⃣ **Launch the App:**
```bash
streamlit run streamlit_app.py
```
Open [http://localhost:8501](http://localhost:8501) in your browser and start classifying!

---



## 🧬 Model & Training Details

- **Base Model:** `google/vit-base-patch16-224`
- **Fine-tuning Method:** LoRA (Low-Rank Adaptation) via Hugging Face PEFT
- **Dataset:** Food-101 (20% subset for faster experimentation)
- **Number of Classes:** 101 food categories
- **Training Configuration:**
  - LoRA Rank: 16
  - LoRA Alpha: 32
  - Learning Rate: 2e-4
  - Batch Size: 32
  - Epochs: 5
  - Precision: FP16 (mixed precision)

---

---



## 🍽️ Food Categories

The model can classify 101 different food categories, including:
- Pizza, Sushi, Tacos, Hamburger
- Apple Pie, Cheesecake, Chocolate Cake
- Spaghetti Carbonara, Pad Thai, Ramen
- ...and 92 more delicious dishes!

See the [Food-101 dataset](https://www.vision.ee.ethz.ch/datasets_extra/food-101/) for the full list.

---

---



## 🗂️ Project Structure

```text
Task3/
├── streamlit_app.py              # Streamlit web app
├── FineTunedViT-FoodClassifier.ipynb  # Model training & fine-tuning notebook
├── requirements.txt              # Python dependencies
├── final_model/                  # Model weights (auto-downloaded)
│   └── final_model.pkl
└── README.md                     # This file
```

---

---



## 🌐 Deploy to Streamlit Cloud



1. Go to [share.streamlit.io](https://share.streamlit.io)
2. Sign in with your GitHub account
3. Click **"New app"**
4. Fill in:
  - **Repository**: `AsfandAhmed3/FineTunedViT-FoodClassifier`
  - **Branch**: `main`
  - **Main file path**: `streamlit_app.py`
5. Click **"Deploy!"**


The app will automatically download the model from your GitHub release on first launch!

---

---



## 📦 GitHub Release Info



The trained model is available as a GitHub Release to keep the repository size small.

- **Release URL**: https://github.com/AsfandAhmed3/FineTunedViT-FoodClassifier/releases
- **Model File**: `final_model.pkl` (~340 MB)
- **Auto-download**: The Streamlit app automatically downloads the model on first run

---

---



## 💡 Usage

1. **Upload an Image:** Click "Choose a food image..." and select a food photo
2. **Classify:** Click the "🔍 Classify Image" button
3. **View Results:** See top predictions with confidence scores

---

---



## 🔧 Troubleshooting



**Model download fails:**
- Check your internet connection
- Manually download from [Releases](https://github.com/AsfandAhmed3/FineTunedViT-FoodClassifier/releases)
- Place it in the `final_model/` folder

**Out of memory:**
- The app runs on CPU by default
- Ensure you have at least 2GB of free RAM

**Slow predictions:**
- First prediction is slower due to model loading (cached afterward)
- CPU inference takes 2-5 seconds per image

---

---



## 📄 License

This project uses the Food-101 dataset and pre-trained models from Hugging Face.

---

---



## 🙏 Acknowledgments

- Food-101 Dataset
- Hugging Face Transformers
- Microsoft PEFT (LoRA)
- Streamlit

---

---



## 📧 Contact



For questions or issues, please open an issue on the GitHub repo: https://github.com/AsfandAhmed3/FineTunedViT-FoodClassifier/issues

---


<div align="center">
  <strong>Built with ❤️ using Vision Transformer (ViT) + LoRA</strong>
  <br><br>
  <img src="https://em-content.zobj.net/source/microsoft-teams/363/chef_1f9d1-200d-1f373.png" width="40"/>
  <h3>Bon Appétit!<br>— <span style="color:#ff6600;">Asfand Ahmed</span> 🍽️</h3>
  <br><br>
  <p>👨‍💻 Crafted with passion by<br>
  ✨ <b>Asfand Ahmed</b> ✨<br>
  Thanks for checking out this project! !<br>
  </p>
</div>
