# 🔐 Hill Cipher in Python

## 📜 Description
This Python program implements the **Hill Cipher**, a polygraphic substitution cipher based on linear algebra. It encrypts and decrypts messages using matrix multiplication with a key matrix.

## ✨ Features
- Encrypts plaintext using the Hill cipher technique.
- Decrypts ciphered text back to its original form.
- Supports user-defined key matrices.
- Works with uppercase letters (A-Z) and ignores non-alphabetic characters.
- Uses modular arithmetic for encryption and decryption.

## ⚙️ How It Works
1. The user provides a plaintext message.
2. The user specifies a key matrix (must be invertible in modulo 26).
3. The program encrypts the plaintext using matrix multiplication and modular arithmetic.
4. The encrypted text is displayed.
5. The program decrypts the encrypted text using the inverse key matrix.
6. The decrypted text (original message) is displayed.

## 🛠 Code Explanation
- 🔐 `encrypt(plaintext, key_matrix)`: Encrypts the given text using the Hill cipher algorithm.
- 🔓 `decrypt(ciphertext, key_matrix)`: Decrypts the given text using the inverse of the key matrix.
- 📏 `mod_inverse(matrix, mod)`: Computes the modular inverse of the key matrix.
- 🎯 `main()`: Handles user input, calls the encryption and decryption functions, and prints results.

## 💡 Example Run

**Input:**
```bash
Enter the plaintext: HELLO
Enter the 2x2 key matrix: [[3, 3], [2, 5]]
```

**Output:**
```bash
Cipher text is: ZEBBW
Decrypted text is: HELLO
```

## 🖥 Requirements
- 🐍 Python 3.x installed.
- 📚 NumPy library installed (`pip install numpy`).
- 📝 A text editor or an IDE like PyCharm, VS Code, or Jupyter Notebook.

## 🚀 How to Run
1. Clone this repository or download the script.
2. Open a terminal or command prompt in the script directory.
3. Run the following command:
   ```bash
   python hill_cipher.py
   ```

## ⚠️ Notes
- The key matrix must be square and invertible modulo 26.
- The plaintext length should be a multiple of the matrix size (padding may be required).
- The decryption process requires computing the modular inverse of the key matrix.

