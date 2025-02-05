
import unittest
import random

def add(a, b):
    return a + b

def subtract(a, b):
    return a - b

def multiply(a, b):
    return a * b

def divide(a, b):
    if b == 0:
        raise ValueError("Cannot divide by zero")
    return a / b

def is_prime(n):
    if n < 2:
        return False
    for i in range(2, int(n ** 0.5) + 1):
        if n % i == 0:
            return False
    return True

# AI-Based-Music-Generator
An AI-powered tool that generates music tracks based on user preferences.

📜 Features:

 • AI-powered melody generation
 • Exports as MP3/WAV
 • Adjustable tempo and style

📂 File Structure:

/ai-music-generator
 ├── models/        # AI models for music generation  
 ├── samples/       # Generated music samples  
 ├── generator.py   # Main script  
 ├── README.md      # Documentation  
 ├── config.json    # Settings  

🚀 How to Run:

pip install -r requirements.txt
python generator.py
