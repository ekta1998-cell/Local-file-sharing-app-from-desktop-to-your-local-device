# Local-file-sharing-app-from-desktop-to-your-local-device
# Local Web Server with QR Code Access

This Python script sets up a basic HTTP web server on your local machine and generates a QR code that can be scanned to access the server. It serves the files located on your desktop, making them accessible to other devices on the same network.

## Features
- Serves files from your desktop on a local web server.
- Generates a QR code that links to the server, making it easy to share with other devices.
- Compatible with any device that can scan QR codes.

## Prerequisites
- Python 3.x
- Required Python modules: `http.server`, `socket`, `socketserver`, `webbrowser`, `pyqrcode`, `png`, `os`

## Installation

1. Clone the repository to your local machine:
    ```bash
    git clone https://github.com/ekta1998-cell/Local-file-sharing-app-from-desktop-to-your-local-device.git
    ```
2. Navigate to the project directory:
    ```bash
    cd your-repository-name
    ```
3. Install the required Python modules:
    ```bash
    pip install pyqrcode pypng
    ```

## Usage

1. Run the Python script:
    ```bash
    python3 your-script-name.py
    ```
2. The script will start a local web server on port 8010.
3. A QR code will be generated and opened in your default web browser.
4. Scan the QR code with any device to access the files being served.

## How It Works

- The script changes the directory to your desktop and serves the files from there.
- It uses the `http.server` module to create a basic HTTP server.
- The `pyqrcode` module is used to generate a QR code that contains the IP address and port of the server.
- The QR code is saved as an SVG file and opened in your default web browser.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
