# 🔐 Caesar Cipher in C

This program implements the **Caesar Cipher**, a simple encryption technique where each letter in the plaintext is shifted by a fixed number of places in the alphabet.

---

## 🚀 Programming Language
This program is written in **C**, making it efficient for handling string manipulations.

---

## 🛠 Features
✅ **Encryption and Decryption** options  
✅ **Supports both uppercase & lowercase letters**  
✅ **Input validation** (ensures the key is between 0-25)  
✅ **User-friendly menu-driven program**  

---

## 📌 How It Works
1. **Encryption**: Shifts each letter forward by a given key.
2. **Decryption**: Shifts each letter backward by the same key.
3. **Only alphabetic characters** are transformed, keeping spaces and punctuation unchanged.

<div style="border: 2px solid #ddd; padding: 15px; border-radius: 5px; background: #f8f9fa;">
  <h2>Encryption Example with key==3</h2>

  <strong>plaintext</strong>
  <pre style="background:#fff;padding:10px;border-radius:5px;">HELLO</pre>
  
  <strong>ciphertext</strong>
  <pre style="background:#fff;padding:10px;border-radius:5px;">KHOOR</pre>
</div>

<div style="border: 2px solid #ddd; padding: 15px; border-radius: 5px; background: #f8f9fa;">
  <h2>Decryption Example with key==3</h2>

  <strong>ciphertext</strong>
  <pre style="background:#fff;padding:10px;border-radius:5px;">KHOOR</pre>
  
  <strong>Decrypted</strong>
  <pre style="background:#fff;padding:10px;border-radius:5px;">HELLO</pre>
</div>

---
## 📜 How to Run

1. **Compile the program** using a C compiler:
   ```bash
   gcc Caesar_Cipher.c -o cipher
