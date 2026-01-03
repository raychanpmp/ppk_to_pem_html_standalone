# PuTTY to OpenSSH Key Converter (Client-Side)

A secure, browser-based utility designed to convert PuTTY Private Key (`.ppk`) files into OpenSSH PEM format.

This tool is designed for strict data isolation. It functions entirely within the web browser, ensuring sensitive cryptographic material is never transmitted over a network.

---

## Security & Privacy

> **Critical Note:** All processing occurs locally within your browser instance. Your private keys, passphrases, and file contents are **never** uploaded to, stored on, or processed by any remote server.

* **Zero Transmission:** The conversion logic runs via client-side JavaScript.
* **Audit-Ready:** The code is contained in a standalone HTML file, allowing for easy code review and security auditing.
* **No Persistence:** Data is cleared from memory once the browser tab is refreshed or closed.

---

## Key Features

* **Format Conversion:** Converts standard `.ppk` files to OpenSSH PEM format compatible with Linux/Unix environments and AWS.
* **Dual Input Methods:** Supports direct text pasting or file uploading for flexibility.
* **Encryption Support:** Full support for passphrase-protected keys.
* **Instant Download:** Generates downloadable key files immediately upon conversion.

---

## Usage Instructions

1.  **Select Input Method:**
    * **Option A:** Copy the content of your `.ppk` file and paste it into the provided text area.
    * **Option B:** Click "Upload" to select the `.ppk` file from your local machine.
2.  **Authenticate (If Required):**
    * If your key is encrypted, enter the passphrase in the designated field.
3.  **Convert:**
    * Click the **"Convert to OpenSSH Keys"** button.
4.  **Retrieve:**
    * Use the download buttons to save your new OpenSSH key to your local secure storage.

---

## Technical Details

* **Architecture:** Standalone HTML/JavaScript application.
* **Dependencies:** pure-JavaScript implementation (client-side only).

