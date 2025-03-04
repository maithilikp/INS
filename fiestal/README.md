# 🔐 Feistel Cipher in Python

## 📜 Description
This Python program implements the **Feistel Cipher**, a symmetric encryption technique used as the basis for many modern cryptographic algorithms. It encrypts and decrypts messages using multiple rounds of processing with a key-dependent function.

## ✨ Features
- Implements Feistel cipher encryption and decryption.
- Supports multiple rounds for enhanced security.
- Uses a simple key-dependent function for demonstration purposes.
- Works with both uppercase and lowercase letters.
- Maintains text integrity and structure.

## ⚙️ How It Works
1. The user provides a plaintext message.
2. The user specifies a key and the number of encryption rounds.
3. The program splits the plaintext into two halves.
4. Each round applies a function to one half and swaps the halves.
5. The encrypted text is displayed.
6. The program reverses the process to decrypt the text.

## 🛠 Code Explanation
- 🔐 `encrypt(text, key, rounds)`: Encrypts the given text using the Feistel cipher algorithm.
- 🔓 `decrypt(ciphertext, key, rounds)`: Decrypts the given text using the same process in reverse.
- 🔄 `feistel_function(half, key)`: A simple key-dependent function used in each round.
- 🎯 `main()`: Handles user input, calls encryption and decryption functions, and prints results.

## 💡 Example Run

**Input:**
```bash
Enter the plaintext: HELLO
Enter the key: 1234
Enter the number of rounds: 4
```

**Output:**
```bash
Cipher text is: XGZPQ
Decrypted text is: HELLO
```

## 🖥 Requirements
- 🐍 Python 3.x installed.
- 📝 A text editor or an IDE like PyCharm, VS Code, or Jupyter Notebook.

## 🚀 How to Run
1. Clone this repository or download the script.
2. Open a terminal or command prompt in the script directory.
3. Run the following command:
   ```bash
   python feistel_cipher.py
   ```

## ⚠️ Notes
- The function used in each round can be modified for stronger security.
- The key and round number should be the same for both encryption and decryption.
- The Feistel structure allows the same algorithm to be used for both encryption and decryption.

