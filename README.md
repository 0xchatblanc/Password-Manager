# 🔐 Password-Manager

## 📑 Table of Contents

- [🔍 About](#about)
- [✨ Features](#features)
- [⚙️ Setup And Installation](#setup-and-installation)
- [🚀 Usage](#usage)
- [📜 License](#license)

---

## 🔍 About

**Password-Manager** is an interactive **command-line interface (CLI)** tool designed to securely store and manage sensitive information. It uses powerful encryption techniques to ensure your data remains private and protected:

- 🛡️ **bcrypt**: For hashing and verifying the master password.
- 🔒 **cryptography.fernet**: For encrypting and decrypting data.

This program allows you to:
- Add, view, update, and delete your data.
- Import/export JSON files.
- Secure data with a master password.
- Manage encryption keys dynamically.

---

## ✨ Features

- 🔑 **Master Password Protection**: Secure your data using a hashed master password.
- 🧩 **Encryption/Decryption**: Leverages Fernet encryption for secure storage.
- 🔄 **Key Management**:
  - Generate a new encryption key.
  - Load an existing key.
  - Re-encrypt data with a new key.
- 📁 **Data Management**:
  - Add or update entries easily.
  - View specific entries or the entire dataset.
  - Delete entries.
- 📤 **Import/Export**: Seamlessly import or export data in JSON format.
- 🖥️ **Interactive CLI**: User-friendly and intuitive menu-driven interface.

---

## ⚙️ Setup And Installation

Follow these simple steps to set up **Password-Manager**:

1. Clone the repository:
```bash
git clone https://github.com/0xchatblanc/Password-Manager.git
cd Password-Manager
```

2. Install the required dependencies:
```bash
pip install -r requirements.txt
```

3. Run the application:
```bash
python main.py
```

---

## 🚀 Usage

Upon starting the application, you will be prompted to authenticate with your **master password**. If no master password exists, the application will guide you to set one.

### 🛠️ Menu Options
1. **Show Data** 📂: View all stored data or data at a specific path.
2. **Add/Update Data** ✏️: Add new entries or update existing ones.
3. **Delete Data** 🗑️: Remove entries from the dataset.
4. **Change Key** 🔄: Generate a new encryption key and re-encrypt existing data.
5. **Export to JSON** 📤: Save data as a JSON file.
6. **Import from JSON** 📥: Load and merge data from a JSON file.
7. **Quit** ❌: Exit the application.

### 🔐 How It Works

- **Encryption Key**: The key is stored in a file (`key.key`) and is essential for encrypting and decrypting your data.
- **Data Storage**: Data is securely saved in an encrypted file (`data.enc`) using JSON formatting.
- **Master Password**: The master password is hashed with bcrypt and stored in `password.hash` for authentication.

### ⚠️ Security Considerations

- **Key Management**: Losing the encryption key will make your data irretrievable. Keep it safe!
- **Strong Password**: Choose a strong and unique master password to prevent unauthorized access.

---

## 🔧 Example

Here’s a quick example of how to add, view, and update your data:

1. Start the program and authenticate with your master password.
2. Select option `2` (Add/Update Data).
3. Provide a location path (e.g., `accounts/github`) and enter the value (e.g., `my-github-password`).
4. To view the added data, select option `1` (Show Data) and input the same path (`accounts/github`).

---

## 📜 License

This project is licensed under the **Apache License 2.0** - see the [LICENSE](https://github.com/0xchatblanc/Password-Manager/blob/main/LICENSE) file for more details.

---

## 💬 Stay Connected

Created with ❤️ by **0xchatblanc**. For questions or suggestions, feel free to reach out or contribute to the repository! 🌟
