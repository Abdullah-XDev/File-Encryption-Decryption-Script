![Alt text](RE.png)

# File Encryption/Decryption Script

This project includes two Python scripts: one for encrypting files and another for decrypting them. These scripts use the `cryptography` library, specifically the `Fernet` symmetric encryption method, to encrypt and decrypt files in the current directory.

## Features
- **File Encryption:** Encrypts all files in the current directory (except for specific scripts and the key) using a randomly generated secret key.
- **File Decryption:** Decrypts the files using a secret key and a user-provided secret phrase.

## Prerequisites
Ensure you have the following Python package installed:
- `cryptography`

You can install it using pip:
```bash
pip install cryptography
```
## How It Works
### Encryption:

The encryption script will encrypt all files in the directory (excluding itself, decrypt.py, and thekey.key).
It will generate a random encryption key and save it as thekey.key.
The encrypted files will overwrite the originals.

### Decryption:

To decrypt the files, you must enter a secret phrase (NotMe).
If the correct phrase is entered, the script will decrypt all files in the directory using the saved encryption key (thekey.key).
If the wrong phrase is entered, the decryption will not occur.

## How to Use
1. Encrypt Files:
Run the encrypt.py script to encrypt files in your current directory.
The script will generate an encryption key (thekey.key) and encrypt all files.
```bash
python3 encrypt.py
```
2. Decrypt Files:
Run the decrypt.py script to decrypt the files.
Enter the secret phrase (NotMe) when prompted to decrypt your files.
```bash
python3 decrypt.py
```
3. Important Files:
thekey.key: This file contains the secret key used to encrypt and decrypt the files. Keep it safe!
Encrypted.py: The script used for encryption.
decrypt.py: The script used for decryption.

## Disclaimer
This script is for educational purposes only. Unauthorized encryption and decryption of files may be illegal. Use responsibly and only on files you have explicit permission to work with.
