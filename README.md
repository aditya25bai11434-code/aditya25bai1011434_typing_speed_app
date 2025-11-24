
# aditya25bai1011434_typing_speed_app
Typing Speed Test (Python)

This is a simple and fun Typing Speed Test built using Python.
It measures how fast you can type a given sentence by calculating:

 Time taken

 Words typed

 Words Per Minute (WPM)

Perfect for beginners learning Python or anyone who wants to test their typing speed.

How It Works

1. The program shows a test sentence:
"the quick brown fox jumps over the lazy dog."


2. You press ENTER when you're ready.


3. As soon as you start typing, the timer begins.


4. After you press ENTER again, the timer stops.


5. The program calculates:

The total time you took

How many words you typed

Your typing speed (WPM)

Features

Easy to run

Beginner-friendly

Clean and simple logic

Works in any Python environment


Requirements

Just Python.
No external libraries needed.

 How to Run

1. Save the code as typing_test.py


2. Run it in your terminal:



python typing_test.py

3. Follow the on-screen instructions and start typing.

Code Used

import time

print("Typing Speed Test\n")

sentence = "the quick brown fox jumps over the lazy dog."
print("Type this sentence:\n")
print(sentence)

input("\nPress ENTER when you are ready...\n")

start = time.time()
typed = input("Start typing:\n")
end = time.time()

time_taken = end - start

# Count words safely
typed_words = len(typed.split())
wpm = typed_words / (time_taken / 60) if time_taken > 0 else 0

print("\nResults:")
print("Time taken:", round(time_taken, 2), "seconds")
print("Words typed:", typed_words)
print("WPM:", round(wpm, 2))

