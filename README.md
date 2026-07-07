# Comparative Analysis of Deceptive Job Advertisement Prediction Using Data Mining

An advanced data science implementation evaluating traditional machine learning frameworks and deep learning topologies to proactively identify and mitigate online recruitment scam vectors.

---

## 📝 Project Abstract
With the rapid integration of electronic recruitment media into the global job market, malicious employment scams ("job scams") have drastically increased. These fraudulent activities explicitly target fresh graduates and students to steal critical personal, academic, financial, or tax information. 

This project implements and evaluates an automated multi-model classification system using **KNN, Decision Trees, Support Vector Machines (SVM), Naïve Bayes, Random Forest, Multilayer Perceptron (MLP), and Deep Neural Networks (DNN)**. Rather than relying on computationally heavy Natural Language Processing (NLP) or raw text processing, this model exclusively targets **7 categorical dimensions** extracted from the **Employment Scam Aegean Dataset (EMSCAD)** containing 18,000 samples. 

By eliminating the preprocessing overhead of unstructured text data, this architecture minimizes trainable parameters and training runtimes. Experimental evaluations prove that while conventional machine learning configurations show high precision, our dense **3-layer Deep Neural Network architecture achieves a peak validation accuracy of ~99% and a generalized mean of 97.7%**.

---

## 🔍 System Evolution Analysis

### ❌ The Existing Paradigm (Baseline Works)
Prior models analyzed recruitment security via traditional text analytics models like Online Recruitment Fraud (ORF) frameworks using classifiers such as Zero R, One R, and standard Logistic Regression.
* **Disadvantages:** Traditional architectures are highly susceptible to deceptive textual profiles designed by fraudsters to bypass standard linguistic rules, failing to dynamically flag emerging scam vectors. 
* **Baseline Accuracy:** Standard benchmarks peak at an **89.5% accuracy threshold** when running standard ensemble workflows on balanced text slices.

### 🚀 The Proposed Architecture
Our optimized methodology introduces a hyper-efficient data engineering lifecycle structured around three sequential stages:

```text
[Raw EMSCAD Dataset] 
         │
         ▼
[Stage 1: Pre-processing] ──► Removes structural noise & HTML formatting tag sets
         │
         ▼
[Stage 2: Feature Selection] ──► Extracts 7 core categorical parameters 
         │                        (e.g., telecommuting, company_logo, questions, etc.)
         │
         ▼
[Stage 3: Hybrid Classification] ──► Parallel execution across ML & 3-Layer Dense DNN
