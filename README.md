# Face Swap App

A Flask-based web app that swaps faces between two uploaded images using OpenCV and dlib’s 68-face-landmarks predictor, featuring a vibrant orange gradient UI with image previews and animations.

## Features
- Upload source and destination images to swap faces.
- Real-time previews for uploaded images.
- Detects faces using dlib and swaps them with seamless cloning.
- Responsive design with orange gradient theme and hover effects.
- Error handling for missing files or undetected faces.
- Made by Sadik Al Jarif in the navbar.

## Prerequisites
- Python 3.8+
- pip
- Git (optional)
- dlib dependencies (cmake, libopenblas)

## Installation

1. **Clone or download the project:**

```bash
git clone <repository-url>
cd face-swap-app

2. **Create and activate a virtual environment:**

```
python -m venv venv
source venv/bin/activate  
```

3. **Install dependencies:**

```
echo -e "flask\nopencv-python\nnumpy\npillow\nwerkzeug\ndlib" > requirements.txt
pip install -r requirements.txt
```

4. **For dlib on Ubuntu:**

```
sudo apt-get install build-essential cmake libopenblas-dev liblapack-dev libx11-dev libgtk-3-dev
```

5. **On Windows, install Visual Studio Build Tools or use a precompiled dlib wheel.**

```
Set up directories:
```
- Add required files:

- Place shape_predictor_68_face_landmarks.dat in static/dat/.

- Place white_bg.jpg in static/images/.

- Use app.py, templates/index.html, static/style.css, requirements.txt from previous responses.


# Project Structure

```
face-swap-app/
├── static/
│   ├── dat/
│   │   ├── shape_predictor_68_face_landmarks.dat  # dlib face landmarks
│   ├── uploads/                                  # Processed images
│   ├── images/
│   │   ├── white_bg.jpg                          # Default image
│   ├── style.css                                 # Custom styles
├── templates/
│   ├── index.html                                # HTML template
├── app.py                                        # Flask app
├── requirements.txt                              # Dependencies
├── README.md                                     # This file
```

# Usage

### Run the app:

```
python app.py
http://127.0.0.1:5000
```

- Upload images:

- Select source image (face to swap).

- Select destination image (target face).

- View previews.

- Click "Swap" to see the result.

- Errors (e.g., missing files, no faces) display below cards.

