# **🔬 Análisis de CNN para Detección de Defectos en Impresión 3D**

## **📋 Descripción del Proyecto**
Este repositorio contiene el código completo de mi **Trabajo de Fin de Grado** en el que se implementan y comparan diferentes arquitecturas de **Redes Neuronales Convolucionales (CNN)** para la clasificación automática de defectos en imágenes de superficies fabricadas mediante **manufactura aditiva (impresión 3D)**.

El proyecto utiliza un conjunto de datos de **imágenes 2D de mapas de altura obtenidos mediante escáner láser 🔍** para detectar y clasificar cuatro tipos de condiciones:

- ✅ **OK** – Material correcto  
- ⚠️ **Under** – Falta de material  
- ❌ **Over** – Exceso de material  
- 🔲 **Empty** – Zona vacía  

---

## **🗂️ Estructura del Repositorio**
```text
📁 TFG_MARTIN_LORING/
│
├── 📁 ScratchVPreentrenados/    # Comparación: desde cero vs. preentrenadas
├── 📁 Modelos Preentrenados/    # Evaluación de modelos preentrenados
├── 📁 Hyperparameters/          # Optimización de hiperparámetros
├── 📁 DataAugmentation/         # Técnicas de aumento de datos
├── 📁 CrossValidation/          # Validación cruzada (k-folds, temporal, aleatoria)
├── 📁 datasets/                 # Scripts de carga y preprocesamiento de datos
├── 📁 results/                  # Gráficas, matrices de confusión, curvas ROC
│
├── 📄 requirements.txt          # Dependencias de Python
├── 📄 README.md                 # Este archivo
└── 📄 TFG_MARTIN_LORING.pdf     # Memoria del trabajo
```

## **🚀 Tecnologías y Conceptos Aplicados**

### **Tecnologías**
| **Tecnología**           | **Aplicación**                          |
|---------------------------|-----------------------------------------|
| **Python 🐍**             | **Lenguaje principal**                  |
| **PyTorch 🧠**            | **Framework de deep learning**          |
| **Google Colab ☁️**       | **Entorno de ejecución con GPU**        |
| **Scikit-learn 📊**       | **Métricas y evaluación**               |
| **Matplotlib/Seaborn 📉** | **Visualización de resultados**         |
| **OpenCV 👁️**             | **Procesamiento de imágenes**           |

### **🧠 Conceptos de IA Implementados**
- 🔄 **Transfer Learning** con modelos preentrenados (**ResNet, AlexNet, VGG, Inception, DenseNet, SqueezeNet**)  
- ⚙️ **Optimización de hiperparámetros** (**learning rate, optimizadores: SGD, Adam, Adagrad, Adadelta**)  
- 🌀 **Data Augmentation** con **PyTorch** e **imgaug**  
- 🔁 **Validación cruzada** (**k-folds, temporal y aleatoria**)  
- 📊 **Métricas avanzadas**: **matrices de confusión, curvas ROC (OvR y OvO), precisión, pérdida**  

---

## **📊 Métodos de Evaluación**
Cada experimento incluye:  

| **Métrica**               | **Visualización**                                   |
|----------------------------|-----------------------------------------------------|
| **Precisión y pérdida**    | **Gráficas de evolución durante entrenamiento**     |
| **Matrices de confusión**  | **Análisis detallado por clase**                    |
| **Curvas ROC**             | **Cálculo de AUC por clase**                        |
| **Tiempo de entrenamiento**| **Comparativa de eficiencia**                       |

---

## **🏆 Resultados Destacados**
- ✅ **ResNet18** obtuvo la mejor relación **precisión/tiempo**: ~**84% de precisión en validación**  
- 📈 **Data augmentation** con transformaciones simples **mejoró la generalización**  
- 🔁 **Validación cruzada con k-folds** mostró la mayor **robustez y mejor AUC** en la clasificación crítica (**Under vs Over**)  
- ⚡ **Modelos preentrenados** superaron consistentemente a los entrenados desde cero  

---

## **🎓 Conclusiones**
Este trabajo demostró la viabilidad de usar **redes neuronales convolucionales (CNN)** para la **detección automática de defectos en impresión 3D**, con aplicaciones en:

- ✅ **Control de calidad automatizado en manufactura aditiva**  
- ⚡ **Inspección en línea de piezas impresas**  
- 📊 **Optimización de parámetros de postprocesado (lijado, relleno)**  
- 🔍 **Sistemas de retroalimentación en tiempo real**  

---

## **👨‍🎓 Autor**
**Martín Loring Bueno**  
**Grado en Ingeniería en Tecnologías Industriales**  
**Universidad de Málaga – Junio 2023**  
**Tutores:** *Ezequiel López Rubio e Iván Gómez Gallego*  

📧 **Contacto:** [martin.loringbueno@hotmail.com](mailto:martin.loringbueno@hotmail.coms) · **[LinkedIn](https:/www.linkedin.com/in/martin-loring-bueno-830886233)**
