# Playfair Cipher in Python

## Overview
This repository contains an implementation of the Playfair Cipher written in Python. The Playfair Cipher is a digraph substitution cipher that encrypts pairs of letters using a 5x5 matrix generated from a keyword.

## Features
- Encrypts plaintext messages using the Playfair Cipher technique
- Decrypts ciphertext back to plaintext
- Handles letter pairs and replaces 'J' with 'I' (as per standard Playfair rules)
- Removes duplicate letters in the key to form a proper 5x5 matrix

## Usage
### Requirements
- Python 3.x

### Running the Code
1. Clone this repository:
   ```bash
   git clone <repository_url>
   ```
2. Navigate to the project directory:
   ```bash
   cd playfair-cipher
   ```
3. Run the script:
   ```bash
   python playfair.py
   ```

### Example
#### Encryption
```python
Enter the key: SECRET
Enter the plaintext: HELLO
Ciphertext: KCJMLQ
```

#### Decryption
```python
Enter the key: SECRET
Enter the ciphertext: KCJMLQ
Plaintext: HELXLO
```
(Note: The 'X' is often used as a filler character when handling repeated letters or odd-length plaintexts.)

## How It Works
1. The key is used to generate a 5x5 matrix (removing duplicates and merging 'I' and 'J').
2. The plaintext is divided into letter pairs, inserting 'X' if needed.
3. Each pair is encrypted based on matrix rules:
   - Same row: Replace each letter with the letter to its right.
   - Same column: Replace each letter with the letter below it.
   - Otherwise, form a rectangle and swap letters.
4. Decryption follows the reverse process.

## License
This project is open-source under the MIT License.

## Author
Maithili KP
