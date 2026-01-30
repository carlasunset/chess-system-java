# ♟️ Chess System in Java (Console Application)

This project is a **console-based chess system implemented in Java**, designed to model the complete rules and flow of a chess match using **object-oriented principles** and a **layered architecture**.

The focus of this project is not UI, but **domain modeling**, clean design, and correct implementation of game rules.

---

## 🎯 Objectives

- Apply Object-Oriented Programming concepts in a real-world problem
- Model complex game rules in a maintainable and extensible way
- Practice system design, encapsulation, and separation of concerns
- Strengthen Java fundamentals without relying on external frameworks

---

## 🧩 Architecture Overview

The system is organized into clear layers:

### Board Layer
Generic board abstractions, independent of chess rules.
- `Board`
- `Position`
- `Piece`
- `BoardException`

Responsibilities:
- Board boundaries and validation
- Piece placement and removal
- Generic movement structure

---

### Chess Layer
Chess-specific logic and rules.
- `ChessMatch`
- `ChessPiece`
- `ChessPosition`
- `ChessException`
- Piece implementations (`King`, `Queen`, `Rook`, `Bishop`, `Knight`, `Pawn`)
- `Color` enum

Responsibilities:
- Game flow and turn control
- Validation of legal moves
- Check and checkmate detection
- Special moves handling
- Match state consistency

---

### UI Layer
Console-based input/output.
- Responsible only for rendering the board and reading user input
- Does not contain business logic

---

## ♜ Implemented Game Rules

- Standard piece movement validation
- Turn-based gameplay with current player control
- Piece capture tracking
- Check and checkmate detection
- Prevention of illegal moves that expose the king
- Special chess rules:
    - Castling
    - En passant
    - Promotion
- Move count tracking
- Undo move logic for validation purposes

---

## 🛠️ Key Technical Concepts Used

- Encapsulation with strict access control
- Inheritance and polymorphism for piece behavior
- Abstract methods (`possibleMoves`) to enforce contracts
- Custom domain-specific exceptions
- Defensive programming
- Matrix-based board representation
- Lists for captured and active pieces
- Method overriding and overloading
- Enum-based state control

---

## ▶️ Running the Application

1. Clone the repository
2. Compile the project using Java
3. Run the main `Program` class
4. Interact with the game via the terminal

---

## 📌 Notes

This project was developed as a practical exercise to **consolidate Object-Oriented Programming concepts in Java** through a non-trivial domain problem.

By implementing the complete logic of a chess match, the project reinforces core OOP principles such as **encapsulation, inheritance, polymorphism, and abstraction**, while also encouraging clean architecture, responsibility separation, and defensive programming.

The system was intentionally designed without external frameworks to strengthen understanding of **Java fundamentals, domain modeling, and system design**, serving as a solid foundation for more complex backend applications.
