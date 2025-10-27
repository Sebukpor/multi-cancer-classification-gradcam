---

## 🧬 Browser-Based Multi-Cancer Classification Framework Using Depthwise Separable Convolutions for Precision Diagnostics

**Authors:**
Divine Sebukpor, Ikenna Odezuligbo*, Maimuna Nagey, Michael Chukwuka, Oluwamayowa Akinsuyi
(*Corresponding Author*)

🔗 **Preprint DOI:** [https://www.preprints.org/manuscript/202510.1612](https://www.preprints.org/manuscript/202510.1612)
🚀 **Live Demo (Hugging Face Space):** [https://huggingface.co/spaces/Sebukpor/multi-cancer-gradcam](https://huggingface.co/spaces/Sebukpor/multi-cancer-gradcam)

---

### 📖 Overview

This repository documents our published work:
**“Browser-Based Multi-Cancer Classification Framework Using Depthwise Separable Convolutions for Precision Diagnostics.”**

The framework introduces a **unified, browser-accessible AI system** capable of detecting multiple cancer types from **various medical imaging modalities**, including:

* **CT Scans**
* **MRI Images**
* **Histopathology Slides**
* **Ultrasound Images**
* **Microscopic / Dermoscopic Images**

This versatility enables clinicians and researchers to deploy deep learning–based cancer diagnostics without hardware constraints — entirely within a browser interface powered by Hugging Face Spaces.

---

### 🧠 Core Features

* 🧩 **Multi-Modality Support** – Works across diverse medical imaging types (CT, MRI, Histopathology, Ultrasound, etc.)
* 🩺 **Multi-Cancer Detection** – Classifies 26 distinct cancer categories with high precision.
* ⚙️ **Optimized Deep Architecture** – Employs depthwise separable convolutions for speed and efficiency.
* 🔥 **Grad-CAM Visualizations** – Generates interpretability heatmaps showing key diagnostic regions.
* 🌐 **Browser-Based Deployment** – Runs entirely online; no installation or GPU required.
* 💡 **TensorFlow → TensorFlow.js Integration** – Trained in TensorFlow, deployed using TensorFlow.js for web inference.

---

### 🏗️ Model Architecture Summary

* **Base Model:** Xception (Depthwise Separable CNN)
* **Additional Layers:** Batch Normalization, Dropout, and L2 Regularization
* **Output:** 26-class Softmax layer
* **Loss Function:** Categorical Cross-Entropy
* **Optimizer:** Adam (LR scheduling enabled)
* **Performance:**

  * Test Accuracy: **98.69%**
  * Excellent generalization across modalities and cancer classes

---

### 🔬 Grad-CAM Visualization

Grad-CAM integration allows clinicians to **visually interpret** the model’s reasoning by overlaying heatmaps on input images.

**Workflow:**

1. Upload an image (CT, MRI, histopathology, etc.).
2. The model predicts the most probable cancer type.
3. Grad-CAM highlights regions that most influenced the prediction.

---

### 📊 Dataset Overview

The dataset used to train and evaluate this framework contains multimodal medical images across **26 cancer types**.
Each class includes balanced samples from multiple imaging sources.

| Split          | Images per Class | Total Classes | Total Images |
| -------------- | ---------------- | ------------- | ------------ |
| Training Set   | 4000             | 26            | 104,000      |
| Validation Set | 500              | 26            | 13,000       |
| Test Set       | 500–501          | 26            | ≈13,000      |

---

### 🔗 Model & App Access

* **Live Web App:** [https://huggingface.co/spaces/Sebukpor/multi-cancer-gradcam](https://huggingface.co/spaces/Sebukpor/multi-cancer-gradcam)
* **Model Repository:** [https://huggingface.co/Sebukpor/multi-cancer-gradcam](https://huggingface.co/Sebukpor/multi-cancer-gradcam)
  *(Model weights are securely hosted and deployed directly on Hugging Face Spaces.)*

---

### 🧰 Tech Stack

* **Deep Learning:** TensorFlow, Keras
* **Visualization:** OpenCV, Matplotlib, Grad-CAM
* **Deployment:** Hugging Face Spaces (Gradio + FastAPI)
* **Frontend:** Gradio browser interface
* **Backend:** Python 3.10
* **Interoperability:** TensorFlow.js for in-browser inference

---

### ⚙️ Local Setup (Optional)

If you’d like to run the app locally (without model weights):

```bash
# Clone the repository
git clone https://github.com/yourusername/multi-cancer-gradcam.git
cd multi-cancer-gradcam

# Create a virtual environment
python -m venv venv
source venv/bin/activate  # For Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run the app
python app.py
```

> ⚠️ **Note:** Model weights are hosted on Hugging Face.
> To run locally, download the `.h5` model file from the model repository and update the path in `app.py`.

---

### 📚 Citation

If you use this work in your research, please cite:

```bibtex
@article{Sebukpor2025MultiCancer,
  title={Browser-Based Multi-Cancer Classification Framework Using Depthwise Separable Convolutions for Precision Diagnostics},
  author={Divine Sebukpor and Ikenna Odezuligbo and Maimuna Nagey and Michael Chukwuka and Oluwamayowa Akinsuyi},
  year={2025},
  doi={10.20944/preprints202510.1612.v1},
  journal={Preprints.org}
}
```

---

### 🧾 License

This project is released under the **MIT License**.
You are free to use, modify, and distribute it for research and education purposes.

---

### 💬 Contact

For collaborations, partnerships, or research inquiries:

📧 **Divine Sebukpor** — [LinkedIn](https://www.linkedin.com/in/divine-sebukpor-344a19227)
🌍 **DAS MedHub** — [Website](https://www.dasmedhub.com)
