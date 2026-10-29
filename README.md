# QR Code Generator 🔳

A beginner-friendly Python project built in Jupyter Notebook to generate QR codes for text, website URLs, and UPI payments. It also includes a basic example of extracting text from an image using OCR.

## Features

- Generate a QR code from text or other input.
- Generate website QR codes with an HTTP/HTTPS prefix check.
- Customize QR code colors, box size, border, and error correction.
- Generate UPI payment QR codes.
- Generate UPI QR codes with a specified amount.
- Save generated QR codes as PNG images.

## Technologies Used

- Python
- Jupyter Notebook
- qrcode
- Pillow

## Installation

Install the required Python libraries:

```bash
pip install qrcode pillow pytesseract
```

To use the OCR example, Tesseract OCR must also be installed on your system and available in your PATH. Installing `pytesseract` alone does not install the OCR engine.

## How to Run

1. Download or clone this repository.
2. Open `QR Code project.ipynb` in Jupyter Notebook or VS Code.
3. Run the installation cells if the required libraries are missing.
4. Run the example you want to use.
5. Enter the requested text, URL, or payment details.
6. Find the generated PNG file in the notebook's working directory.

The examples can be run individually after installing their dependencies.

## Examples Included

| Example | Description | Output File |
|---|---|---|
| Basic QR Code | Converts user input into a QR code | `FirstQR_2026_MCA.png` |
| Website QR Code | Checks for an HTTP/HTTPS prefix and generates a QR code | `FirstQR.png` |
| Customized QR Code | Generates a QR code with custom colors and settings | `Third_QR.png` |
| UPI QR Code | Encodes a UPI ID and recipient name | `Ravi_UPI2.png` |
| Fixed-Amount UPI QR Code | Encodes a UPI ID, recipient name, and amount | `Specific amount.png` |

## UPI QR Code Format

The notebook uses the following URI formats:

**Without a specified amount:**

```text
upi://pay?pa=YOUR_UPI_ID&pn=YOUR_NAME
```

**With a specified amount:**

```text
upi://pay?pa=YOUR_UPI_ID&pn=YOUR_NAME&am=AMOUNT
```

Scanning a UPI QR code opens the encoded payment details in a compatible app. Payment still requires the user's confirmation.

## Concepts Practiced

- User input and output
- Conditional statements
- String methods
- Formatted strings (f-strings)
- Integer conversion
- Python library usage
- QR code customization
- Saving image files
- Basic optical character recognition

## Notes

- Website checking only verifies whether the input starts with `http://` or `https://`; it does not verify that the website exists.
- The fixed-amount example currently accepts whole-number amounts.
- Running an example again overwrites its existing output image.
- For OCR, place `www.png` in the working directory or update the image path.
- Use strong contrast between QR foreground and background colors for reliable scanning.

## Author

**Ravi Kumar**  
MCA — Artificial Intelligence & Machine Learning  
Invertis University
