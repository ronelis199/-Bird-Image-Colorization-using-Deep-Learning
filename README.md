## 📘 Advanced Topics in Deep Learning – Final Project

By:  
Raz Diamond (322281528), Ron Elyashar (209350644),  
Liav Ermias (211684956), Roeeii Itshayek (212210751)  
Course: Basics of Deep Learning, Colman, 2025

---

## 🎯 Project Goal

The task was to solve an **image colorization problem** using deep learning methods taught during the semester.  
We aimed to develop a model that can automatically colorize grayscale bird images from the [20_UK_Garden_Birds](https://www.kaggle.com/datasets/gpiosenka/20-bird-species) dataset.

The dataset contains 2,841 images across 20 bird species. Each image was converted to grayscale (1 channel) as input and matched with its RGB version (3 channels) as the output.

---

## 📁 Dataset & Preprocessing

- Train/Validation/Test split: 70% / 10% / 20%
- Images resized to 128×128
- Data Augmentation: `RandomZoom`, `RandomRotation` from Keras

---

## 🧪 Project Structure

The project was divided into two main parts:

---

### 🧠 Part 1: Naive Deep Neural Networks

We explored **three different architectures** for direct grayscale-to-color translation:

1. **Fully Connected Neural Network (FCNN)** – served as a baseline  
2. **Convolutional Neural Network (CNN)** – better spatial feature extraction  
3. **U-Net** – encoder-decoder with skip connections for superior performance

📎 **Notebooks:**
- [🔗 Training Notebook (Naive)](https://nbviewer.org/github/ronelis199/-Bird-Image-Colorization-using-Deep-Learning/blob/main/final_project_atdl_method1_train_env.ipynb)
- [🔗 Testing Notebook (Naive)](https://nbviewer.org/github/ronelis199/-Bird-Image-Colorization-using-Deep-Learning/blob/main/final_project_atdl_method1_test_env.ipynb)

**Best Result (Naive):**  
The U-Net model showed the best results among the naive methods.

---

### ⚡ Part 2: Conditional GAN (cGAN)

Inspired by [Pix2Pix paper (Isola et al.)](https://arxiv.org/pdf/1611.07004), we implemented three cGAN variations:

1. **Basic cGAN** – simple CNN generator & discriminator  
2. **cGAN with MAE & CCE loss** – improved generation quality  
3. **U-Net Generator + PatchGAN Discriminator** – state-of-the-art approach

📎 **Notebooks:**
- [🔗 Training Notebook (cGAN)](https://nbviewer.org/github/ronelis199/-Bird-Image-Colorization-using-Deep-Learning/blob/main/final_project_atdl_method2_train_env.ipynb)
- [🔗 Testing Notebook (cGAN)](https://nbviewer.org/github/ronelis199/-Bird-Image-Colorization-using-Deep-Learning/blob/main/final_project_atdl_method2_test_env.ipynb)

**Best Result (Overall):**  
The **second cGAN model (with MAE+CCE loss)** outperformed all others in visual quality and MSE.

---

## 🧪 How to Run the Project

To test the models yourself:

1. Open the relevant **training notebook** and explore the experiments
2. Open the **testing notebook**, upload a grayscale image, and see the colored output from our best model

---

## 🛠 Technologies Used

- Python
- TensorFlow / Keras
- NumPy
- Scikit-learn
- Google Colab

---

## 📂 File Structure

```
Bird-Image-Colorization/
│
├── final_project_atdl_method1_train_env.ipynb      # Part 1 - Naive Training
├── final_project_atdl_method1_test_env.ipynb       # Part 1 - Naive Testing
├── final_project_atdl_method2_train_env.ipynb      # Part 2 - cGAN Training
├── final_project_atdl_method2_test_env.ipynb       # Part 2 - cGAN Testing
└── README.md
```

---

## 🚨 Disclaimer

> Files saved in the Colab virtual machine are deleted after the session ends.  
> Our models (`.keras` files) and notebooks are shared via GitHub and Google Drive for persistence.
