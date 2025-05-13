# Generative Modeling of Limit Order Book (LOB) Data

This project simulates realistic order flow using generative models trained on LOBSTER market data. It captures key properties of order book dynamics, including mid-price evolution, order arrivals, sizes, directions, and limit order prices.

## Project Overview

The goal is to simulate a full trading day of synthetic market activity that statistically resembles real LOBSTER data. This is useful for:

- Testing trading strategies
- Modeling rare market events
- Analyzing liquidity and order book dynamics

## Features Modeled

- **Order Arrival** (Market & Limit) using logistic regression and Bernoulli sampling
- **Order Side** (Buy/Sell) based on time-dependent probabilities
- **Order Size** using power-law distributions fitted to real LOBSTER data
- **Limit Order Price** using lognormal offsets from mid-price
- **Mid-Price Path** simulated with a lognormal random walk (Geometric Brownian Motion)

## Files

- `generative_model.ipynb`: Main notebook containing full simulation pipeline
- `synthetic_orders.csv`: Output of synthetic orders in LOBSTER format
- `requirements.txt`: Dependencies to run the notebook
- 'lob_engine_group3.py': Limit Order Book engine from group 3
- `README.md`: Project description and instructions
- 'AAPL_2012-06-21_message_10.csv': Message data



