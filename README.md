# Guess-game

# 🎲 Number Guessing Game

A terminal-based number guessing game written in C++. The computer picks a random number, you guess it with **higher/lower** hints, and your best score is saved between sessions.

Built as a beginner-friendly project for [Hack Club](https://hackclub.com) — small enough to read in one sitting, but real enough to ship. 🚀

---

## ✨ Features

- 🎯 Random number between 1 and 100
- ⬆️⬇️ "Higher" / "Lower" hints after every guess
- 🏆 Persistent high score saved to `highscores.txt`
- ✅ Input validation (no crashes on typos)
- 🔁 Play-again loop
- 📦 No dependencies — just the C++ standard library

---

## 🧠 Concepts Practiced

| Concept | Where It Lives |
|---|---|
| Conditionals (`if`/`else`) | Hint logic in `main()` |
| Random numbers (`rand()`) | `std::rand() % (upper - lower + 1) + lower` |
| File I/O (`fstream`) | `readHighScore()` / `saveHighScore()` |
| Loops & input validation | `getValidInt()` + replay loop |

---

## 🚀 Getting Started

### Prerequisites

You just need a C++ compiler:

- **Linux / macOS:** `g++` (comes with GCC or Clang)
- **Windows:** [MinGW-w64](https://www.mingw-w64.org/) or use WSL

### Build & Run

```bash
g++ -std=c++17 -O2 main.cpp -o guessing_game
./guessing_game
