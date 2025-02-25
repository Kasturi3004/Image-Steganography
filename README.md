# Image-Steganography
# Image Steganography using OpenCV

## Overview
This project provides a simple implementation of image steganography using OpenCV. It allows users to encrypt a secret message into an image and later decrypt it using a passcode.

## Requirements
Ensure you have the following installed before running the script:
- Python 3.x
- OpenCV (`cv2`)

Install OpenCV using pip if not already installed:
```sh
pip install opencv-python
```

## How It Works
### Encryption
1. The user inputs a secret message and a passcode.
2. The message is encoded into pixel values of the selected image.
3. The modified image is saved as `encryptedImage.jpg`.

### Decryption
1. The user is prompted to enter the passcode.
2. If the passcode matches, the message is retrieved from the image.
3. If the passcode is incorrect, access is denied.

## Usage
### Running the Script
```sh
python script.py
```

### Example Workflow
1. Provide an image path in the script (modify `img_path` accordingly).
2. Enter the secret message when prompted.
3. Set a passcode for encryption.
4. The script encrypts the message and saves a new image.
5. Run the script again to decrypt the message by entering the correct passcode.

## Important Notes
- The encryption alters pixel values, so the decrypted message is only readable if the original image is used.
- Ensure the image has enough pixels to store the entire message.
- This method does not provide strong security; it's a basic implementation for educational purposes.

## License
This project is open-source and available for educational and personal use.

