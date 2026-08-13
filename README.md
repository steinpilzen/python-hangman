# 🎮 Hangman Game

A classic Hangman game built in Python, with a modern twist using the [Rich](https://github.com/Textualize/rich) library for colorful terminal panels, plus a smart hint system and input validation.

## Features

- 🎲 **Random word selection** from a built-in word list
- 🖼️ **Rich-styled panels** for a polished welcome and end screen
- ✅ **Input validation** — rejects empty input, numbers, symbols, and multi-character entries
- 💡 **Smart hint system** — reveals a random hidden letter at the cost of one life
- 🔁 **Duplicate guess detection** — won't let you waste a turn on a letter you already tried
- 🖌️ **ASCII hangman art** that updates with every wrong guess

## Demo

```
==============================================
The hidden word is: _ _ _ _ _ _
Incorrect letters: []
Pick a letter (or type 'HINT' for a clue):
```

## Requirements

- Python 3.7+
- [rich](https://pypi.org/project/rich/)

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/steinpilzen/python-hangman.git
   cd python-hangman
   ```

2. Install the required dependency:
   ```bash
   pip install rich
   ```

## How to Play

Run the game from your terminal:

```bash
python hangman_game.py
```

- Type a single letter and press Enter to guess it.
- Type `HINT` to reveal a random letter (costs you one life).
- You have 6 mistakes before the game ends.
- Guess all the letters before you run out of lives to win!

## How It Works

The game picks a random word from a predefined list and represents it as underscores. Each guess is checked against the word:

- **Correct guesses** reveal the letter(s) in the hidden word.
- **Incorrect guesses** reduce your remaining mistakes and draw the next stage of the hangman.
- **Hints** reveal a random unguessed letter but cost a life, just like a wrong guess.

## Project Structure

```
python-hangman/
├── hangman_game.py     # Main game script
└── README.md      # This file
```

## Possible Future Improvements

- Add difficulty levels (short vs. long words)
- Load word list from an external file or API
- Track wins/losses across sessions
- Add a GUI version

## Author

Made by [steinpilzen](https://github.com/steinpilzen)
