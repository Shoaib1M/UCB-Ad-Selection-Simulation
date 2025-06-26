# 📊 UCB Ad Selection Simulation

This project demonstrates the use of the **Upper Confidence Bound (UCB)** algorithm for selecting the most rewarding advertisement out of a set of 10 possible ads based on user clicks. It simulates ad selection over 10,000 rounds using a dataset of simulated user responses.

## 🧠 Concept

The **UCB algorithm** is a Reinforcement Learning method that solves the **Multi-Armed Bandit problem** — choosing the best option (ad) over time based on limited information.

In each round:
- It selects the ad with the highest upper confidence bound.
- Tracks selections and rewards to balance **exploration vs. exploitation**.

## 📁 Dataset

File: `Ads_CTR_Optimisation.csv`  
- 10,000 rows × 10 columns  
- Each row represents a single user click session.
- A `1` indicates the ad was clicked; `0` means no click.

## 📈 Output

At the end of 10,000 rounds, a histogram is shown indicating how many times each ad was selected.

![Histogram Example](f4b4497a-90fd-4883-b54e-92de8459c290.png)

## 📦 Requirements

- Python 3.x
- pandas
- matplotlib
- numpy

Install with:

```bash
pip install -r requirements.txt
