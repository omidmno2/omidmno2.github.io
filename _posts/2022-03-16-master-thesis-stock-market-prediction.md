---
title: "Master’s Thesis: Stock Market Prediction Using Machine Learning and Deep Learning"
layout: post
date: 2022-03-16 11:00
image: /assets/images/markdown.jpg
headerImage: false
category: papers
paper_status: academic
author: Omid
star: false
tags:
- Master_Thesis
- Deep_Learning
- Machine_Learning
- Stock_Market_Forecasting
- Tehran_Stock_Exchange
- LSTM
- CNN
- Candlestick_Chart
- Technical_Analysis
description: "Master’s thesis in Operations Research on stock market prediction using machine learning, deep learning, technical indicators, candlestick charts, LSTM, and CNN-based approaches."
permalink: /master-thesis-stock-market-prediction/
---

## Academic Status

This work was my Master’s thesis in **Industrial Management – Operations Research** at **Kharazmi University**.

**Thesis title:** Stock Market Prediction by Using Machine Learning and Deep Learning Approaches  
**Degree:** Master of Science in Industrial Management, Operations Research  
**University:** Kharazmi University  
**Supervisor:** Dr. Omid Mahdi Ebadati Esfahani  
**Co-supervisor:** Prof. M. Afshar Alam  
**Defense date:** March 16, 2022  
**Final mark:** 18/20  

This thesis later led to three research outputs, including one published paper and two completed research manuscripts. :contentReference[oaicite:0]{index=0}

---

## Overview

This thesis focused on predicting stock market movements in the Tehran Stock Exchange using machine learning and deep learning approaches.

The research explored several ways of representing financial time-series data for predictive modeling, including direct numerical forecasting, technical-indicator-based image generation, candlestick chart image classification, and time-series-to-image conversion techniques.

The central idea was to investigate whether deep learning models could detect nonlinear and hidden patterns in financial data more effectively than traditional approaches.

---

## Research Motivation

Stock market prediction is difficult because financial markets are noisy, nonlinear, and influenced by many external factors.

These factors include:

- political and economic conditions;
- company performance;
- investor behavior;
- market sentiment;
- news and social media;
- structural instability in emerging markets.

The thesis focused on the Tehran Stock Exchange, where volatility, market shocks, and incomplete market maturity make forecasting especially challenging.

The goal was not to build a guaranteed trading system, but to explore whether machine learning and deep learning could provide useful predictive signals for financial decision support.

---

## Research Objectives

The main objective was to design and evaluate machine learning and deep learning approaches for forecasting stock price behavior in the Iranian stock market.

The research aimed to:

- test different deep learning architectures for stock market prediction;
- compare numerical and image-based representations of financial data;
- evaluate LSTM and CNN-based models;
- transform technical indicators into two-dimensional model inputs;
- generate candlestick chart images from historical prices;
- compare different labeling methods;
- assess how preprocessing and data representation affect model performance.

---

## Dataset

The thesis used historical data from the Tehran Stock Exchange.

The research time domain covered the period from **December 6, 2008 to June 28, 2021**, including **3014 trading days**.

The dataset included daily trading variables such as:

- closing price;
- opening price;
- last traded price;
- highest price;
- lowest price;
- trading volume;
- number of trades;
- traded value;
- daily price changes.

Different experiments used different subsets of companies depending on data availability and the requirements of each method.

---

## Methodological Structure

The thesis included several modeling tracks.

### 1. Closing Price Forecasting with LSTM and 1D CNN

The first track focused on predicting stock closing prices using deep learning models designed for sequential data.

This part used:

- one-dimensional convolutional layers;
- Long Short-Term Memory networks;
- sliding-window time-series preparation;
- standardized and non-standardized data comparisons;
- different feature configurations and time windows.

This track later developed into the published paper:

[Deep Learning-Based Price Forecasting in Tehran Stock Exchange: LSTM and 1D CNN Approaches](/LSTM-and-1D-CNN/)

---

### 2. CNN with Technical Indicator Images

The second track transformed technical indicators into two-dimensional image-like matrices.

The idea was to convert numerical financial information into a structure that could be processed by Convolutional Neural Networks.

This method used:

- technical indicators;
- sliding windows;
- image-like matrices;
- Buy / Sell / Hold labels;
- Up / Down labels;
- CNN classification.

This work contributed to the manuscript:

[Predicting Stock Market Movements: Technical Indicators, Image Conversion, and Deep Learning Approaches](/Image-Conversion-Techniques/)

