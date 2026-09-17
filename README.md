# Image Watermarking Web Application

A web-based image watermarking application built using **Python, Flask, OpenCV, HTML, and CSS**.

The application allows users to upload an image, embed a watermark using an **LSB (Least Significant Bit) steganography-based technique**, and generate a watermarked image.

## Features

* Upload an image through a web interface
* Embed a watermark into the image
* LSB-based watermarking
* Watermark embedded in the blue color channel
* Image processing using OpenCV
* PNG-based output
* Simple and responsive web interface

## Technologies Used

* **Python**
* **Flask**
* **OpenCV**
* **NumPy**
* **HTML5**
* **CSS3**

## How It Works

The application uses an LSB-based technique to embed watermark information into the image.

The watermark data is embedded into the least significant bits of selected pixel values. The blue channel is used for embedding the watermark.

Because the least significant bits have a relatively small contribution to the pixel value, the visual difference between the original and watermarked image can be minimized.

### Processing Flow


User Uploads Image
        ↓
Flask Backend
        ↓
OpenCV Image Processing
        ↓
LSB Watermark Embedding
        ↓
Watermarked Image
        ↓
User Downloads Result


## Installation

Clone the repository:

bash
git clone https://github.com/YOUR-USERNAME/image-watermarking-app.git


Navigate to the project directory:

bash
cd image-watermarking-app


Create a virtual environment:

bash
python -m venv venv


Activate it on Windows:

bash
venv\Scripts\activate


Install the dependencies:

bash
pip install -r requirements.txt


Run the application:

bash
python app.py


Open the local application in your browser:

text
http://127.0.0.1:5000


## Project Structure


image-watermarking-app/
│
├── app.py
├── requirements.txt
├── README.md
├── .gitignore
│
├── templates/
│   └── index.html
│
├── static/
│   └── css/
│       └── style.css
│
├── uploads/
└── output/


## Future Improvements

* Add password-based watermark protection
* Support multiple watermark formats
* Add watermark extraction/verification
* Improve watermark robustness against image compression
* Add image quality metrics such as PSNR and SSIM
* Deploy the application online

## Author

**Subhajit Sarkar**

B.Tech – Computer Science & Technology
