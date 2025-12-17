# Face Attendance System using OpenCV

An automated Face Recognition–based Attendance System built using Python and OpenCV.
This project detects and recognizes faces in real time and marks attendance automatically, eliminating the need for manual attendance tracking.

## Features

- Real-time face detection
- Face recognition using trained data
- Automatic attendance marking
- Attendance stored locally (CSV / text file)
- Fast and lightweight
- Works with live webcam feed

## Technologies Used

- Python 3
- OpenCV
- NumPy
- Haar Cascade Classifier
- LBPH Face Recognizer

## Project Structure
```
OpenCV_FaceAttendance/
│
├── dataset/                  # Collected face images
├── trainer/                  # Trained model files
├── attendance/               # Attendance records
├── haarcascade_frontalface_default.xml
├── face_dataset.py           # Script to collect face data
├── face_training.py          # Script to train the model
├── face_recognition.py       # Main attendance script
├── requirements.txt
└── README.md
```
## Installation & Setup

### 1. Clone the Repository
```
git clone https://github.com/your-username/OpenCV_FaceAttendance.git
cd OpenCV_FaceAttendance
```
### 2. Create Virtual Environment (Optional)
```
python -m venv venv
source venv/bin/activate      # macOS/Linux
venv\Scripts\activate         # Windows
```
### 3. Install Dependencies
```
pip install -r requirements.txt
```
If requirements.txt is missing:
```
pip install opencv-python numpy
```
## How to Run

### Step 1: Collect Face Data

python face_dataset.py

- Enter User ID
- Enter User Name
- System captures multiple images automatically

### Step 2: Train the Model

python face_training.py

- Generates trained face recognition model

### Step 3: Run Attendance System

python face_recognition.py

- Opens webcam
- Recognizes faces
- Marks attendance automatically

## Attendance Output

Attendance is saved in CSV or text format and includes:
- ID
- Name
- Date
- Time

Example:
```
ID, Name, Date, Time
101, Kartikeya, 2025-03-01, 10:12:30
```
## Face Detection Model

Uses Haar Cascade Classifier:

haarcascade_frontalface_default.xml

Make sure this file is present in the project root.

## Common Issues & Fixes

Camera not opening:
- Check webcam permissions
- Try changing camera index (cv2.VideoCapture(0) to cv2.VideoCapture(1))

Low recognition accuracy:
- Collect more images per person
- Ensure good lighting
- Face should be clearly visible

## Future Improvements

- GUI using Tkinter or Streamlit
- Cloud-based attendance storage
- Multiple camera support
- Face mask detection
- Database integration (MySQL or Firebase)

## License

This project is for educational purposes.
You are free to modify and enhance it.

## Acknowledgements

- OpenCV Community
- Python Developers 

<img width="413" alt="Screenshot 2025-05-26 at 10 10 56 AM" src="https://github.com/user-attachments/assets/d3ea68b5-6501-42ff-987a-4d25b1675bc7" />
.
.
.
.
.
<img width="470" alt="Screenshot 2025-05-26 at 10 12 20 AM" src="https://github.com/user-attachments/assets/8b6aecdd-098a-49cf-96f9-751a4fb151d2" />
.
.
.
.
.
<img width="516" alt="Screenshot 2025-05-26 at 10 12 43 AM" src="https://github.com/user-attachments/assets/1d07ac9d-3829-4c35-8166-c565b1b7ff9b" />
