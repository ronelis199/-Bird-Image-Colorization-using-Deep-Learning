# **Advanced topics in Deep Learning Final Project**

By:\
**Raz Diamond (322281528)**, **Ron Elyashar (209350644)**,\
**Liav Ermias (211684956)** and **Roeeii Itshayek (212210751)**.

In this project, we were tasked with solving a **coloring** problem using methods we have learned over the semester. The
goal is to build a model capable of coloring images from
Kaggle's [20_UK_Garden_Birds](https://www.kaggle.com/datasets/davemahony/20-uk-garden-birds) dataset, which contains
**2,841 images** labeled across **20 classes**.

The assignment consists of two parts:

### **Pt. 1: Naive Image-to-Image Translation Deep Neural Network**

Three **naive DNN experiments** to solve the **coloring** problem.\
[🔗 Training Notebook (Part 1)](https://colab.research.google.com/drive/1tsFcOgRydmz39jILi01OOOYc0dqK1gfw?usp=sharing)\
[🔗 Testing Notebook (Part 1)](https://colab.research.google.com/drive/1uo53rHGtg1xbefcv1gLsO-dWiTX90TBj?usp=sharing)

### **Pt. 2: Image-to-Image Translation with Conditional Adversarial Networks**

Three **cGAN experiments** to solve the **coloring** problem. Inspired by a research paper from Berkeley.\
[🔗 Training Notebook (Part 2)](https://colab.research.google.com/drive/1HUJUY9YvVQKETTJ15odrARgyacliYpfl?usp=sharing)\
[🔗 Testing Notebook (Part 2)](https://colab.research.google.com/drive/1WfIW1RzE31Da0yKr0cYtFnKV_jaWskeV?usp=sharing)

We used the Python programming language, along with TensorFlow, Numpy, and Scikit-Learn. The notebooks were presented
using the Google Colab platform

## Structure of Colab Notebooks:

Each training notebook is divided into 4 sections:

- **Introduction** - Overview, imports, and dataset downloading.
- **Preprocessing** - Processing and preparing the dataset.
- **Experiments** - The three experiments we implemented.
- **Conclusions** - Key notes from this part.

Each testing notebook is a test environment, allowing users to upload an image and test it against our best model.

## Testing Our Implementation

To test our implementation of the assignments in each part:

1. Check the training notebook and the output of the cells.
2. Run the cells in the test notebook to try the best model by yourself.

### **Disclaimer**

Any files saved in the notebook's virtual machine (VM) will be deleted after the session ends.
To ensure persistence, we saved this file ("README.md") and the models (.keras files) in our Google Drive accounts.
These files are shared with anyone who has the links, allowing them to access and use them when running our notebooks.
