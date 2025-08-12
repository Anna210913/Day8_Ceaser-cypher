# Day 8: Caesar Cipher Project

On Day 8, we built a Python program that can **encode** (encrypt) and **decode** (decrypt) messages using the Caesar cipher.

## What is a Caesar Cipher?

A **Caesar cipher** is one of the simplest and most well-known encryption techniques. It’s a type of substitution cipher where each letter in the plaintext is shifted a certain number of places down or up the alphabet.

As explained by Dr. Angela Yu, imagine the alphabet as a circle. When you shift letters, you move forward or backward around this circle by a fixed number (called the “shift” or “key”). For example, with a shift of 3, `a` becomes `d`, `b` becomes `e`, and so on. When you reach the end of the alphabet, it wraps around to the beginning.

This method is used to encode messages to keep them secret, and decoding just reverses the process by shifting letters back.

## What We Learned and How the Code Works

- We created a list of the alphabet letters to easily find and shift letters.
- We wrote a function `caesar()` that:
  - Takes the input text, shift amount, and direction (`encode` or `decode`).
  - Adjusts the shift direction by multiplying by -1 if decoding.
  - Iterates through each letter of the input:
    - If the letter is not in the alphabet (like spaces, punctuation), it stays unchanged.
    - Otherwise, it finds the letter’s index, shifts it by the shift amount, and uses modulo `%` to wrap around the alphabet.
  - Builds the resulting encoded or decoded string and prints it.
- We used a `while` loop to allow the user to encode or decode multiple messages until they choose to quit.
- User inputs determine the action (`encode` or `decode`), the message, and the shift number.

## This project helped us practice:

- List indexing and modulo arithmetic for wrapping around the alphabet.
- String manipulation and iteration.
- Defining and using functions with parameters.
- Basic input/output and program flow control.

## How to Use the Program

1. Run the program.
2. When prompted, type `encode` to encrypt or `decode` to decrypt a message.
3. Enter your message (letters, spaces, and symbols are allowed).
4. Enter the shift number (how many letters to shift).
5. View the encoded or decoded result.
6. Choose to continue or exit.
