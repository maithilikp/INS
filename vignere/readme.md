# Vigenère Cipher Implementation in Python

## Overview
This project implements the Vigenère Cipher, a classical encryption technique, in Python. The Vigenère Cipher is a method of encrypting alphabetic text using a simple form of polyalphabetic substitution.

## Features
- Encrypt plaintext using the Vigenère Cipher.
- Decrypt ciphertext back to plaintext.
- Support for custom keys.
- Handles both uppercase and lowercase letters while ignoring non-alphabetic characters.

## Prerequisites
Ensure you have Python installed on your system.

## Usage

### 1. Clone the Repository
```sh
git clone https://github.com/yourusername/vigenere-cipher.git
cd vigenere-cipher
```

### 2. Run the Script
To encrypt a message:
```sh
python vigenere.py encrypt "HELLO WORLD" "KEY"
```
To decrypt a message:
```sh
python vigenere.py decrypt "RIJVS UYVJN" "KEY"
```

## Code Example
```python
def vigenere_encrypt(plaintext, key):
    encrypted_text = ""
    key = key.upper()
    key_index = 0
    
    for char in plaintext:
        if char.isalpha():
            shift = ord(key[key_index]) - ord('A')
            if char.isupper():
                encrypted_text += chr((ord(char) - ord('A') + shift) % 26 + ord('A'))
            else:
                encrypted_text += chr((ord(char) - ord('a') + shift) % 26 + ord('a'))
            key_index = (key_index + 1) % len(key)
        else:
            encrypted_text += char
    
    return encrypted_text
```

## Example
**Encryption:**
```sh
Input: "HELLO WORLD", Key: "KEY"
Output: "RIJVS UYVJN"
```

**Decryption:**
```sh
Input: "RIJVS UYVJN", Key: "KEY"
Output: "HELLO WORLD"
```

## License
This project is licensed under the MIT License.

## Author
MAAITHILI KP

