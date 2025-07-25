# IMATX Net - Integrated Multi-Attention Transformer for Cervical Cancer Classification

## 🌐 Overview

IMATX Net is a novel deep learning architecture tailored for cervical cancer classification using advanced attention mechanisms and pyramidal T-block modules. It synergizes DenseNet-169 as the backbone with an Integrated Multi-Attention (IMA) layer and stacked dilated convolutions to efficiently extract robust features from medical images while enhancing diagnostic performance.

The proposed method prioritizes medically relevant areas in cytological slides and addresses the challenges of high variability in sample morphology and texture.

---

## 🧠 Architecture

The IMATX architecture is composed of:

- **Backbone**: DenseNet-169 for hierarchical feature extraction
- **T-blocks**: Three sequential pyramidal blocks with increasing filters (64, 128, 256) applying standard and dilated convolutions for contextual information capture
- **IMA Layer**: Integrated Multi-Attention module designed to filter out irrelevant background and focus on diagnostic features
- **Decoder Head**: Final classification layers with ReLU, batch normalization, and softmax output

---

## 📊 Performance Summary

### 🔍 Metric Summary (Cross-Validation)

| Metric              | Accuracy | Jaccard Similarity | Cohen’s Kappa |
|---------------------|----------|---------------------|----------------|
| **Mean**            | 0.9724   | 0.945               | 0.942          |
| **Standard Deviation** | 0.001 | 0.0015              | 0.0014         |
| **Variance**        | 0.000001 | 2.25E-06            | 1.96E-06       |
| **Minimum**         | 0.971    | 0.943               | 0.940          |
| **Maximum**         | 0.974    | 0.947               | 0.944          |
| **Range**           | 0.003    | 0.004               | 0.004          |
| **Median (Q2)**     | 0.972    | 0.945               | 0.942          |
| **1st Quartile (Q1)** | 0.9715 | 0.944               | 0.9405         |
| **3rd Quartile (Q3)** | 0.9735 | 0.9465              | 0.9435         |

---

### 📈 Benchmark Comparison

| Metric     | **IMATX Net** | Musa et al. [20] | Pacal & Kılıcarslan [1] | Habtemariam et al. [18] | Fei et al. [21] | Tanimu et al. [19] |
|------------|---------------|------------------|--------------------------|--------------------------|------------------|---------------------|
| Sensitivity | **0.97**     | 0.934            | 0.89                     | 0.804                    | 0.8348           | 0.825               |
| Specificity | **0.971**    | 0.905            | 0.827                    | 0.713                    | N/A              | 0.713               |
| Accuracy    | **0.972**    | 0.902            | 0.893                    | 0.821                    | 0.8526           | 0.821               |
| Precision   | **0.976**    | 0.904            | 0.858                    | 0.825                    | 0.8314           | 0.825               |
| F1 Score    | **0.973**    | 0.923            | 0.89                     | 0.804                    | 0.8416           | 0.804               |

---

## 🏗️ Installation & Usage

### ⚙️ Requirements

- Python >= 3.8  
- TensorFlow or PyTorch  
- NumPy, Pandas, Seaborn, Matplotlib  
- OpenCV for preprocessing  

```bash
pip install -r requirements.txt



🧪 Ablation Study Highlights
DenseNet169 alone: Accuracy 93.89%, F1-score 0.9413

Inception + ResNetV2: Accuracy 96.17%, F1-score 0.9629

IMATX Net (Full): Accuracy 97.20%, F1-score 0.9730

Parallel T blocks (without IMA): Significant performance drop (F1-score: 0.8226, Accuracy: 81.37%)

🩺 Why Cervical Cancer?
Cervical cancer is the fourth most common cancer in women worldwide, responsible for over 300,000 deaths annually (WHO, 2023). Early detection through cytological imaging plays a crucial role in survival, and machine learning (ML) combined with deep learning (DL) architectures can revolutionize automated screening.

IMATX Net helps reduce human error, enhance visual attention on clinically relevant areas, and improve classification accuracy for better diagnostics.

📚 Citation
If you use this repository in your research or work, please cite:

pgsql
Copy
Edit
@article{yourname2025IMATX,
  title={IMATX Net: A Novel Deep Learning Network for Cervical Cancer Classification using Integrated Multi-Attention and T-blocks},
  author={Your Name et al.},
  journal={Medical Imaging and Diagnostics},
  year={2025}
}
🤝 Contributing
Contributions are welcome. Please fork the repo and open a pull request.

📬 Contact
For questions or collaborations, contact:
Tathagat Banerjee
📧 tathagatbanerjee@example.com
📍 IIT Patna

🧠 Acknowledgments
Thanks to the open-source community and researchers contributing to cervical cancer datasets and attention-based network designs.
