# How Predictable Are Humans?  
## Establishing a Behavioral Ceiling in Machine Learning

This project predicts human binary decisions in a rule-learning task using behavioral history.

I compared:
- XGBoost
- LSTM
- Q-learning
- Win-Stay-Lose-Shift (WSLS)

using Leave-One-Participant-Out (LOPO) cross-validation.

The best model, XGBoost, achieved:

# AUC-ROC = 0.676 ± 0.001

The project establishes a behavioral predictability ceiling, showing that some human decision behavior remains fundamentally unpredictable from observable history alone.

---

# Key Findings

| Model | AUC-ROC |
|---|---:|
| Chance | 0.500 |
| WSLS | 0.503 |
| Q-learning | 0.512 |
| LSTM | 0.645 |
| XGBoost | **0.676** |

---

# Major Contributions

- Correct episodic preprocessing improved AUC by +0.087
- Compared cognitive, RL, deep learning, and tree-based models
- Identified a behavioral predictability ceiling
- Performed multi-seed validation
- Discovered four behavioral learner types using clustering

---

# Tech Stack

- Python
- XGBoost
- TensorFlow / Keras
- Scikit-learn
- Pandas
- NumPy
- Matplotlib

---

# Repository Structure

```text
src/         -> model training scripts
notebooks/   -> experimentation notebook
figures/     -> plots and visualizations
results/     -> exported metrics
reports/     -> final academic report
```

---

# Dataset

Dataset:
https://huggingface.co/datasets/marcelbinz/badham2017deficits

---

# Results

## Predictability Ceiling

All major model families converged near the same upper bound:

- XGBoost: 0.676
- LSTM: 0.645
- Q-learning: 0.512
- WSLS: 0.503

This suggests the limit is a property of human behavior rather than a limitation of a specific model.

---

# Skills Demonstrated

- Machine Learning
- Sequential Behavioral Modeling
- Feature Engineering
- Cross Validation
- XGBoost
- LSTM
- Reinforcement Learning
- Clustering
- PCA
- Human-Centered AI

---

# Author

Sabeeh Malik Ali Abdul Rahman
