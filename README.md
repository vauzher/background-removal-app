# Background Removal App

This is a Flask-based web application that allows users to upload images and remove their backgrounds using the `rembg` library. The app provides a simple interface for uploading images and returns a Base64-encoded version of the image with the background removed. It supports common image formats like PNG, JPG, and JPEG.

## Features
- **Flask Backend**: A lightweight web server built with Flask to handle file uploads and image processing requests.
- **rembg Library**: Utilizes the powerful `rembg` tool for background removal.
- **Pillow (PIL)**: Used for image handling and manipulation.
- **Base64 Image Encoding**: After processing, the app returns the image in Base64 format, making it easy to embed in HTML or share over APIs.
- **Frontend Interface**: A minimal HTML, CSS, JS webpage where users can upload images for background removal.

## Project Structure
```
background-removal-app/
│
├── app.py                    # Main Flask application
├── templates/                 # Frontend HTML templates
│   └── upload.html            # HTML template for image upload
├── uploads/                   # Directory for storing uploaded files (if needed)
├── requirements.txt           # List of dependencies
├── README.md                  # Project description (this file)
└── .gitignore                 # Git ignore file
```

## Installation

### Prerequisites
- Python 3.x
- `pip` (Python package installer)

### Steps

1. **Clone the repository:**
   ```bash
   git clone https://github.com/vauzher/background-removal-app.git
   cd background-removal-app
   ```

2. **Create a virtual environment (optional but recommended):**
   ```bash
   python -m venv venv
   source venv/bin/activate  # For Linux/Mac
   # .\venv\Scripts\activate  # For Windows
   ```

3. **Install the dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Run the Flask app:**
   ```bash
   python app.py
   ```

5. **Access the app** in your browser at `http://127.0.0.1:5000/`.

## Usage

1. Open your browser and go to `http://127.0.0.1:5000/`.
2. Use the upload form on the page to select an image (PNG, JPG, or JPEG).
3. After submitting the image, the app will process the image and remove the background.
4. The result will be returned as a Base64-encoded string, which you can use in web applications.

## Contributing

Contributions are welcome! If you have any suggestions or improvements, feel free to fork the repository and submit a pull request.


## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

