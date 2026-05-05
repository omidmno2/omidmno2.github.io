---
title: "Predicting Stock Market Movements: Technical Indicators, Image Conversion, and Deep Learning Approaches"
layout: post
date: 2023-05-01 11:00
image: /assets/images/markdown.jpg
headerImage: false
category: papers
paper_status: manuscript
author: Omid
star: false
tags:
- Deep_Learning
- CNN
- Technical_Indicators
- Image_Conversion
- Stock_Market_Prediction
- Tehran_Stock_Exchange
- GAF
- MTF
- PCA
description: "Completed but unpublished research manuscript on stock market movement prediction using technical indicators, time-series image conversion, PCA, and CNN-based deep learning models."
permalink: /Image-Conversion-Techniques/
---

## Manuscript Status

This work is a completed but unpublished research manuscript.

It explored how stock market data can be transformed into two-dimensional image-like representations and used as input for Convolutional Neural Networks to predict stock movement and trading-action labels in the Tehran Stock Exchange.

This page summarizes the research in a portfolio-friendly format. It is not a published article and should not be cited as a peer-reviewed publication.

---

## Overview

Stock market prediction is a difficult problem because financial markets are noisy, nonlinear, and affected by economic, political, behavioral, and market-specific factors.

This research investigated whether deep learning models could support stock movement prediction by converting financial time-series data into two-dimensional image representations.

Instead of using raw numerical data only, the study tested multiple approaches for preparing CNN-compatible inputs from stock market data.

The research compared three main image-based preparation strategies:

1. technical indicators transformed into 15×15 image-like matrices;
2. time-series image conversion using Gramian Angular Field and Markov Transition Field;
3. technical-indicator matrices reduced with Principal Component Analysis before CNN training.

---

## Research Objective

The main objective was to compare different image-based data representation techniques for predicting stock market movement in the Tehran Stock Exchange.

The study focused on three practical questions:

1. Can technical indicators be converted into image-like structures for CNN-based prediction?
2. Can time-series image conversion methods such as GAF and MTF improve stock movement classification?
3. Does the model perform differently when the target is defined as Buy/Sell/Hold versus simple Up/Down movement?

---

## Dataset

The study used daily stock market data from the Tehran Stock Exchange.

The dataset covered the period from **December 6, 2008 to June 28, 2021**, including daily variables such as:

- closing price;
- opening price;
- last price;
- highest price;
- lowest price;
- trading volume;
- number of trades;
- traded value.

The experiments focused on selected companies with sufficient historical data and more analyzable trading records.

---

## Methodology

The study proposed and compared three main methods for converting financial data into CNN-compatible inputs.

### Method 1: CNN with Technical Indicator Images

The first method used technical indicators and sliding windows to convert numerical financial data into **15×15 image-like matrices**.

Each image was created using a set of technical indicators computed over multiple time intervals.

The selected indicators included common technical-analysis features such as:

- RSI;
- Williams %R;
- moving averages;
- MACD;
- ROC;
- CCI;
- Bollinger Band-related indicators;
- stochastic indicators;
- momentum-based indicators.

The resulting images were used as inputs to a CNN classifier.

---

### Method 2: GAF and MTF Time-Series Image Conversion

The second method used time-series image conversion techniques.

Two approaches were tested:

- **Gramian Angular Field (GAF)**;
- **Markov Transition Field (MTF)**.

These methods transform one-dimensional financial time series into two-dimensional image representations. The goal was to preserve temporal structure in a format that can be processed by a CNN.

In this part of the study, the generated images were used to classify stock movement labels using the same general CNN-based approach.

---

### Method 3: Technical Indicators with PCA-Based Reduction

The third method used a larger set of technical indicators to create two-dimensional matrices, then applied **Principal Component Analysis (PCA)** to reduce the dimensionality.

The purpose of PCA was to reduce computational complexity while preserving the most important information in the feature structure.

The reduced matrices were then used as CNN inputs.

---

## Labelling Strategies

The study compared two different labelling strategies.

### Buy / Sell / Hold Labels

In the first strategy, each observation was labelled as:

- **Buy**;
- **Sell**;
- **Hold**.

This formulation tried to identify trading-action zones rather than only next-day direction.

### Up / Down Labels

In the second strategy, each observation was labelled based on whether the stock price moved up or down on the next trading day.

This created a simpler binary classification task.

The comparison between these two labelling strategies was one of the most important parts of the study.

---

## Model

A Convolutional Neural Network was used for classification.

The general architecture included:

- convolutional layers;
- ReLU activation functions;
- max-pooling;
- dropout layers;
- fully connected layers;
- output layers adapted to the classification task.

The model was implemented in Python using a Jupyter Notebook environment and deep learning libraries such as TensorFlow.

---

## Key Results

The results differed strongly depending on the labelling strategy.

For the **Buy / Sell / Hold** classification setup, the models achieved high validation accuracy across the tested image-conversion methods.

For the **Up / Down** classification setup, the results were much weaker, with validation accuracy around the mid-50% range.

This difference suggests that the way the prediction target is defined can have a major effect on the apparent performance of a financial prediction model.

In other words, the model performed much better when the problem was framed as a trading-action classification problem than when it was framed as a next-day direction prediction problem.

---

## Interpretation

The results should be interpreted carefully.

The high accuracy in Buy/Sell/Hold classification is promising, but it does not automatically mean the model is ready for real trading. Financial prediction models need stronger validation before being used in investment decisions.

Important additional checks would include:

- out-of-sample validation;
- walk-forward testing;
- transaction-cost analysis;
- risk-adjusted performance evaluation;
- comparison with simple trading baselines;
- robustness across different market regimes.

The weaker Up/Down performance also highlights how difficult short-term direction prediction is in noisy financial markets.

---

## Contribution

The main contribution of this manuscript is the comparison of multiple image-based data preparation methods for CNN-based stock market prediction in the Tehran Stock Exchange.

The project connects financial time-series analysis with computer vision techniques by transforming technical indicators and stock-price sequences into structured two-dimensional inputs.

It also shows that model performance is strongly influenced by the choice of labelling strategy, not only by model architecture.

---

## Limitations

This work remained at the manuscript stage and has not been formally published.

The main limitations include:

- no peer-reviewed publication status;
- sensitivity to the labelling method;
- limited evidence for real trading profitability;
- need for stronger out-of-sample validation;
- potential market-regime instability in the Tehran Stock Exchange;
- lack of transaction-cost and liquidity analysis;
- limited interpretability of CNN-based predictions.

The results are useful as a research experiment, but they should not be interpreted as a ready-to-use trading system.

---

## Future Work

Future work could improve the framework by:

- combining technical indicators with textual data from news and financial reports;
- adding macroeconomic variables;
- testing walk-forward validation;
- evaluating transaction costs and realistic trading constraints;
- comparing CNN models with LSTM, Transformer, and hybrid architectures;
- improving explainability of image-based financial predictions;
- testing the framework on different emerging and mature markets.

---

## Keywords

- Tehran Stock Exchange
- Stock Market Prediction
- Technical Indicators
- Image Conversion
- Convolutional Neural Network
- Deep Learning
- Gramian Angular Field
- Markov Transition Field
- Principal Component Analysis
- Financial Time Series

---

## Authors

Hossein Mostafaei Nia, Omid Mahdi Ebadati Esfahani, and M. Afshar Alam
