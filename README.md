# Java Swing Tic-Tac-Toe

## Project Overview

A lightweight, two-player Tic-Tac-Toe game developed in Java, demonstrating core Java Swing GUI principles. This project implements fundamental game logic, state management, and event handling within a clean, single-class architecture.

---

## Core Functionality

- **Swing-based GUI**: A 3x3 grid using `JButton` components for user interaction.
- **Dynamic Status Label**: A `JLabel` provides real-time feedback, indicating the current player's turn ("X" or "O").
- **Win/Draw Detection**: Implements algorithmic logic to check for all 8 winning conditions (rows, columns, and diagonals) and detects stalemate (draw) situations.
- **Game State Management**: Automatically handles game resets upon completion (win or draw) to allow for continuous play.
- **Clean UI Layout**: Utilizes `BorderLayout` and `GridLayout` with appropriate margins for a polished user experience.

---

## Build & Run

### Prerequisites

- Java Development Kit (JDK) 8 or higher.

### Compilation & Execution

1.  Clone or download the repository.
2.  Save the source code as `TicTacToeGame.java`.
3.  Compile the source file from your terminal:
    ```bash
    javac TicTacToeGame.java
    ```
4.  Run the compiled Java class:
    ```bash
    java TicTacToeGame
    ```
5.  The application window will launch, ready for play.

---

## Architectural Overview

- **Main Class (`TicTacToeGame`)**: A single-class implementation encapsulating all game logic and GUI rendering. It initializes the `JFrame`, `JLabel` (status), and the `JButton[3][3]` array (game board).
- **Event Handling**: Utilizes a nested `ButtonClickListener` class (implementing `ActionListener`) to manage user input, update the game state, modify button text, and trigger win-checking logic.

---

## Screenshot

![Tic-Tac-Toe GUI](https://github.com/user-attachments/assets/2c952870-1e2a-4558-9901-d37b3e893866)

---

## Potential Roadmap

- **Persistent Scoreboard**: Implement score tracking across multiple game sessions.
- **AI Opponent**: Integrate an AI player, potentially using a Minimax algorithm.
- **Scalable Grid**: Refactor the logic to support a user-defined N x N grid.
