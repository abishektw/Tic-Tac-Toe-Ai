# Tic-Tac-Toe AI

This project implements a **Tic-Tac-Toe game** in Python with three different AI opponents and a comparative analysis module.  
The goal is to compare the performance of different AI strategies using both **game outcomes** and **decision-quality metrics**.

---

## ✅ Features

### 🎯 Play Mode (Human vs AI)
You can play Tic-Tac-Toe against:
1. **Minimax AI** (optimal strategy)
2. **Depth-Limited Minimax + Heuristic AI** (faster search)
3. **Rule-Based AI** (simple win/block rules)

### 📊 Comparative Analysis Mode (AI vs AI)
Runs automated experiments and generates:
- Win / Draw / Loss counts
- NoLoss%
- Average decision time per move
- Move accuracy (outcome-based)
- Regret (opportunity loss)

Includes:
- Summary table in terminal
- Matplotlib graphs

---

## 🧠 Algorithms Implemented

### 1) Minimax (Full Search)
- Searches all possible future states until game ends
- Always chooses optimal move
- **Never loses** in Tic-Tac-Toe
- Slower due to full search

### 2) Depth-Limited Minimax + Heuristic
- Searches only up to a fixed depth (default depth = 2)
- Uses heuristic evaluation at cutoff depth
- Very fast and performs near optimally

### 3) Rule-Based AI
Simple logic:
1. Win if possible
2. Block opponent win
3. Else random move  

Fastest algorithm but weakest because it cannot predict forks or long-term tactics.

---

## 📌 Metrics Used (Comparative Analysis)

- **W/D/L**: Wins / Draws / Losses
- **NoLoss%** = (Wins + Draws) / Total games × 100
- **Average decision time (ms/move)** using `time.time()`
- **Move Accuracy (%)** (optimal-outcome based)
- **Regret**
  - Regret = Best possible score − Chosen move score
  - Lower regret means better decision quality

---

## 🛠 Requirements
- Python 3.x  
- matplotlib  

---

## ▶️ Install & Run

Run the following commands:


Run If matplotlib is not installed:

```bash
pip install matplotlib
```
To run:

```bash
python ai.py
```

---

You will see a menu:

-Play vs Minimax

-Play vs Depth-Limited Minimax (Heuristic)

-Play vs Rule-Based AI

-Run Comparative Analysis (table + graphs)

---

## 📊 Comparative Analysis Output

When selecting Run Comparative Analysis, the program will:

-run AI vs AI matchups (alternating who starts first for fairness)

-print performance results in a table

-display graphs such as:

-Win/Draw/Loss comparison

-Average decision time

-Move accuracy

-Average regret

---

## 👤 Author

Name: Abishek Tiwari

Student ID: 23048472

Module: Artificial Intelligence
