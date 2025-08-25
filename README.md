# Wumpus World with Minimax Algorithm

This project implements the **Minimax algorithm** applied to the classic **Wumpus World** problem, demonstrating decision-making under uncertainty in an adversarial environment.

---

## Overview

The environment consists of a grid-based world populated by an agent, dangerous obstacles, hinst, and a coin. The agent must safely navigate the world to retrieve the coin while avoiding obstacles. The decision-making process leverages the **Minimax algorithm**, ensuring that the agent follows a strategy that minimizes risk while maximizing rewards.

Key highlights:
- **Sprites directory**: Contains all visual assets used to represent the board. These were created in *Photoshop CS6*.
- **Execution environment**: The code was developed and tested on *Jupyter Notebook v6.4.8*. In newer versions, sprites may not render correctly. However, each image includes an `alt` attribute with the sprite name, ensuring that the board representation remains understandable.

---

## Algorithm Behavior

- **Successor evaluation**: Each move is evaluated using Minimax, and only the selected state is represented. The output also displays the resulting state after the agent’s real move and the subsequent random move of the pits.
- **Risk balance**: The evaluation parameters are calibrated so that the agent searches for the coin in an extremely safe manner. This leads to potentially long executions, but the probability of defeat remains very low.
- **Agent constraints**: Although the current cell is displayed in the evaluation output, it is not included in the Minimax decision process. The agent is assumed to move every turn and cannot remain idle. An alternative implementation (commented in the code) explores including the current cell as a valid option.
- **Rule enforcement**: Distance rules are strictly prioritized. If a rule cannot be respected, the corresponding entity (e.g., a pit) is omitted. This may result in a board without one of the pits. In such cases, it is recommended to reset the board.

---

## How to Run

1. Clone the repository.
2. Open the Jupyter Notebook in version **6.4.8** (recommended).
3. Run all cells sequentially to observe:
   - Board initialization with sprites.
   - Successor state evaluations.
   - Agent and pit movements.

---

## Notes

- The Minimax implementation focuses on **safety over speed**, which may result in longer simulations but ensures a robust strategy.
- The project is designed for educational and research purposes, showcasing how adversarial search algorithms can be applied to grid-based decision-making problems.

---
