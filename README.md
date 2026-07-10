# Sugarcane Leaf Disease Detection

### 📌 Project Overview
Sugarcane is a vital global crop, serving as the primary source for approximately 80% of the world's sugar. In Pakistan, the 7th largest sugar producer, sugarcane diseases significantly impact yield and sugar quality. This project leverages **Computer Vision** and **Deep Learning** algorithms to analyze plant images for the early and timely identification of diseases, allowing farmers to implement control measures and minimize crop losses.

### 📂 Dataset Information
The project utilizes the **Sugarcane Leaf Image Dataset** sourced from Mendeley, consisting of **7,134 images**.

*   **Total Images:** 7,134
*   **Data Split:** 
    *   Training: 4,318 samples
    *   Validation: 1,080 samples
    *   Testing: 1,350 samples
*   **Target Classes (11):** 
    *   Healthy Leaves
    *   Brown Rust
    *   Viral Disease
    *   Dried Leaves
    *   Brown Spot
    *   Sett Rot
    *   Smut
    *   Banded Chlorosis
    *   Pokkah Boeng
    *   Grassy Shoot
    *   Yellow Leaf

### ⚙️ Methodology & Preprocessing
To improve model robustness and generalize performance, the following image augmentation and preprocessing techniques were applied:
*   **Rescale & Shear Transformation**
*   **Zoom**
*   **Horizontal Flip**

### 🤖 Model Training & Performance
Multiple Deep Learning architectures, including custom CNNs and pre-trained models, were evaluated based on their accuracy across various epochs.

| Model | Epochs | Accuracy (%) |
| :--- | :--- | :--- |
| **CNN (v3)** | **100** | **93.78%** |
| CNN (v2) | 100 | 93.19% |
| MobileNetV2 | 50 | 93.11% |
| MobileNetV2 | 100 | 92.81% |
| CNN (v3) | 150 | 92.87% |
| InceptionV3 | 50 | 92.44% |
| CNN (v2) | 50 | 92.37% |
| CNN (v1) | 50 | 85.85% |

🏆 **Best Performing Model:** The **CNN (v3)** architecture achieved the highest accuracy of **93.78%** at 100 epochs.

### 📊 Visualizations
The project includes detailed performance metrics such as:
*   **Confusion Matrices:** To evaluate class-wise prediction accuracy.
*   **ROC Curves:** To analyze the True Positive Rate vs. False Positive Rate for each disease category.
*   **Sample Predictions:** Visualizing identified diseases like Brown Rust, Viral Disease, and Sett Rot.

### 🛠️ Technologies Used
*   **Language:** Python
*   **Frameworks:** TensorFlow / Keras
*   **Architectures:** CNN, MobileNetV2, InceptionV3
*   **Augmentation:** Keras ImageDataGenerator

### 🔗 Data Sources & References
*   [Sugarcane Leaf Disease Dataset - Kaggle](https://www.kaggle.com/datasets/nirmalsankalana/sugarcane-leaf-disease-dataset)
*   [Sugarcane Leaf Dataset - Mendeley](https://doi.org/10.17632/355Y629YNJ.1)
*   [Sugarcane Leaf Image Dataset - Mendeley](https://doi.org/10.17632/355Y629YNJ.1)

### 👨‍💻 Author
**Rafia Tehseen**
