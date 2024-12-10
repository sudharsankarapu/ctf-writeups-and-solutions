# Cryptography Challenge: Caesar Cipher

## Challenge Description
The encrypted message was: "Khoor Zruog". The objective was to decrypt it without knowing the key.

---

## Steps to Solve
1. **Understand the Cipher:**  
   - The Caesar Cipher shifts each letter by a fixed number of positions in the alphabet.

2. **Decrypt the Message:**  
   - Wrote a Python script to brute force all possible shifts:
     ```python
     message = "Khoor Zruog"
     for shift in range(1, 26):
         decrypted = ''.join(
             chr((ord(char) - shift - 65) % 26 + 65) if char.isupper() else
             chr((ord(char) - shift - 97) % 26 + 97) if char.islower() else char
             for char in message
         )
         print(f"Shift {shift}: {decrypted}")
     ```
   - Found the correct shift (3): "Hello World".

---

## Lessons Learned
- Simple ciphers can often be brute-forced easily.
- Understanding cryptographic algorithms helps in both attacking and securing systems.
