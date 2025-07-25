📊 Cervical Cancer Detection using IMATX Network and Transfer Learning Approaches
This repository presents a collection of Jupyter Notebooks for cervical cancer classification using deep learning and machine learning methods on the SIPaKMeD dataset. The models include our proposed IMATX Net architecture, as well as transfer learning baselines like InceptionResNetV2 and VGG16. A comparative study of ML and DL techniques is also provided.

🧠 Repository Structure
Notebook Filename	Description
imatx-net-pretrained-inceptionresnetv2-for-cervi.ipynb	Implements the IMATX Net, which integrates Multi-Attention and Pyramidal T-Block modules using InceptionResNetV2 as the backbone for accurate cervical cell classification. Includes performance metrics, heatmaps, and explainability.
tl-ablation-imatx-network-for-cervical.ipynb	Contains ablation study for the IMATX Net, comparing different architectural variants (with/without IMA, T-Blocks) and analyzing their performance contributions.
v2-pretrained-vgg16-for-cervicale.ipynb	Transfer Learning model using VGG16 pretrained weights on the SIPaKMeD dataset. Serves as a benchmark for comparison with IMATX.
sipakmed-comparative-study-ml-dl.ipynb	Comparative evaluation of various ML classifiers (SVM, KNN, Random Forest) and DL architectures. Helps understand baseline performance across traditional vs. deep methods.

📌 Key Highlights
Dataset: SIPaKMeD (Single-cell Pap smear images)

Classification: 5-class cervical cell classification

Backbones Used: InceptionResNetV2, VGG16, DenseNet variants

Techniques Used: Multi-Attention (IMA), Pyramidal T-Blocks, Transfer Learning, Ablation Studies

📈 Performance Summary
📌 IMATX NET Metrics (Average over 5 folds)
Metric	Accuracy	Jaccard Similarity	Cohen's Kappa
Mean	0.9724	0.945	0.942
Std. Dev	0.001	0.0015	0.0014
Min	0.971	0.943	0.940
Max	0.974	0.947	0.944

📊 Comparative Performance Table
Method	Accuracy	Precision	F1 Score	Sensitivity	Specificity
IMATX NET (Proposed)	0.972	0.976	0.973	0.970	0.971
Abdalla et al. [20]	0.902	0.904	0.923	0.934	0.905
Pacal & Kılıcarslan [1]	0.893	0.858	0.890	0.890	0.827
Habtemariam et al. [18]	0.821	0.825	0.804	0.804	0.713
Fei M. et al. [21]	0.8526	0.8314	0.8416	0.8348	NA
Tanimu et al. [19]	0.821	0.825	0.804	0.825	0.713

🚀 How to Use
Clone the repository:

bash
Copy
Edit
git clone https://github.com/yourusername/cervical-imatx-net.git
cd cervical-imatx-net
Install requirements:

bash
Copy
Edit
pip install -r requirements.txt
Open any .ipynb notebook in Jupyter or Google Colab and run all cells.


📬 Contact
For collaboration or queries, reach out to:

Tathagat Banerjee
[Your Email or LinkedIn]
Indian Institute of Technology, Patna
