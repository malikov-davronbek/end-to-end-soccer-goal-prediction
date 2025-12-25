# ⚽ Football Goals Prediction (Supervised Regression)

An end-to-end **machine learning project** to predict the **number of goals** using football performance metrics, built with **modular architecture**, **data leakage prevention**, and **production deployment readiness**.

---

## 📌 Table of Contents

- [Project Overview](#project-overview)
- [Features Description](#features-description)
- [Project Workflow](#project-workflow)
- [Modular Structure](#modular-structure)
- [EDA](#eda)
- [Baseline Model](#baseline-model)
- [Model Improvement](#model-improvement)
- [Train / Test Strategy (t &amp; t+1)](#train--test-strategy-t--t1)
- [Avoiding Data Leakage](#avoiding-data-leakage)
- [Model Training &amp; Evaluation](#model-training--evaluation)
- [FastAPI Inference](#fastapi-inference)
- [Dockerization](#dockerization)
- [CI/CD](#cicd)
- [AWS Deployment](#aws-deployment)

---

## 📖 Project Overview

This project predicts **football goals** using a **supervised regression model** based on player match statistics and advanced metrics.

**Goal:**Predict `goals` while ensuring:

- No data leakage
- Time-aware train/test split
- Reproducible ML pipeline
- Production-ready API

---

## 🧾 Features Description

| Feature       | Description                  |
| ------------- | ---------------------------- |
| games         | Matches played               |
| goals         | Goals scored (TARGET)        |
| assists       | Assists                      |
| yellow_cards  | Yellow cards                 |
| red_cards     | Red cards                    |
| position      | Player position              |
| xGChain       | xG involvement in possession |
| xGBuildup     | xG buildup contribution      |
| season        | Season year                  |
| league_weight | League strength              |
| aGg           | Assists per game             |
| gpm / apm     | Goals / assists per minute   |
| shpg / shpm   | Shots per game / minute      |
| kppg / kppm   | Key passes                   |
| ypg / rpm     | Cards per game               |
| xGg           | Expected goals per game      |
| xG            | Expected goals               |

---

## 🔄 Project Workflow

1. Modular Structure
2. EDA
3. Baseline Model
4. Improvement
5. Model Selection
6. API
7. Docker
8. CI/CD
9. AWS Deployment

---

## 🧱 Modular Structure

```text
football-goals-ml/
│
├── data/
│   ├── raw/
│   ├── processed/
│   └── features/
│
├── src/
│   ├── data/
│   ├── features/
│   ├── models/
│   ├── training/
│   ├── evaluation/
│   ├── api/
│   └── utils/
│
├── scripts/
├── notebooks/
├── tests/
├── docker/
└── README.md
```
