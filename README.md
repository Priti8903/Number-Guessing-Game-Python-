# 🎮 Number Guessing Game (Python)

This is a simple **number guessing game** built in Python. The computer randomly selects a number between 1 and 1000, and the user tries to guess it. The game provides feedback if the guess is too high or too low and counts the number of attempts.

## 📋 Features

- Random number generation between 1 and 1000
- User input with guidance
- Tracks number of attempts
- Feedback on each guess

## 🧠 How It Works

1. The program selects a random number between 1 and 1000.
2. You enter a guess.
3. The program tells you if the guess is too high, too low, or correct.
4. It repeats until you guess the correct number.
5. Displays the total number of attempts.

## Code
```
import random

def guess_the_number():
    number = random.randint(1, 1000)
    attempt = 0
    print("Welcome to the Number Guessing Game!")

    while True:
        try:
            guess = int(input("Guess a number between 1 to 1000: "))
            attempt += 1
            if guess == number:
                print(f"🎉 Congratulations! You guessed the number {number} in {attempt} attempts.")
                break
            elif guess < number:
                print("📉 Too low! Try again.")
            else:
                print("📈 Too high! Try again.")
        except ValueError:
            print("⚠️ Invalid input. Please enter a valid number.")

guess_the_number()

```
## 🛠️ How to Run

```
number_guessing_game.py
```


## 💡 Example Output

```
Welcome to the Number Guessing Game!
Guess a number between 1 to 1000: 500
📉 Too low! Try again.
Guess a number between 1 to 1000: 750
📈 Too high! Try again.
Guess a number between 1 to 1000: 723
🎉 Congratulations! You guessed the number 723 in 8 attempts.
Guess a number between 1 to 1000: Priti
⚠️ Invalid input. Please enter a valid number.

```


### Prerequisites

Make sure Python is installed on your machine.

```bash
python --version
```

## 
📁 File Structure
```
.
├── guess_the_number.py
└── README.md
```

