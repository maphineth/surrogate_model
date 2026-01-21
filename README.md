# Surrogate Model Decision Framework

A project for training surrogate models to replace Agent-Based Model (ABM) simulations.

## Overview

This project trains machine learning models to predict ABM output (Cost) from input parameters, helping decide when to use surrogate models instead of full simulations.

## Files

- `train_surrogate_model_decision_framework.ipynb` - Main notebook for training surrogate models
- `200runs_complete.csv` - Dataset with 200 ABM runs
- `400runs_complete.csv` - Dataset with 400 ABM runs
- `800runs_complete.csv` - Dataset with 800 ABM runs
- `1600runs_complete.csv` - Dataset with 1600 ABM runs

## Models

- Decision Tree
- Random Forest
- Gradient Boosted Trees

## Key Metric

**SMBI (Surrogate Model Benefit Indicator)**: 1 - R, where R = n_train / N_total

This metric indicates the fraction of ABM budget saved by using a surrogate model.

## Usage

Open the Jupyter notebook and run the cells to train models on different dataset sizes and evaluate the decision framework.
