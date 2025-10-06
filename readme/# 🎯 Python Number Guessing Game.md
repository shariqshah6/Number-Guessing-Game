# 🎯 Python Number Guessing Game

A fun and simple **Number Guessing Game** built using Python!  
The computer randomly selects a number, and the player has to **guess it**.  
After each guess, the program tells you whether your guess was **too high**, **too low**, or **correct**.  

---

## 🚀 Features
- 🔢 Random number generation between 1 and 20  
- 💬 Helpful hints: “Too High” or “Too Low”  
- 🧠 Tracks number of attempts  
- 🕹️ Simple console-based interface  

---

## 🧰 Technologies Used
- **Python 3**
- **`random` module**

---

## 🧑‍💻 How It Works
1. The program randomly picks a number between **1 and 20**.  
2. You keep guessing until you find the correct number.  
3. After each wrong guess, it tells you if your number is **too high** or **too low**.  
4. When you guess correctly, it shows how many attempts you took.  

---

## 🧩 Code Example
```python
import random

number = random.randint(1, 20)
attempts = 0

while True:
    guess = int(input("Guess a number (1-20): "))
    attempts += 1

    if guess == number:
        print(f"🎉 Correct! You guessed it in {attempts} tries.")
        break
    elif guess < number:
        print("Too low!")
    else:
        print("Too high!")
