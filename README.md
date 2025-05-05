<<<<<<< HEAD
# Secretsharing
=======
# Secret Sharing Android App

This Android application allows you to securely share secrets by splitting them into multiple shares using Shamir's Secret Sharing scheme. The app supports both text and image-based secret sharing.

## Prerequisites

Before you begin, ensure you have the following:
- Android Studio (latest version recommended)
- Android device running Android 5.0 (Lollipop) or higher
- USB cable to connect your device to your computer
- USB debugging enabled on your Android device

## Installation Steps

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

3. **Build the Project**
   - Wait for Gradle to sync and download dependencies
   - Click on "Build" > "Make Project" (or press Ctrl+F9)

4. **Run the App**
   - Connect your Android device via USB
   - Enable USB debugging on your device
   - Click the "Run" button (green play icon) in Android Studio
   - Select your device from the deployment target dialog
   - Click "OK" to install and run the app

### Method 2: Direct APK Installation

1. **Download the APK**
   - Download the latest APK file from the releases section

2. **Install the APK**
   - On your Android device, navigate to the downloaded APK file
   - Tap on the APK file to begin installation
   - If prompted, enable "Install from Unknown Sources" in your device settings
   - Follow the on-screen instructions to complete the installation

## Usage Guide

### Sharing a Secret

1. **Launch the App**
   - Open the Secret Sharing app from your device's app drawer

2. **Choose Secret Type**
   - Select either "Text Secret" or "Image Secret"
   - For text secrets, enter your secret text
   - For image secrets, select an image from your gallery

3. **Configure Share Settings**
   - Enter the total number of shares to generate (n)
   - Enter the minimum number of shares required to reconstruct the secret (k)
   - Click "Generate Shares"

4. **Save Shares**
   - The app will generate QR codes for each share
   - Save each share by clicking the save button
   - Shares will be saved in the app's private storage

### Reconstructing a Secret

1. **Open the App**
   - Launch the Secret Sharing app

2. **Access Saved Shares**
   - Navigate to the "Saved Shares" section
   - Select the shares you want to use for reconstruction

3. **Reconstruct Secret**
   - The app will automatically attempt to reconstruct the secret
   - For text secrets, the reconstructed text will be displayed
   - For image secrets, the reconstructed image will be shown

## Troubleshooting

### Common Issues

1. **App Crashes on Launch**
   - Clear app data and cache
   - Reinstall the app
   - Ensure your device meets the minimum requirements

2. **Cannot Save Shares**
   - Check storage permissions
   - Ensure sufficient storage space is available
   - Restart the app

3. **QR Code Scanning Issues**
   - Ensure good lighting conditions
   - Hold the QR code steady
   - Clean the camera lens

### Permissions Required

The app requires the following permissions:
- Storage: To save and load shares
- Camera: To scan QR codes
- Internet: For potential future features

## Support

For issues, feature requests, or questions:
- Open an issue on the GitHub repository
- Contact the development team at [support-email]

## License

This project is licensed under the MIT License - see the LICENSE file for details. 
>>>>>>> 45bfabf (Initial commit)
