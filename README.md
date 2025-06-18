# Cyber_Security
🔐 AES + Steganography Image Encoder

This project is a Python-based tool that combines AES encryption and LSB image steganography to securely hide secret messages inside images. It supports dynamic text, user-defined keys, and real-time image upload—ideal for secure data hiding and transmission.

> ✅ Compatible with Google Colab, Jupyter Notebooks, and supports .png/.jpg image formats.




---

🚀 Features

🔏 AES Encryption (CBC Mode) using custom key

🖼️ LSB Image Steganography to hide encrypted data in image pixels

🔐 Secret message and key entered at runtime

📸 Image upload support (via Google Colab or local file system)

🧠 Robust decryption with error handling

📥 Automatic saving and downloading of encoded images

📊 Output visualization using matplotlib

🔁 End-to-end encode/decode workflow



---

📂 Folder Structure

.

├── stego_output/              # Folder for output image

├── notebook.ipynb             # Jupyter/Colab-compatible notebook

├── README.md                  # This documentation file


---

📦 Dependencies

Install using:

pip install opencv-python pycryptodome matplotlib

Or for Google Colab:

!pip install opencv-python pycryptodome


---

💡 How It Works

🔐 Step 1: Encryption

The user provides a secret message and a 16-character key.

The message is encrypted using AES (CBC mode).


🖼️ Step 2: Encoding

The encrypted message is converted into binary.

It is hidden inside the Least Significant Bits (LSBs) of image pixels.


🔓 Step 3: Decoding & Decryption

The receiver uploads the encoded image and enters the key.

The program extracts the encrypted data and decrypts it using AES.



---

📸 Example

🔐 Enter the secret message: Hello

🔑 Enter a 16-character encryption key: mysecretkey12345

✅ Secret message encrypted and hidden in: stego_output/encoded_20250618_101522.png

🖼️ Output Image Displayed with Message Hidden

📤 Decoded Secret Message: Hello


---

🛡️ Security Notes

Uses AES 128-bit encryption for confidentiality.

Only the correct key can successfully decrypt the hidden message.

LSB embedding causes no visible distortion in image.



---

🧪 Use Cases

🔐 Secure communication over public channels

📁 Confidential watermarking

🎓 Educational projects in cybersecurity, cryptography, or image processing

🕵️‍♂️ Covert messaging for research



---

📌 To Do

[ ] GUI version using Tkinter or Streamlit

[ ] Batch image encoding

[ ] Support for audio steganography

[ ] Encryption with password-based key derivation (PBKDF2)



---

👨‍💻 Developed With

Python

OpenCV

PyCryptodome

Google Colab / Jupyter Notebook



---

📄 License

This project is licensed under the MIT License — use it freely for academic, personal, or commercial purposes.


---

