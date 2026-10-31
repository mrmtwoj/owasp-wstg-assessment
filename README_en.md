# OWASP WSTG Assessment Tool & Checklist Editor

![OWASP WSTG Assessment](https://img.shields.io/badge/OWASP-WSTG%20Assessment-blue.svg)
![Version](https://img.shields.io/badge/version-3.0-green.svg)
![License](https://img.shields.io/badge/license-MIT-orange.svg)
![RTL Support](https://img.shields.io/badge/RTL-Supported-success.svg)

A web-based, fully client-side and offline tool for conducting web security assessments based on the OWASP Web Security Testing Guide (WSTG), featuring a dedicated checklist editor and full multilingual support (including Persian with right-to-left alignment).

---

## Key Features

- **100% Offline & Secure Architecture**: No backend server or external database required; all data is processed and stored locally in the browser (`localStorage`).
- **Full Multilingual Support (i18n)**: Supports 7 languages (`fa`, `en`, `zh`, `ru`, `la`, `hi`, `ar`) with automatic RTL detection and handling for Persian and Arabic.
- **Comprehensive Standard Checklist**: Includes 10 core OWASP categories and over 248 structured security tests with WSTG codes and CWE mappings.
- **Advanced Reporting**: Export and import assessment data via JSON, plus a specialized Word (`.doc`) report generator dedicated to failed tests, complete with POC images and notes.
- **Evidence Management (POC)**: Drag-and-drop support for vulnerability screenshots, stored efficiently as Base64.
- **Dedicated Checklist Editor (`editor.html`)**: A separate tool to add, edit, enable/disable tests, and update the master `checklist.json` file.

---

## Project Structure

The project consists of three main files:

- `index.html` : The main assessment and security testing application
- `editor.html` : Graphical editor for managing and editing the checklist
- `checklist.json` : Master reference data file (including 248 tests across 10 categories with 7-language support)

---

## Getting Started

This project requires no compilers, package managers (like NPM), or local servers.

1. Clone the repository or download the files:
   `git clone https://github.com/your-username/owasp-wstg-assessment.git`
2. Open `index.html` in any modern web browser to start your security assessment.
3. To edit or add new tests, open `editor.html` in your browser, make your modifications, and download/replace the updated `checklist.json` file.

---

## Technical Specifications (`checklist.json`)

- Number of Categories: 10 sections (aligned with web assessment standards)
- Total Tests: 248 structured security tests
- Test Fields: Includes ID, WSTG code, severity level (Critical, High, Medium, Low), description, test objectives, sample payloads, and remediation guidance.

---

## Author

Designed and developed by **Mohammad Javad Joshani (MR.MTwoJ)**

---

## License

This project is licensed under the **MIT License**.
