# CrypticStore
# Django Firebase AES-256 File Encryption Project

This Django project allows authenticated users to encrypt their files using the AES-256 algorithm before uploading them to Firebase storage. Users can view their uploaded files and download the encrypted versions. Additionally, users can decrypt their files using the AES-256 algorithm.

## Features

- User authentication system.
- File encryption using AES-256 algorithm.
- Firebase storage integration.
- Uploading encrypted files.
- Viewing uploaded files.
- Downloading encrypted files.
- Decrypting files using AES-256.

## Setup

1. **Clone the Repository:**
   
 ```bash
 git clone https://github.com/yourusername/django-firebase-aes-256.git
 cd django-firebase-aes-256
```
   
2. **Install Dependencies:**

It's recommended to set up a virtual environment before installing dependencies.
  ```bash 
  python -m venv venv
  source venv/bin/activate  # On Windows, use: venv\Scripts\activate
  pip install -r requirements.txt
  ```

2. **Configure Firebase:**

- Create a Firebase project and set up Firebase Authentication and Firebase Storage.
- Obtain your Firebase credentials and update the `confing` variable of backend/views.py.

3. **Run Migrations:**
  ```
  bash
  python manage.py migrate
  ```
4. **Run the Development Server:**
  ```
  bash
  python manage.py runserver
  Access the application at http://localhost:8000.
  ```
## Usage
1. Create an Account:
- Visit the application and create an account if you don't have one.
2. Login:
- Log in with your credentials.
3. Encrypt and Upload a File:
- Navigate to the upload page.
- Select a file and choose to encrypt and upload it.
- The file will be encrypted using AES-256 and uploaded to Firebase storage.
4. View and Download Encrypted Files:
- Navigate to the "My Files" page.
- You'll see a list of your uploaded files.
- Click on a file to download the encrypted version.
5. Decrypt a File:
- Navigate to the "Decrypt Files" page.
- Select the encrypted file you want to decrypt.
- Provide the decryption key (you set the key during encryption).
- The file will be decrypted and downloaded.
