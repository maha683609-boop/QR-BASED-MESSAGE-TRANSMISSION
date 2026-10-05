# Secure QR Code-Based Message Transmission System

## Project Overview

This project presents a secure message transmission system using AES-256 encryption, QR code generation, OTP authentication, TCP communication, and Wireshark packet analysis.

The system encrypts the original message before transmission. The encrypted data is converted into Base64 format and stored in a QR code. A separate OTP is used to authenticate the receiver before the message is decrypted.

## Objectives

- To securely encrypt messages using AES-256.
- To store encrypted data in a QR code.
- To provide OTP-based receiver authentication.
- To transmit encrypted data using TCP communication.
- To analyze the transmitted packets using Wireshark.
- To prevent message decryption when an incorrect OTP is entered.

## System Workflow

Original Message
↓
AES-256 Encryption
↓
Base64 Encoding
↓
QR Code Generation
↓
QR Code Scanning
↓
OTP Verification
↓
AES-256 Decryption
↓
Original Message

## Technologies Used

- Python
- AES-256 Encryption
- QR Code
- OTP Authentication
- TCP/IP
- Wireshark
- Visual Studio Code

## Project Files

### Python Programs

- `sender.py` – Encrypts the message and sends the encrypted data.
- `receiver.py` – Receives the encrypted data and decrypts it.
- `qr_generator.py` – Generates the QR code and OTP.
- `qr_decoder.py` – Verifies the OTP and decrypts the QR data.

### Output and Documentation

- `Secure_QR_Program_Outputs.pdf` – Program execution outputs.
- `Secure_QR_Python_Source_Code.pdf` – Python source code.
- `Secure_QR_Code.pdf` – Generated encrypted QR code.
- `Wireshark_Actual_Output.pdf` – Wireshark packet capture output.

## Security Features

### AES-256 Encryption

The original message is encrypted using AES-256 before transmission.

### QR Code

The encrypted Base64 data is stored in the QR code. The original plaintext message is not stored in the QR code.

### OTP Authentication

A six-digit OTP is generated separately. The receiver must enter the correct OTP before the encrypted message can be decrypted.

### Wireshark Analysis

Wireshark is used to capture and analyze the TCP communication through port 5000.

## Testing

The system was tested using:

1. Correct OTP – Message successfully decrypted.
2. Incorrect OTP – Decryption blocked.
3. TCP communication – Encrypted data successfully transmitted.
4. Wireshark capture – TCP packets successfully captured and analyzed.

## Result

The proposed system successfully performs encrypted message transmission, QR code generation, OTP authentication, message decryption, and network packet analysis using Wireshark.

## Project Type

Academic / Course End Project

## Author

Mahalakshmi

Electronics and Communication Engineering  
Velammal Engineering College, Chennai