---

### 3. Time-Series Image Conversion with GAF and MTF

The third track used time-series image conversion techniques.

The thesis explored methods such as:

- Gramian Angular Field;
- Markov Transition Field;
- CNN-based classification on transformed time-series images.

The purpose was to test whether financial time series could be represented as images while preserving temporal structure.

This was also part of the image-conversion research manuscript.

---

### 4. Technical Indicators with PCA-Based Dimensionality Reduction

Another track used a larger technical-indicator feature space and applied Principal Component Analysis to reduce dimensionality.

The reduced matrices were then used as CNN inputs.

This method tested whether dimensionality reduction could preserve useful predictive information while reducing computational complexity.

---

### 5. Candlestick Chart Image Classification

The final major track converted historical price data into candlestick chart images.

These images were used as inputs for CNN and transfer learning models, including architectures such as:

- custom CNN;
- VGG16;
- ResNet50;
- InceptionV3.

This work later became the manuscript:

[Candlestick Chart Analysis and Deep Learning Approaches for Predicting Stock Market Trends](/Candlestick-Chart-Analysis/)

---

## Key Results

The thesis produced several experimental findings across the different modeling tracks.

The LSTM and 1D CNN-based closing price forecasting experiments showed promising error levels, with a reported Mean Absolute Error around **0.56** in the thesis abstract. :contentReference[oaicite:1]{index=1}

The technical-indicator image approach showed stronger performance when the problem was framed as **Buy / Sell / Hold** classification, with average accuracy around **92%**, while the simpler **Up / Down** direction task performed much weaker, around the mid-50% range. :contentReference[oaicite:2]{index=2}

The candlestick chart image approach produced moderate validation accuracy. In the thesis abstract, the reported average accuracies for CNN, VGG16, ResNet50, and InceptionV3 were approximately **61.31%**, **60.50%**, **51.75%**, and **59.50%**, respectively. :contentReference[oaicite:3]{index=3}

These results showed that the representation of the prediction problem has a major impact on model performance.

---

## Main Contribution

The main contribution of this thesis was the comparison of several machine learning and deep learning approaches for stock market prediction in the Tehran Stock Exchange.

The thesis connected multiple methodological directions:

- time-series forecasting;
- technical analysis;
- image-based financial data representation;
- candlestick chart classification;
- CNN-based image learning;
- LSTM-based sequential modeling;
- transfer learning;
- dimensionality reduction.

Instead of testing only one model, the research compared several ways of representing financial market data for deep learning.

---

## Research Outputs

This thesis later led to the following research outputs:

1. [Deep Learning-Based Price Forecasting in Tehran Stock Exchange: LSTM and 1D CNN Approaches](/LSTM-and-1D-CNN/)  
   Published paper.

2. [Predicting Stock Market Movements: Technical Indicators, Image Conversion, and Deep Learning Approaches](/Image-Conversion-Techniques/)  
   Completed but unpublished manuscript.

3. [Candlestick Chart Analysis and Deep Learning Approaches for Predicting Stock Market Trends](/Candlestick-Chart-Analysis/)  
   Completed but unpublished manuscript.

---

## Limitations

The thesis should be interpreted as academic research rather than a production-ready trading system.

Main limitations included:

- high volatility in the Iranian stock market;
- market instability during parts of the research period;
- sensitivity to labeling strategies;
- limited evidence of real trading profitability;
- need for stronger out-of-sample and walk-forward validation;
- no full transaction-cost or liquidity analysis;
- computational cost of image generation and deep learning model training.

These limitations are important because high model accuracy in an experimental setting does not automatically translate into profitable or reliable trading decisions.

---

## Future Work

Future research could extend this thesis by:

- combining numerical data with textual news data;
- adding macroeconomic variables such as exchange rate, gold price, oil price, and inflation;
- applying walk-forward validation;
- testing Transformer-based architectures;
- improving explainability of deep learning predictions;
- evaluating trading performance after transaction costs;
- testing the methods across different emerging and mature markets.

---

## Keywords

- Stock Market Forecasting
- Tehran Stock Exchange
- Machine Learning
- Deep Learning
- LSTM
- CNN
- Technical Analysis
- Candlestick Chart
- Image Conversion
- Financial Time Series
- Operations Research

---

## Portfolio Note

This page summarizes my Master’s thesis and its research outputs. The full thesis is an academic document, while the portfolio pages linked above provide shorter summaries of the three main research directions that emerged from it.
