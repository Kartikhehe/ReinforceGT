```markdown
# Game Theory: Nash Equilibrium Detection and Best Response Analysis

This repository contains two Python-based assignments demonstrating core concepts in Game Theory:

1. **Nash Equilibrium Identification in a 2-Player Game**
2. **Best Action (Best Response) Computation Based on Payoff Matrix**

---

## 📌 Assignment 1: Nash Equilibrium Detection

### Description
This script checks for pure strategy Nash Equilibria in a classic two-player payoff matrix game (Prisoner's Dilemma).

### Payoff Matrix
```python
payoff = {
    "C": {
        "C": (3, 3),
        "D": (0, 5)
    },
    "D": {
        "C": (5, 0),
        "D": (1, 1)
    }
}
```

### Logic
The function `isNash(p1, p2)` checks whether the strategy pair `(p1, p2)` is a Nash Equilibrium by ensuring no player can unilaterally deviate to improve their payoff.

### Output
```
Nash Equilibria attained for: [('D', 'D')]
```

---

## 📌 Assignment 2: Best Response Strategy Computation

### Description
This script determines the best response (action) for a player given the opponent's action, based on a 2x2 payoff matrix.

### Payoff Matrix (Battle of the Sexes variant)
```python
payoff = {
    "C": {
        "C": (2, 1),
        "D": (0, 5)
    },
    "D": {
        "C": (0, 0),
        "D": (1, 2)
    }
}
```

### Function
- `best_action(payoff_matrix, player, opponent_action)`:
    - Returns the best action for player 1 or 2 depending on what the opponent played.

### Action Encoding
```python
action_encoding = {
    'Bash': 'C',
    'Stravinsky': 'D',
    'C': 'Bash',
    'D': 'Stravinsky'
}
```

### Output
```
Best action for player 1 against opponent's action 'C': Bash
```

---

## ✅ Requirements
- Python 3.x
- No external dependencies

---

## 📂 Files
- `nash_equilibrium.py` – Code to find all Nash Equilibria
- `best_response.py` – Code to compute best responses given opponent's move

---

## 👨‍💻 Author
This project is a part of a Game Theory assignment exploring strategy optimization in 2x2 games.

---

## 📚 References
- Game Theory (Nash Equilibrium, Best Response)
- Classic examples: Prisoner's Dilemma, Battle of the Sexes
```
