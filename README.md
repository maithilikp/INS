# 🔐 Caesar Cipher in Python

## 📜 Description
This Python program implements the **Caesar Cipher** encryption and decryption techniques. Users can enter a plaintext message and a shift value, which determines how many positions each letter in the text will be shifted in the alphabet.

## ✨ Features
- Encrypts a given text using the Caesar cipher technique.
- Decrypts the ciphered text back to its original form.
- Works for both uppercase and lowercase letters.
- Maintains spaces and non-alphabetic characters.

## ⚙️ How It Works
1. The user provides a plaintext message.
2. The user specifies a shift value (key) for encryption.
3. The program encrypts the plaintext using the Caesar cipher.
4. The encrypted text is displayed.
5. The program decrypts the encrypted text using the same shift value.
6. The decrypted text (original message) is displayed.

## 🛠 Code Explanation
- 🔐 `encrypt(text, shift)`: Encrypts the given text by shifting characters forward in the alphabet.
- 🔓 `decrypt(text, shift)`: Decrypts the given text by shifting characters backward in the alphabet.
- 🎯 `main()`: Handles user input, calls the encryption and decryption functions, and prints results.

## 💡 Example Run

**Input:**
```bash
Enter the plaintext: hello world
Enter the shift value: 3
```

**Output:**
```bash
Cipher text is: khoor zruog
Decrypted text is: hello world
```

## 🖥 Requirements
- 🐍 Python 3.x installed.
- 📝 A text editor or an IDE like PyCharm, VS Code, or Jupyter Notebook.

## 🚀 How to Run
1. Clone this repository or download the script.
2. Open a terminal or command prompt in the script directory.
3. Run the following command:
   ```bash
   python caesar_cipher.py
   ```

## ⚠️ Notes
- The program only shifts alphabetical characters; spaces and punctuation remain unchanged.
- The shift value should be a positive integer.
- The decryption process reverses the shift to retrieve the original message.

