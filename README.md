# Real-Time Text Detection using OCR and OpenCV

This project demonstrates a **real-time text detection** system using Python, OpenCV, and Tesseract OCR. It processes live webcam feed or screen captures to detect and recognize text in images.

## **Features**
- Real-time text detection from webcam feed.
- Option to capture and process screen regions.
- Displays bounding boxes and recognized characters on the frame.
- Measures and displays FPS (Frames Per Second) for performance.

---

## **Technologies Used**
- Python
- OpenCV
- Tesseract OCR
- NumPy
- PIL (Python Imaging Library)

---

## **Prerequisites**
### 1. Install Required Libraries
Make sure the following Python libraries are installed:
```bash
pip install opencv-python pytesseract pillow numpy


## **2. Install Tesseract OCR**

Download and install Tesseract OCR from its GitHub page.

Configure the pytesseract.pytesseract.tesseract_cmd variable in the script to point to the installed Tesseract executable. Example:

python
pytesseract.pytesseract.tesseract_cmd = r'C:\Program Files\Tesseract-OCR\tesseract.exe'

**# Project Structure
bash
Copy code
text-detection-ocr/
│
├── text_detection.py       # Main Python script
├── README.md               # Documentation
├── requirements.txt        # List of required Python libraries
└── example.jpg             # Example input image (optional)

Customization
**
Switch to Screen Capture Mode:

Uncomment the capture_screen() function in the code and use it instead of the webcam feed.
Multilingual OCR Support:

Edit the pytesseract.image_to_boxes() call to include multiple languages:
python

boxes = pytesseract.image_to_boxes(img, lang='eng+hin')  # Example: English + Hindi
Save Results to File:

Save the recognized text to a file for further use:
python

detected_text = pytesseract.image_to_string(img)
with open("output.txt", "w") as f:
    f.write(detected_text)
Example Output
Input:

Output:
Bounding boxes and recognized characters overlaid on the input.

License
This project is licensed under the MIT License - see the LICENSE file for details.


---

### **Steps to Upload on GitHub**

1. **Create a Repository**:
   - Go to GitHub and create a new repository (e.g., `text-detection-ocr`).

2. **Add Your Project Files**:
   - Include the following files:
     - `text_detection.py`
     - `README.md`
     - `requirements.txt` (optional but recommended for dependencies)
     - Any example images or additional files.

3. **Push to GitHub**:
   Use the following commands to push your project to GitHub:
   ```bash
   git init
   git add .
   git commit -m "Initial commit for Text Detection project"
   git branch -M main
   git remote add origin https://github.com/your-username/text-detection-ocr.git
   git push -u origin main

4. **Add a Download Link**:
The ZIP download link should look like this:
vbnet
Copy code
https://github.com/your-username/text-detection-ocr/archive/refs/heads/main.zip



