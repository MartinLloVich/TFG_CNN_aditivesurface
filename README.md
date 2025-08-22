# **🔬 CNN Analysis for Defect Detection in 3D Printing**

## **📋 Project Description**
This repository contains the complete code for my **Bachelor’s Thesis**, where different **Convolutional Neural Network (CNN)** architectures are implemented and compared for the automatic classification of defects in images of surfaces produced via **additive manufacturing (3D printing)**.

The project uses a dataset of **2D height map images obtained via laser scanning 🔍** to detect and classify four types of conditions:

- ✅ **OK** – Correct material  
- ⚠️ **Under** – Lack of material  
- ❌ **Over** – Excess material  
- 🔲 **Empty** – Empty area  

---

## **🗂️ Repository Structure**
```text
📁 TFG_MARTIN_LORING/
│
├── 📁 ScratchVPretrained/        # Comparison: from scratch vs. pretrained
├── 📁 PretrainedModels/          # Evaluation of pretrained models
├── 📁 Hyperparameters/           # Hyperparameter optimization
├── 📁 DataAugmentation/          # Data augmentation techniques
├── 📁 CrossValidation/           # Cross-validation (k-folds, temporal, random)
├── 📁 datasets/                  # Data loading and preprocessing scripts
│
├── 📄 requirements.txt           # Python dependencies
├── 📄 README.md                  # This file
└── 📄 TFG_MARTIN_LORING.pdf      # Thesis document
```

## **🚀 Technologies and Applied Concepts**

### **Technologies**
| **Technology**           | **Application**                           |
|---------------------------|------------------------------------------|
| **Python 🐍**             | **Main programming language**            |
| **PyTorch 🧠**            | **Deep learning framework**              |
| **Google Colab ☁️**       | **Execution environment with GPU**       |
| **Scikit-learn 📊**       | **Metrics and evaluation**               |
| **Matplotlib/Seaborn 📉** | **Results visualization**                |
| **OpenCV 👁️**             | **Image processing**                     |

### **🧠 AI Concepts Implemented**
- 🔄 **Transfer Learning** with pretrained models (**ResNet, AlexNet, VGG, Inception, DenseNet, SqueezeNet**)  
- ⚙️ **Hyperparameter optimization** (**learning rate, optimizers: SGD, Adam, Adagrad, Adadelta**)  
- 🌀 **Data Augmentation** using **PyTorch** and **imgaug**  
- 🔁 **Cross-validation** (**k-folds, temporal, and random**)  
- 📊 **Advanced metrics**: **confusion matrices, ROC curves (OvR and OvO), accuracy, loss**  

---

## **📊 Evaluation Methods**
Each experiment includes:  

| **Metric**                | **Visualization**                                   |
|----------------------------|----------------------------------------------------|
| **Accuracy and Loss**      | **Training evolution graphs**                      |
| **Confusion Matrices**     | **Detailed class-wise analysis**                   |
| **ROC Curves**             | **AUC calculation per class**                      |
| **Training Time**          | **Efficiency comparison**                           |

---

## **🏆 Key Results**
- ✅ **ResNet18** achieved the best **accuracy/time ratio**: ~**84% validation accuracy**  
- 📈 **Data augmentation** with simple transformations **improved generalization**  
- 🔁 **K-fold cross-validation** showed the highest **robustness and best AUC** for critical classification (**Under vs Over**)  
- ⚡ **Pretrained models** consistently outperformed models trained from scratch  

---

## **🎓 Conclusions**
This work demonstrated the feasibility of using **convolutional neural networks (CNNs)** for **automatic defect detection in 3D printing**, with applications in:

- ✅ **Automated quality control in additive manufacturing**  
- ⚡ **Inline inspection of printed parts**  
- 📊 **Optimization of post-processing parameters (sanding, filling)**  
- 🔍 **Real-time feedback systems**  

---

## **👨‍🎓 Author**
**Martín Loring Bueno**  
**Bachelor’s in Industrial Technologies Engineering**  
**University of Málaga – June 2023**  
**Supervisors:** *Ezequiel López Rubio and Iván Gómez Gallego*  

📧 **Contact:** [martin.loringbueno@hotmail.com](mailto:martin.loringbueno@hotmail.com) · **[LinkedIn](https://www.linkedin.com/in/martin-loring-bueno-830886233)**
