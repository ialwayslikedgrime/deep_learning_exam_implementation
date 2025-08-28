## Deep Learning Exam Implementation

This repository contains the implementation of my Deep Learning exam project for the course Machine Learning, Artificial Neural Networks and Deep Learning (Exam session: June 2025).

I scored full marks on this exam.


## 📄 Exam Context

The exam consisted of a problem structured into six open questions, covering the full modeling pipeline:

	1.	Model — choice of the most appropriate architecture and rationale

	2.	Input — preprocessing strategy, input types, shapes, and value domains

	3.	Output — design of output layers and justification

	4.	Loss — choice of loss functions and label formatting

	5.	Model Configuration — layer composition, hyperparameters, optimization strategy

	6.	Evaluation — assessing generalization on unseen data

Students first answered these questions in writing, with no access to the dataset, then had to deliver a Colab notebook implementation that faithfully adhered to the stated design choices, with no changes allowed afterwards.

The original exam text is available at:
[Exam text (PDF)](docs/exam_test.pdf)


🧠 My Solution

	•	Model Architecture: Multi-input, multi-output neural network (Functional API, Keras)

	•	Inputs:

	•	Text reviews (tokenized, padded sequences → Embedding + LSTM branch)

	•	Categorical metadata (seasons, reviewer continent, hotel popularity quartiles → Dense layers branch)

	•	Outputs:

	•	Binary classification (Good vs. Bad review, sigmoid activation)

	•	Regression (Review score, linear activation)

	•	Loss Functions: Binary cross-entropy + Mean Squared Error (weighted sum)

	•	Optimization: Adam optimizer with tuned hyperparameters (learning rate, dropout, batch size, LSTM units)
	
	•	Evaluation: Baseline training, random search for hyperparameter tuning, and 5-fold cross-validation




The original dataset (`input_data.pkl`) is no longer publicly available. (This is why there is not a requirements.txt anymore here)

done by me, ialwayslikedgrime alias grimey_s
