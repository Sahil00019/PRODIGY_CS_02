# **PROJECT TITLE :**

PIXEL MANIPULATION FOR IMAGE ENCRYPTION

## **DESCRIPTION :**

The Image Encryption and Decryption Tool is a Python application created to protect images by altering their pixels. This tool uses a straightforward encryption method to convert images into a scrambled, unreadable format and then restores them to their original form using a secret key. It’s a great project for learning the basics of image processing and encryption techniques.

### REQUIREMENTS
- **Python `3.x`**: Ensure you have Python 3 installed on your system.
- **Pillow Library**: Install the Pillow library using the command: `pip install pillow`.

### HOW DOES IT WORK?

#### **Encryption Process**
1. **Input**: Provide an image file (e.g., PNG, JPEG) and a encryption key (an integer between 0 and 255).
2. **Pixel Manipulation**:
   - Each pixel in the image consists of three color channels: Red (R), Green (G), and Blue (B).
   - The program performs a bitwise XOR operation on each channel using the secret key.
3. **Output**: The result is an encrypted image that appears scrambled and visually unreadable.

#### **Decryption Process**
1. **Input**: Provide the encrypted image and the same encription key used during encryption.
2. **Pixel Manipulation**:
   - The program reapplies the XOR operation to each pixel’s color channels using the secret key.
   - This reverses the encryption process, restoring the original pixel values.
3. **Output**: The decrypted image is recovered, matching the original image.

### EXAMPLE USAGE

#### **Encrypting an Image**
1. **Input**:
   - Image path: `C:\Users\YourName\Pictures\image.png`
   - Key: `123`
2. **Output**: The encrypted image is saved as `encrypted_image.png`.

#### **Decrypting an Image**
1. **Input**:
   - Image path: `encrypted_image.png`
   - Key: `123` (the same key used for encryption)
2. **Output**: The decrypted image is saved as `decrypted_image.png`.
