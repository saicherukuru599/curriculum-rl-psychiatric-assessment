# Curriculum Reinforcement Learning for Psychiatric Assessment

AI-powered Curriculum Reinforcement Learning framework for adaptive psychiatric assessment and intelligent treatment recommendation using Dueling DQN, Gymnasium, and PyTorch.

![Banner](images/banner.png)

---

## Overview

This project presents a Curriculum Reinforcement Learning (Curriculum RL) system designed for psychiatric assessment and adaptive intervention recommendation. The framework combines reinforcement learning, curriculum learning, and deep neural networks to simulate intelligent clinical decision-making.

The system trains an RL agent in a custom psychiatric environment where patient states evolve dynamically based on treatment actions. A curriculum learning strategy is applied to gradually increase the complexity of patient cases during training, improving stability and learning efficiency.

The project demonstrates how AI can support adaptive psychiatric treatment planning using reinforcement learning-based policies.

---

## Key Features

- Custom Psychiatric Reinforcement Learning Environment
- Curriculum Learning-based Training Pipeline
- Dueling Deep Q-Network (DQN)
- Adaptive Treatment Recommendation System
- Dynamic Reward-based Learning
- Severity Classification (Stable / Moderate / Critical)
- Policy Evaluation & Performance Analysis
- PyTorch-based Deep Learning Architecture
- Training Visualization & Metrics

---

## System Architecture

The complete pipeline follows the architecture below:

```text
Patient Data
     ↓
Psychiatric Environment
     ↓
Curriculum Learning Manager
     ↓
Dueling DQN Agent
     ↓
Policy Optimization
     ↓
Treatment Recommendation
```

---

## Technologies Used

| Technology | Purpose |
|------------|---------|
| Python | Core Development |
| PyTorch | Deep Learning |
| Gymnasium | RL Environment |
| NumPy | Numerical Operations |
| Pandas | Data Processing |
| Matplotlib | Visualization |
| Scikit-learn | Evaluation Metrics |

---

## Reinforcement Learning Pipeline

### Environment
A custom psychiatric simulation environment was developed using Gymnasium.

### Agent
A Dueling DQN agent learns optimal intervention policies based on patient states and rewards.

### Curriculum Learning
The system gradually introduces more difficult patient conditions during training:
- Stable Cases
- Moderate Cases
- Critical Cases

### Reward Function
Rewards are assigned based on:
- Symptom severity reduction
- Clinical improvement
- Treatment effectiveness

---

## Dataset Information

The project utilizes a psychiatric simulation dataset containing patient-related health indicators such as:

- Age
- Affect Dysregulation
- Symptom Severity
- BMI

The dataset is normalized and processed before training the RL agent.

---

## Treatment Actions

| Action ID | Treatment |
|-----------|-----------|
| 0 | Monitoring |
| 1 | Medication |
| 2 | Advanced Treatment |

---

## Severity Classification

| Severity Level | Threshold |
|----------------|-----------|
| Stable | < 0.40 |
| Moderate | 0.40 - 0.70 |
| Critical | > 0.70 |

---

## Training Results

The Curriculum RL framework demonstrated improved performance over traditional rule-based approaches.

### Performance Highlights
- Improved intervention recommendation accuracy
- Better handling of critical psychiatric conditions
- Stable learning through curriculum training
- Effective policy generalization

---

## Sample Output

```text
Patient Profile:
Age: 45
BP: 180 mmHg
Symptom Severity: 189
BMI: 21

Condition: CRITICAL
Recommended Treatment: Medication
Improvement: 5.00%
```

---

## Project Structure

```text
curriculum-rl-psychiatric-assessment/
│
├── README.md
├── requirements.txt
├── LICENSE
├── notebook/
│   └── Curriculum_RL_Psychiatric_Assessment.ipynb
│
├── images/
│   ├── banner.png
│   ├── architecture.png
│   ├── results.png
│   └── training_graph.png
│
├── models/
│   └── trained_model.pth
│
└── src/
    ├── environment.py
    ├── agent.py
    ├── curriculum.py
    ├── train.py
    └── evaluate.py
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/curriculum-rl-psychiatric-assessment.git
```

Move into the project folder:

```bash
cd curriculum-rl-psychiatric-assessment
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Running the Project

Run the notebook:

```bash
jupyter notebook
```

Or execute training scripts:

```bash
python train.py
```

---

## Future Improvements

- Multi-step RL Planning
- Real Clinical Dataset Integration
- Explainable AI for Medical Decisions
- Transformer-based Policy Networks
- Federated Learning Integration
- Real-time Clinical Deployment
- Telepsychiatry Integration

---

## Research Motivation

Traditional psychiatric assessment systems rely heavily on static rules and manual evaluation. This project explores how Reinforcement Learning can enable adaptive, data-driven, and sequential clinical decision-making systems capable of improving treatment personalization.

---

## Author

Cherukuru Muni Sai Balaji  
Artificial Intelligence & Machine Learning  
Dayananda Sagar University

---

## License

This project is licensed under the MIT License.

---

## References

- Sutton & Barto — Reinforcement Learning: An Introduction
- PyTorch Documentation
- Gymnasium Documentation
- Curriculum Reinforcement Learning Research Papers
- Healthcare Reinforcement Learning Literature

---

## Acknowledgement

This project was developed as part of an academic research initiative focused on Reinforcement Learning applications in healthcare and psychiatric assessment. :contentReference[oaicite:0]{index=0}
