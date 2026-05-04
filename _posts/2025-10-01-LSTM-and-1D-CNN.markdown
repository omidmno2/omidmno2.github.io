---
title: "Deep Learning-Based Price Forecasting in Tehran Stock Exchange: LSTM and 1D CNN Approaches"
layout: post
date: 2025-10-01 11:00
image: /assets/images/markdown.jpg
headerImage: false
tag:
- LSTM
- 1D_CNN
- Deep_Learning
- Time_Series
- Stock_Market_Forecasting
- Tehran_Stock_Exchange
category: papers
author: Omid
description: Published research paper on deep learning-based stock price forecasting using LSTM and 1D CNN models in the Tehran Stock Exchange.
permalink: /LSTM-and-1D-CNN/
---

## Publication Status

This article has been published in *Advances in Finance and Investment*.

**Full title:** Deep learning-based price forecasting in Tehran Stock Exchange: LSTM and 1D CNN approaches  
**Authors:** Hossein Mostafaei Nia, Kaebeh Yaeghoobi, and Omid Mahdi Ebadati Esfahani  
**Journal:** Advances in Finance and Investment  
**Volume / Issue:** 6(3)  
**Pages:** 1–40  
**Year:** 2025  
**DOI:** [10.71729/afi.2025.1205282](https://doi.org/10.71729/afi.2025.1205282)  
**ResearchGate:** [View publication](https://www.researchgate.net/publication/396561253_Deep_learning-based_price_forecasting_in_Tehran_Stock_Exchange_LSTM_and_1D_CNN_approaches)

---

## Overview

Forecasting stock prices in volatile and emerging markets is a challenging time-series problem. The Tehran Stock Exchange is affected by non-linear price behavior, market noise, incomplete data, and structural instability, which makes traditional forecasting models less reliable in many scenarios.

This study developed a deep learning framework for next-day closing price prediction in the Tehran Stock Exchange by combining **one-dimensional Convolutional Neural Networks (1D CNNs)** and **Long Short-Term Memory networks (LSTMs)**. The model was designed to capture both short-term local price patterns and longer temporal dependencies in financial time series.

The research focused on symbol-level forecasting rather than only aggregate market-index prediction, making the framework more relevant for stock-specific analysis and decision-support applications.

---

## Research Objective

The main objective of this study was to design and evaluate a hybrid deep learning model capable of forecasting the next-day closing price of stocks listed on the Tehran Stock Exchange.

The study aimed to answer three practical questions:

1. Can a hybrid CNN-LSTM architecture improve forecasting accuracy in a volatile emerging market?
2. How does preprocessing, especially standardization, affect prediction stability?
3. Can the model remain robust under different data scenarios, including noisy, incomplete, or structurally changing market conditions?

---

## Methodology

The study used historical trading data from the Tehran Stock Exchange covering the period from **2008 to 2021**, including **3014 trading days**. The dataset included daily trading variables such as closing price, opening price, high price, low price, trading volume, and transaction value.

After data cleaning, anomaly removal, and normalization, the time series was reconstructed using a **sliding window** approach. In this structure, the model used previous observations to predict the following day’s closing price.

The proposed architecture included:

- a **1D CNN layer** to extract short-term local patterns from sequential price data;
- **stacked LSTM layers** to learn temporal dependencies across time;
- dense layers to refine the learned representation;
- a final linear output layer to predict the next closing price.

The model was implemented in Python using **TensorFlow** and **Keras**.

---

## Key Results

The hybrid CNN-LSTM model showed stable performance across different experimental scenarios. On daily Tehran Stock Exchange data, the model achieved:

- **Mean Absolute Error (MAE):** approximately 0.56 to 0.63  
- **Mean Absolute Percentage Error (MAPE):** approximately 1.26% to 1.46%

The results showed that standardization played an important role in improving model stability. The CNN component helped capture short-term price patterns, while the LSTM component supported the learning of longer-term temporal dependencies.

The study also found that closing price was one of the most reliable input features compared with more volatile derived features such as percentage changes.

---

## Robustness and Generalization

To evaluate the adaptability of the model, several experimental scenarios were tested, including:

- full versus trimmed datasets;
- different feature configurations;
- different train-validation splits;
- exclusion of volatile periods;
- comparison across Iranian and non-Iranian market data;
- recursive multi-step forecasting.

The model also showed potential for medium-term forecasting. In recursive forecasting scenarios, it maintained realistic trend continuity for prediction horizons of up to 60 days.

---

## Contribution

The main contribution of this research is the development of a practical deep learning framework for stock-level price forecasting in the Tehran Stock Exchange.

Unlike studies focused only on broad market indices, this research emphasized individual stock-level forecasting, scenario testing, and robustness under noisy or incomplete market data. This makes the framework relevant for researchers, analysts, and investors interested in applying AI-driven forecasting methods in emerging financial markets.

---

## Keywords

- Tehran Stock Exchange
- Stock Market Forecasting
- Long Short-Term Memory
- 1D Convolutional Neural Network
- Deep Learning
- Time Series Forecasting
- Financial Prediction

---

## Citation

Mostafaei Nia, H., Yaeghoobi, K., & Ebadati Esfahani, O. M. (2025). *Deep learning-based price forecasting in Tehran Stock Exchange: LSTM and 1D CNN approaches*. Advances in Finance and Investment, 6(3), 1–40. https://doi.org/10.71729/afi.2025.1205282
