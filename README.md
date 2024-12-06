Secure Traveler
Project Overview
The Secure Traveler is a cryptography-focused web application designed to provide a secure, user-friendly platform for uploading, storing, and sharing sensitive files. 
The project prioritizes data confidentiality, integrity, and secure access, leveraging three advanced encryption mechanisms to achieve robust security.
Firstly, the Advanced Encryption Standard (AES) is utilized to encrypt file content, ensuring that sensitive data remains private and unreadable by unauthorized parties. 
Secondly, RSA encryption is employed to secure the AES keys used for file encryption, enabling safe key exchange and storage. Only users with access to the corresponding RSA private key can decrypt and retrieve files. 
Finally, SHA-256 hashing ensures data integrity by generating a unique digital fingerprint for each file. This mechanism verifies that no unauthorized changes or tampering have occurred, providing an additional layer of security.
With features like user authentication, a file management dashboard, and detailed encryption information, the Secure Traveler application combines cutting-edge cryptographic techniques with a seamless user experience to address critical security needs in today’s interconnected world.

How to Run the Application
Prerequisites
Python Version: Ensure Python 3.8 or higher is installed.
Dependencies: Install the required Python libraries:
bash
Copy code
pip install flask flask_sqlalchemy werkzeug cryptography

Environment Setup:
A directory named uploads/ will be created automatically for storing encrypted files.
RSA keys (private_key.pem and public_key.pem) are generated during the first run if they do not already exist.

Steps to Run the Application
Clone the Repository:
bash
Copy code
git clone <repository_url>
cd <repository_folder>

Initialize the Database: Run the application once to create the necessary database tables:
bash
Copy code
python app.py

Start the Application: Launch the Flask development server:
bash
Copy code
python app.py
The application will be accessible at http://127.0.0.1:5000.

Application Usage
Sign Up: Register a new account on the /signup page.
Log In: Log into your account through /login.
Dashboard: Upload files for encryption, view file metadata, and manage your files.
Download Files: Decrypt and retrieve files securely.
Delete Files: Remove unwanted files.
Encryption Information: Learn about the cryptographic mechanisms used in the system.
Security Features
AES Encryption: Secures file content during storage and transmission.
RSA Encryption: Protects AES keys, ensuring secure key exchange.
SHA-256 Hashing: Verifies file integrity, preventing tampering.
Secure Authentication: User credentials are hashed and stored safely.
