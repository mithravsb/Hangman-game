🪢 Hangman Game (Python)

Welcome to the Hangman Game written in Python! This is a fun, interactive terminal-based game where you try to guess a secret word one letter at a time before your chances run out.


🧠 How It Works

The program randomly selects a word from a predefined list.

You guess one letter at a time.

The game displays:

Correctly guessed letters in their positions.

Underscores for unknown letters.


If the guessed letter is not in the word, you lose one life.

The game continues until:

You guess the full word correctly (you win 🎉).

You run out of lives (you lose 💀).

🛠️ Requirements

Python 3.x



▶️ How to Run

1. Clone the repository or download the Python file:

git clone <repository-link>


2. Navigate to the project folder:

cd hangman-game


3. Run the Python file:

python hangman.progam
Output Example

Welcome to Hangman!
_ _ _ _ _ _

Guess a letter: e
Good guess: _ _ e _ _ _

Guess a letter: a
Sorry, 'a' is not in the word.
Lives remaining: 5

Guess a letter: s
Good guess: s _ e _ _ _

Guess a letter: c
Good guess: s c e _ _ _

Guess a letter: n
Good guess: s c e n _ _

Guess a letter: t
Good guess: s c e n t _

Guess a letter: s
You've already guessed that letter.

Guess a letter: r
Good guess: s c e n t r

Congratulations! You guessed the word: 'scentr'
You won in 7 guess
