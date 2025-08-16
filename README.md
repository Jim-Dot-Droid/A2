# Crash Predictor — Under Count Strategy with Martingale 0.01→0.02→stop

This is a Streamlit app that predicts crash outcomes using an **under-count strategy**.  
It tracks history, calculates predictions, and simulates three betting systems:

- **Flat Bet (0.01 SOL)** → Bets 0.01 SOL on every "Above" prediction.
- **Fixed Bet (0.02 SOL)** → Bets 0.02 SOL on every "Above" prediction.
- **Martingale (Custom)** → Sequence: 0.01 → 0.02 → stop until under average ≥ 8.

The app saves balances and results locally, so progress is remembered between runs.

---

## 🚀 Features
- Upload a CSV of multipliers or input manually.
- Predicts based on the number of unders (`< 2.0x`) in the last 20 rounds.
- Three balance trackers (Flat, Fixed, Martingale).
- Martingale logic resets after hitting stop and waiting until **under average ≥ 8**.
- Accuracy tracker showing prediction success rate.

---

## 🛠️ Installation

1. Clone or download this repository.
2. Create a virtual environment (recommended):

   ```bash
   python -m venv venv
   source venv/bin/activate   # On Windows: venv\Scripts\activate

