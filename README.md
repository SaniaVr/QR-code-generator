# QR Code Generator

This Python script generates a customizable QR code based on user inputs. It utilizes the `qrcode` library to encode a website link into a QR code, allowing the user to specify its size, border, and colors.

## Features
- Accepts a **website URL** as input.
- Allows customization of:
  - **Version**: Controls the data capacity of the QR code.
  - **Box Size**: Determines the size of each square in the QR code.
  - **Border**: Sets the width of the border around the QR code.
  - **Fill Color**: Sets the QR code's color.
  - **Background Color**: Sets the background color.
- Saves the QR code as an image file (`qr_code.png`) in the current directory.

## Requirements
- Python 3.x
- `qrcode` library  
  Install using:
  ```bash
  pip install qrcode[pil]

## Usage
- Clone or download the script.
- Ensure the required dependencies are installed.
- Run the script:
  ```bash
  python qr_code_generator.py

- Follow the prompts:
   - Enter the website link to be encoded.
   - Specify the version (an integer between 1 and 40; higher values allow more data but increase complexity).
   - Specify the box size (an integer for the size of each square in the QR code).
   - Specify the border size (an integer for the width of the border in squares).
   - Enter the fill color (e.g., black, blue, red).
   - Enter the background color (e.g., white, yellow, green).

## Notes
The version determines the complexity of the QR code:
- Version 1 has 21x21 modules.
- Each increment adds 4 modules to both dimensions.
- Ensure the input for colors matches a valid color name or hexadecimal code (e.g., #000000 for black).
