# OTP Verification System

## Description

This Python project implements a secure One-Time Password (OTP) verification system using email authentication. The system generates a random 6-digit OTP and sends it to the user's registered email address for verification during the login process.

## Key Features

- **Random OTP Generation**: Creates a secure 6-digit OTP using Python's `random` module
- **Email Validation**: Verifies email format and checks against common domains (Gmail, Yahoo, Outlook, etc.)
- **SMTP Integration**: Uses Gmail's SMTP server to send OTP emails securely
- **Error Handling**: 
  - Validates email format (presence of "@" and valid domain/TLD)
  - Handles incorrect OTP entries with resend options
- **Security Measures**:
  - Clears email variables from memory after use
  - Uses TLS encryption for email transmission
  - Supports app passwords for secure authentication

## Workflow

1. User enters their email address
2. System validates the email format
3. Generates and sends a 6-digit OTP
4. User enters the received OTP
5. System verifies the OTP match
6. Provides options to resend OTP or use a different email if verification fails

## Technical Implementation

- Built with Python 3.9.7
- Uses `smtplib` for email functionality
- Implements recursive functions for email validation and OTP resending
- Includes proper memory cleanup for sensitive data

## Use Cases

- Secure user authentication systems
- Password reset functionality
- Two-factor authentication (2FA) implementations
- Account verification processes

The project demonstrates core security principles while maintaining user-friendly interaction for email-based verification systems.
