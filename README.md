# Hangman Game

Welcome to the Hangman Game Code! This Python script allows you to play the classic word-guessing game, Hangman, in your console. Below, you'll find an explanation of the code and how to use it.

## Table of Contents

- [Introduction](#introduction)
- [Code Explanation](#code-explanation)
- [How to Use](#how-to-use)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Hangman is a popular word puzzle game where the player tries to guess a hidden word one letter at a time. This code implements the game's core logic and provides a fun and interactive way to play Hangman in your terminal.

## Code Explanation

The code is organized as follows:

1. It imports the `word_list` (a list of words to guess), `stages` (a list of hangman drawing stages), and `logo` from external modules.

2. The script randomly selects a word from the `word_list` and calculates its length.

3. It initializes variables for the game, including `end_of_game` (a flag to check if the game has ended) and `lives` (the number of attempts the player has).

4. The Hangman logo is displayed using the `logo` variable.

5. A list called `display` is created to represent the word to be guessed. It initially contains underscores, one for each letter in the chosen word.

6. The game loop (`while not end_of_game`) handles the game's logic:

   - It displays the current state of the word with underscores and correctly guessed letters.
   
   - The player is prompted to guess a letter (case-insensitive).
   
   - The code checks if the guessed letter has already been entered and provides feedback to the player if necessary.

   - It iterates through the chosen word, checking if the guessed letter matches any of its characters. If so, the correct letter is revealed in the `display` list.

   - If the guessed letter is not in the chosen word, the player loses a life. If lives reach zero, the game ends, and the player loses, with the chosen word revealed.

   - It checks if the player has successfully guessed all letters, indicating a win.

   - The current hangman drawing stage is displayed based on the number of remaining lives using the `stages` list.

## How to Use

To use this code, follow these steps:

1. Ensure you have Python 3.x installed on your computer.

2. Create a Python script (e.g., `hangman.py`) and paste the code into it.

3. Download the `hangman_words.py` and `hangman_art.py` files, which contain the required word list and hangman graphics.

4. Run the script using your Python interpreter:

## Contributing

If you would like to contribute to this project, feel free to open issues or submit pull requests. Any enhancements or improvements to the game are welcome!

## License

This code is licensed under the MIT License. You can find the full license details in the [LICENSE](LICENSE) file.

---

Enjoy playing Hangman with this code! If you have any questions or encounter issues, please don't hesitate to get in touch. Have fun guessing words!


   ```bash
   python hangman.py
