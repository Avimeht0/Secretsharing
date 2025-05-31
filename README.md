# Secret Sharing Scheme

## Overview
This Android application implements a secret sharing scheme using QR codes, allowing users to securely share secrets by splitting them into multiple shares using Shamir's Secret Sharing scheme. The app supports both text and image-based secret sharing.

## Table of Contents
- [Features](#features)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage Guide](#usage-guide)
- [Development](#development)

## Features
- **Share Construction**
  - Generate QR codes for secret sharing
  - Support for both text and image secrets
  - Configurable number of shares (n) and threshold (k)
- **Share Reconstruction**
  - Reconstruct secrets from shared QR codes
  - Support for both text and image reconstruction
- **File Management**
  - View and share generated QR code images
  - Multiple file selection support
  - System image viewer integration

## Prerequisites
- Android Studio (latest version recommended)
- Android device running Android 6.0 (API level 23) or higher
- USB debugging enabled on your Android device
- Android SDK with build tools installed

## Installation

### Method 1: Using Android Studio (For Developers)
1. **Clone the Repository**
   ```bash
   git clone [repository-url]
   cd SecretSharing
   ```

2. **Open the Project**
   - Launch Android Studio
   - Click on "Open an existing project"
   - Navigate to and select the project directory

3. **Build and Install**
   ```bash
   # Build the debug version
   ./gradlew assembleDebug

   # Install on connected device
   ./gradlew installDebug
   ```

### Method 2: Direct APK Installation
1. Download the latest APK file from the releases section
2. On your Android device:
   - Navigate to the downloaded APK file (usually in `/storage/emulated/0/Download/` or `/sdcard/Download/`)
   - The APK will be named `app-debug.apk` and located in `app/build/outputs/apk/debug/` of the project directory
   - Tap to begin installation
   - Enable "Install from Unknown Sources" if prompted
   - Follow on-screen instructions

## Usage Guide

### Sharing a Secret
1. **Launch the App**
   - Open the Secret Sharing app from your device's app drawer

2. **Choose Secret Type**
   - Select "Share Construction"
   - Choose between text or image secret
   - For text: Enter your secret text
   - For image: Select an image from your gallery

3. **Configure Share Settings**
   - Set total number of shares (n)
   - Set minimum shares required (k)
   - Click "Generate Shares"

4. **Save and Share**
   - QR codes will be generated for each share
   - Use the 3-dots menu to:
     - Share files: Select and share multiple images
     - View files: Select and view images using system viewer

### Reconstructing a Secret
1. **Open the App**
   - Launch the Secret Sharing app

2. **Access Shares**
   - Select "Share Reconstruction"
   - Choose saved shares for reconstruction

3. **View Results**
   - For text secrets: Reconstructed text will be displayed
   - For image secrets: Reconstructed image will be shown

## Development
This project is built using:
- **Kotlin**: Primary programming language
- **Jetpack Compose**: Modern Android UI toolkit
- **AndroidX Libraries**: Core Android components
- **ZXing**: QR code generation and scanning
- **Shamir's Secret Sharing**: Core secret sharing algorithm

## Contributing
1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

