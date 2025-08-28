![Python](https://img.shields.io/badge/Python-3.9%2B-blue?logo=python)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.18-orange?logo=tensorflow)
![Keras](https://img.shields.io/badge/Keras-API-red?logo=keras)
![NumPy](https://img.shields.io/badge/NumPy-1.26-013243?logo=numpy)
![Pandas](https://img.shields.io/badge/Pandas-2.0-150458?logo=pandas)
![Scikit--learn](https://img.shields.io/badge/scikit--learn-1.5-F7931E?logo=scikit-learn)
# Deep Learning Exam Implementation

This repository contains the implementation of my Deep Learning exam project for the course Machine Learning, Artificial Neural Networks and Deep Learning (Exam session: June 2025).

I scored full marks on this exam.

## Exam Context  

The exam problem was structured into **six open questions**, covering the entire deep learning pipeline:  

1. **Model** — choice of the most appropriate architecture and rationale  
2. **Input** — preprocessing strategy, input types, shapes, and value domains  
3. **Output** — design of output layers and justification  
4. **Loss** — choice of loss functions and label formatting  
5. **Model Configuration** — layer composition, hyperparameters, and optimization strategy  
6. **Evaluation** — assessing generalization on unseen data  


**Format**:  
- Students first answered these questions in writing, **without access to the dataset**.  
- Afterwards, each student had to deliver a Colab notebook implementation that **faithfully adhered** to their written design choices, with no changes allowed.  


The original exam text is available at:
[Exam text (PDF)](docs/exam_test.pdf)



## My Solution  

- **Model Architecture**  
  Multi-input, multi-output neural network implemented with the **Keras Functional API**.  

- **Inputs**  
  - **Text reviews** → tokenized, padded sequences → Embedding + LSTM branch  
  - **Categorical metadata** → seasons, reviewer continent, hotel popularity quartiles → Dense layers branch  

- **Outputs**  
  - **Binary classification** → Good vs. Bad review (sigmoid activation)  
  - **Regression** → Review score (linear activation)  

- **Loss Functions**  
  - Binary cross-entropy (classification)  
  - Mean Squared Error (regression)  
  - Combined via weighted sum  

- **Optimization**  
  Adam optimizer with tuned hyperparameters: learning rate, dropout, batch size, LSTM units  

- **Evaluation**  
  - Baseline training  
  - Random search for hyperparameter tuning  
  - 5-fold cross-validation to assess generalization  


The original dataset (`input_data.pkl`) is no longer publicly available. (This is why there is not a requirements.txt anymore here)

done by me, ialwayslikedgrime alias grimey_s

let's connect on X ! https://x.com/grimey_s 
