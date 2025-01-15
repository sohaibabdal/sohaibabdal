# My Tester Application

## Overview
My Tester is a Python-based application designed for network scanning and service analysis. It integrates Nmap for scanning and Firebase for storing and managing results. The app features a user-friendly GUI built with CustomTkinter and supports advanced scanning capabilities like deep scans and vulnerability detection.

---

## Features
- **Login and Signup System**: Supports user authentication using Firebase.
- **Network Scanning**:
  - Normal and deep scans using Nmap.
  - Displays port, state, service, version, and vulnerabilities.
  - Simulates and identifies outdated services.
- **GUI Features**:
  - Dark mode support.
  - Responsive, user-friendly design.
  - Log display for activity tracking.
- **Report Generation**:
  - Save scan results as PDF.
  - Email scan results via Postmark API.
- **Real-time Updates**: Listens for new scan requests in Firebase.

---

## Installation

Opens an installation folder you'll find file named Qscan.MSI open it and click next until the appinstalled 

### Prerequisites
1. Python 3.8 or higher.
2. Nmap installed and available in the system PATH.
3. Firebase setup with a valid `scann.json` file.
4. Install the required Python dependencies:
   ```bash
   pip install -r requirements.txt
   ```

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/my-tester.git
   ```
2. Navigate to the project folder:
   ```bash
   cd my-tester
   ```
3. Run the application:
   ```bash
   python fufu.py
   ```

---

## Deployment
### Building Executable
Use PyInstaller to create an executable file:
```bash
pyinstaller --onefile --noconsole fufu.py
```
The generated `.exe` file will be available in the `dist` folder.

---

## Usage
1. Run the application.
2. Log in or sign up.
3. Enter a URL or IP address to scan.
4. Choose scan type (Normal or Deep).
5. View scan results, save them as PDF, or send them via email.

---

## Folder Structure
```
my-tester/
|-- dust/
|   |-- arialroundedmtbold.ttf  # Font file
|   |-- scann.json              # Firebase credentials
|   |-- nmap.exe                # Nmap executable
|
|-- sources/
|   |-- background.png          # Background image
|   |-- person.png              # Person icon
|   |-- email.png               # Email icon
|   |-- lock.png                # Lock icon
|   |-- google_icon.png         # Google icon
|-- fufu.py                     # Main application script
|-- README.md                   # Documentation
|-- requirements.txt            # Python dependencies
```

---

## Dependencies
- Python Libraries:
  - `customtkinter`
  - `subprocess`
  - `Pillow`
  - `firebase-admin`
  - `reportlab`
  - `postmarker`
- External Tools:
  - `nmap`

---

## Contributing
1. Fork the repository.
2. Create a feature branch:
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m 'Add some feature'
   ```
4. Push to the branch:
   ```bash
   git push origin feature-name
   ```
5. Open a pull request.

---

## License
This project is licensed under the MIT License. See `LICENSE` for more details.

---

## Contact
For any questions or support, please contact [your-email@example.com].

