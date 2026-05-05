---
title: "Candlestick Chart Analysis and Deep Learning Approaches for Predicting Stock Market Trends"
layout: post
date: 2023-06-01 11:00
image: /assets/images/markdown.jpg
headerImage: false
category: papers
paper_status: manuscript
author: Omid
star: false
tags:
- Deep_Learning
- CNN
- Transfer_Learning
- Candlestick_Chart
- Stock_Market_Prediction
- Tehran_Stock_Exchange
- Image_Classification
description: "Completed but unpublished research manuscript on stock market trend prediction using candlestick chart images, CNN models, and transfer learning approaches."
permalink: /Candlestick-Chart-Analysis/
---

## Manuscript Status

This work is a completed but unpublished research manuscript.

It explored the use of candlestick chart images and deep learning models to predict stock market movement trends in the Tehran Stock Exchange.

This page summarizes the research in a portfolio-friendly format. It is not a published article and should not be cited as a peer-reviewed publication.

---

## Overview

Stock market prediction is a challenging problem because price movements are affected by many external and internal factors, including economic conditions, political events, investor behavior, company performance, and market sentiment.

This research explored an image-based deep learning approach for stock market trend prediction. Instead of using stock prices only as numerical time-series data, historical price movements were transformed into candlestick chart images. These images were then used as input for Convolutional Neural Networks and transfer learning models.

The main idea was to test whether visual patterns in candlestick charts could help deep learning models classify whether a stock price would move upward or downward.

---

## Research Objective

The main objective of this study was to evaluate whether candlestick chart images could be used as a visual representation of stock market behavior for CNN-based prediction.

The study focused on three practical questions:

1. Can historical stock price data be transformed into candlestick chart images for deep learning models?
2. Can CNN-based models detect useful visual patterns in candlestick charts?
3. How do custom CNN models compare with transfer learning models such as VGG16, ResNet50, and InceptionV3?

---

## Dataset

The study used daily stock market data from the Tehran Stock Exchange.

The dataset covered the period from **December 6, 2008 to June 28, 2021**, including **3014 trading days**.

The raw data included daily variables such as:

- opening price;
- closing price;
- last traded price;
- highest price;
- lowest price;
- trading volume;
- number of trades;
- traded value;
- daily price change.

The study first tested the approach on individual stock symbols, then expanded the experiment to a larger dataset across multiple companies listed on the Tehran Stock Exchange.

---

## Methodology

The methodology was based on converting time-series price data into candlestick chart images.

Candlestick charts encode four key pieces of price information:

- opening price;
- closing price;
- highest price;
- lowest price.

The study generated candlestick images using Python and Matplotlib. Different image configurations were tested, including different time windows, image dimensions, and the inclusion or exclusion of volume bars.

The experiments included:

- candlestick charts with 20-day and 60-day windows;
- image sizes such as 50×50, 75×75, and 150×150;
- charts with and without volume bars;
- binary labels representing whether the stock price moved up or down on the following trading day;
- custom CNN models;
- transfer learning models including VGG16, ResNet50, and InceptionV3.

---

## Model Development

The study first tested several CNN architectures on a selected stock symbol to understand whether candlestick image classification was feasible.

After initial experiments, the study expanded to a larger dataset containing candlestick chart images generated from multiple stock symbols.

The final large-scale dataset included more than **590,000 candlestick chart images**. These images were split into training and validation sets and used to compare the performance of different deep learning architectures.

The tested models included:

- a custom CNN architecture;
- VGG16;
- ResNet50;
- InceptionV3.

Transfer learning was used to evaluate whether pre-trained image-classification architectures could improve stock movement prediction from candlestick chart images.

---

## Key Results

The results showed that candlestick chart images could provide some useful predictive signal, but the overall performance remained moderate.

On the larger dataset, the approximate validation accuracies were:

- **Custom CNN:** 61.31%
- **VGG16:** 60.50%
- **InceptionV3:** 59.50%
- **ResNet50:** 51.75%

The custom CNN produced the strongest validation result among the tested models, with VGG16 performing closely behind. ResNet50 performed weakest in this specific experimental setup.

One important finding was that more complex pre-trained models did not necessarily produce better results. In this case, a simpler CNN architecture was competitive with, and slightly better than, several transfer learning approaches.

---

## Interpretation

The results should be interpreted carefully.

The validation accuracy suggests that candlestick chart images may contain visual patterns that are partially useful for stock movement classification. However, the performance is not strong enough to treat the model as a ready-to-use trading system.

This project is better understood as a methodological experiment in financial time-series-to-image conversion and CNN-based classification.

Important considerations include:

- stock markets are noisy and structurally unstable;
- image-based representation alone may not capture enough market context;
- short-term direction prediction is inherently difficult;
- transfer learning from natural image datasets may not fully transfer to financial chart images;
- financial performance would require backtesting, transaction-cost analysis, and risk-adjusted evaluation.

---

## Contribution

The main contribution of this manuscript is the exploration of candlestick chart images as input data for deep learning models in the Tehran Stock Exchange.

The project connected financial time-series analysis with computer vision methods by transforming historical price data into structured image inputs.

It also compared custom CNN modeling with transfer learning approaches, showing that model complexity alone does not guarantee better predictive performance.

---

## Limitations

This work remained at the manuscript stage and has not been formally published.

The main limitations include:

- moderate validation accuracy;
- sensitivity to market volatility;
- limited evidence for real trading profitability;
- no transaction-cost or liquidity analysis;
- limited explainability of CNN-based predictions;
- possible instability across different market regimes;
- high computational cost for large-scale image generation and model training.

The results are useful as a research experiment, but they should not be interpreted as investment advice or a production-ready trading system.

---

## Future Work

Future work could improve the framework by:

- combining candlestick images with numerical technical indicators;
- adding macroeconomic variables such as exchange rates, gold prices, oil prices, or inflation indicators;
- incorporating textual data from news and financial reports;
- testing more advanced hybrid architectures;
- using walk-forward validation;
- evaluating trading profitability after transaction costs;
- applying explainability methods to understand which visual chart patterns influence model decisions;
- testing the approach on other emerging and mature markets.

---

## Keywords

- Tehran Stock Exchange
- Stock Market Prediction
- Candlestick Chart
- Image Classification
- Convolutional Neural Network
- Transfer Learning
- Deep Learning
- Financial Time Series

---

## Authors

Hossein Mostafaei Nia, Omid Mahdi Ebadati Esfahani, and M. Afshar Alam
