# ECEN758

This is Course Project for doing classification on [mnist-fashion](https://github.com/zalandoresearch/fashion-mnist) dataset.
## Run code for scoring
The environemnt is well configured in Colab. Please use the [link](https://colab.research.google.com/drive/13NHcv7iiZGY84wxIQ4RBL18D_W5axF7M?usp=sharing) for testing the code. The code is the same as /src/main_for_scoring.ipynb. **Please make sure the GPU is used in Colab by clicking Edit->Notebook Settings->T4 GPU.**

## Code Files Introduction
- src/main_cv.ipynb: This is the integrated code with cross validation. (It takes long time to run).
- src/main_for_scoring.ipynb: This is the code for scoring, which has the basic training, validation, and testing function.
- src/data_exploration.ipynb: This is the code for Exploratory Data Analysis.


## Environment Configuration

1. install conda environment

```
conda create --name fashion python=3.10
conda activate fashion
#install torch=2.1.0 py=3.10 cuda=11.8 cudnn=8.7.0
conda install pytorch torchvision torchaudio pytorch-cuda=11.8 -c pytorch -c nvidia
conda install -c anaconda jupyter
```
2. install packages
```
pip install -U scikit-learn
pip install grad-cam
```

## Grading Rubic (Checklist)

1. Data Preparation (10 points)

* [x] Data cleansing and transformation (5 points)
* [x] Data splitting (i.e., training, validation, and test splits) (5 points)

2. Exploratory Data Analysis (EDA) (10 points)

* [x] Descriptive statistics (e.g., class distributions, data statistics) (5 points)
* [x] Data visualization (e.g., plot examples from classes, dimensionality reduction approach to show data) (5 points)

3. Model Selection (20 points)

* [x] Algorithm selection: Justification for choosing specific data mining algorithm (e.g., decision trees, KNN, neural networks, etc.). (5 points)
* [x] Model building: Developing and tuning selected model (e.g., hyperparameter tuning) (10 points)
* [x] Model evaluation: Proper evaluation metrics (e.g., accuracy, precision, recall, F1-score) and qualitative analysis (e.g., confusion matrices) for classification on test set. (5 points)

4. Code and Software (10 points)

* [x] Code quality (i.e., well-documented, readable, and structured code) (5 points)
* [x] Ability to run code (5 points)

5. Collaboration (10 points)

* [x] Teamwork: Each individual will provide a ranking for their team members: excellent, very good, satisfactory, needs improvement, and unsatisfactory. Justification will be needed for rankings less than satisfactory. This will be submitted individually on Canvas. (5 points per team member)

6. Interpretability (10 point)

* [x] Model interpretablity: Demonstrating an understanding of how the model makes predictions (e.g., feature importance). (5 points)
* [x] Business insights: Discussion of the practical implications of this work for a clothing company. (5 points)

7. Project Report (30 points)

* [x] This component will be graded based on the requirements outlined above.

8. (Optional) Accessible Work (5 points)

* [x] Website or blog post to share work completed on project.

