# AI-Based Test Case Prioritization Using Defect Risk Prediction

This repository contains the implementation and experiments for the research project:

**AI-Based Test Case Prioritization Using Defect Risk Prediction**

📄 Project 2 Preprint (Zenodo DOI): <PASTE_ZENODO_LINK_AFTER_UPLOAD>  
📄 Related Work (Project 1): Software Defect Prediction Using Machine Learning


## Abstract
This project proposes an AI-based test case prioritization approach that integrates machine learning-driven defect risk prediction with test automation. Defect probabilities are first estimated at the module level using static code metrics and then propagated to test cases based on their coverage. Experimental results demonstrate improved fault detection effectiveness compared to baseline execution strategies.


## Dataset
- Source: NASA CM1 dataset (PROMISE repository)
- Modules: 498
- Features: 21 static code metrics
- Test Coverage: Simulated test–module mapping (research-accepted practice)


## Methodology
- Defect prediction using Logistic Regression with class-balanced learning
- Test case risk computation via aggregation of module defect probabilities
- Test prioritization based on descending risk scores
- Evaluation using APFD metric


## Experiments
- Baseline strategies: Original order, Random order
- Proposed strategy: AI-based risk prioritization
- Metric: Average Percentage of Fault Detection (APFD)


## How to Run
bash
pip install -r requirements.txt
