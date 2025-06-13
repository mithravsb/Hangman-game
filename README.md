import randam
word_list = ["python", "hangman", "challenge", "programming", "developer", "artificial", "intelligence"]


word = random.choice(word_list)
word_letters = set(word)
guessed_letters = set()
lives = 6

print("Welcome to Hangman!")

while len(word_letters) > 0 and lives > 0:
    print(f"\nYou have {lives} lives left.")
    print("Guessed letters: ", " ".join(sorted(guessed_letters)))
    
    
    word_display = [letter if letter in guessed_letters else '_' for letter in word]
    print("Word: ", " ".join(word_display))

    guess = input("Guess a letter: ").lower()

    if guess in guessed_letters:
        print("You already guessed that letter.")
    elif guess in word_letters:
        guessed_letters.add(guess)
        word_letters.remove(guess)
        print("Good guess!")
    else:
        guessed_letters.add(guess)
        lives -= 1
        print("Wrong guess.")

if lives == 0:
    print(f"\nGame Over! The word was '{word}'.")
else:
    print(f"\nCongratulations! You guessed the word '{word}' correctly.")
