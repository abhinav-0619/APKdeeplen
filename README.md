﻿# APKdeeplen
# APKDeepLens

[Features](#features) • [Installation](#installation) • [Changelog](https://github.com/d78ui98/APKDeepLens/blob/master/CHANGELOG.md)

APKDeepLens is a Python-based tool designed to scan Android applications (APK files) for security vulnerabilities. It specifically targets the OWASP Top 10 mobile vulnerabilities, providing an easy and efficient way for developers, penetration testers, and security researchers to assess the security posture of Android apps.

![APKDeepLens Screenshot](https://github.com/d78ui98/APKDeepLens/assets/27950739/c9236e3d-60d5-4832-85dc-f09a449bade3)

## Features

APKDeepLens offers robust features for APK analysis:

- **APK Analysis**: Scans Android application package (APK) files for security vulnerabilities.
- **OWASP Coverage**: Covers OWASP Top 10 vulnerabilities for comprehensive assessments.
- **Advanced Detection**: Uses custom Python code for APK file analysis and vulnerability detection.
- **Sensitive Information Extraction**: Identifies potential security risks, including insecure authentication/authorization keys and insecure request protocols.
- **In-depth Analysis**: Detects insecure data storage practices, such as SD card data exposure, and insecure request protocols.
- **Intent Filter Exploits**: Pinpoints vulnerabilities in intent filters extracted from AndroidManifest.xml.
- **Local File Vulnerability Detection**: Safeguards against mishandlings related to local file operations.
- **Report Generation**: Generates detailed reports with actionable insights for developers.
- **CI/CD Integration**: Easily integrates into CI/CD pipelines for automated security testing.
- **User-Friendly Interface**: Color-coded terminal outputs for easy distinction of findings.

## Installation

### Prerequisites
- Python 3.10 (recommended) or higher
- Java or OpenJDK

### Steps
#### For Linux
```bash
git clone https://github.com/d78ui98/APKDeepLens.git
cd APKDeepLens
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python APKDeepLens.py --help
```

#### For Windows
```bash
git clone https://github.com/d78ui98/APKDeepLens.git
cd APKDeepLens
python3 -m venv venv
.\venv\Scripts\activate
pip install -r requirements.txt
python APKDeepLens.py --help
```

## Usage

### Basic Scan
To scan an APK file:
```bash
python3 APKDeepLens.py -apk file.apk
```

### Source Code Path
For faster scans using pre-extracted source code:
```bash
python3 APKDeepLens.py -apk file.apk -source <source-code-path>
```

### Report Generation
To generate detailed PDF and HTML reports:
```bash
python3 APKDeepLens.py -apk file.apk -report
```



