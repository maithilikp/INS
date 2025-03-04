# Monoalphabetic Cipher in Python

## Overview
The Monoalphabetic Cipher is a type of substitution cipher where each letter in the plaintext is replaced with a corresponding letter in the ciphertext based on a fixed key mapping. This implementation in Python provides functionalities for encryption and decryption.

## Features
- Encrypts plaintext using a fixed substitution key
- Decrypts ciphertext back to plaintext
- Supports user-defined key mappings
- Handles case sensitivity and spaces

## Installation
Ensure you have Python installed on your system. Clone this repository and navigate to the project directory:
```sh
$ git clone <repository-url>
$ cd monoalphabetic-cipher
```

## Usage
Run the script and provide the plaintext message and key mapping:
```sh
$ python monoalphabetic_cipher.py
```

### Example
```python
from monoalphabetic_cipher import MonoalphabeticCipher

key_mapping = {
    'a': 'm', 'b': 'n', 'c': 'b', 'd': 'v', 'e': 'c', 'f': 'x', 'g': 'z', 'h': 'a', 'i': 's', 'j': 'd',
    'k': 'f', 'l': 'g', 'm': 'h', 'n': 'j', 'o': 'k', 'p': 'l', 'q': 'p', 'r': 'o', 's': 'i', 't': 'u',
    'u': 'y', 'v': 't', 'w': 'r', 'x': 'e', 'y': 'w', 'z': 'q'
}

cipher = MonoalphabeticCipher(key_mapping)
plaintext = "hello world"
ciphertext = cipher.encrypt(plaintext)
print("Ciphertext:", ciphertext)

decrypted_text = cipher.decrypt(ciphertext)
print("Decrypted Text:", decrypted_text)
```

## Functions
- `encrypt(plaintext: str) -> str`: Encrypts the given plaintext using the key mapping.
- `decrypt(ciphertext: str) -> str`: Decrypts the given ciphertext back to plaintext.

## License
This project is licensed under the MIT License.

## Contributing
Feel free to fork the repository and submit pull requests for improvements or bug fixes.

## Author
maithili KP
