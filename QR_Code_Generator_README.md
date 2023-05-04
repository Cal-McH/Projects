# QR Code Generator

This mini project creates a simple QR code generator taking a string input of the website and the desired QR filename

## Requirements

For this code you will require the qrcode library, "qrcode[pil]" which includes pillow for generating the images, and matplotlib for showing and saving the outputted qrcode

- pip install qrcode
- pip install "qrcode[pil]"
- pip install matplotlib

## Method

The qr_gen() function is defined which takes two inputs, the website, and the desired filename for the QR code image and Qr code data

A QR Code is created with the recomended example parameters as shown in https://pypi.org/project/qrcode/

This uses the uses the version=None parameter which allows the QR code to change size as necessary and the error_correction parameter which allows the QR code to correct any errors (ERROR_CORRECT_M corrects ~15% of error).

The inputted website data is added to the QR plot, and the QR code is rescalled depending on the required size of the plot using the fit=True parameter.

The plot is then created using black as the fill colour, shown using matplotlib using the gray colormap, and saved as a png using matplotlib with a transparent background using the filename concatenated with the .png suffix

