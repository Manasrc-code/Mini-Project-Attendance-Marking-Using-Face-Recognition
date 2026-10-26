# Mini Project: Attendance Marking Using Face Recognition

A real-time face recognition-based attendance system developed using Python, OpenCV, and the `face_recognition` library. The system identifies registered students through a webcam and automatically records their attendance in Excel spreadsheets.

## Features

- Real-time face recognition using a webcam
- Student image capture and registration
- Automatic attendance marking for recognized students
- Facial encoding generation and storage using Pickle
- Attendance records with timestamps and presence status
- Excel-based attendance management using Pandas
- Visual identification with bounding boxes around recognized faces

## Technologies Used

- Python
- OpenCV
- face_recognition
- NumPy
- Pandas
- Pickle
- Excel (`.xlsx`)

## Project Structure

```text
Mini-Project-Attendance-Marking-Using-Face-Recognition/
├── mainsingl.py
├── addimgfolder.py
├── facerecproimg/
│   └── Images/
├── encodefile.p
├── attendance_records/
├── .gitignore
└── README.md
```

*Note: The encoding file and attendance records are generated when the application runs.*

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/Manasrc-code/Mini-Project-Attendance-Marking-Using-Face-Recognition.git
cd Mini-Project-Attendance-Marking-Using-Face-Recognition
```

### 2. Install the required dependencies

```bash
pip install opencv-python face_recognition numpy pandas openpyxl
```

**Note:** The `face_recognition` library depends on `dlib`, which may require additional installation steps depending on your operating system and Python version.

## How to Run

### Step 1: Capture student images

Run the following command:

```bash
python addimgfolder.py
```

- Enter a unique student name or ID.
- Press **SPACE** to capture an image.
- Press **ESC** to exit the camera.

The captured image is saved in the configured student images directory.

### Step 2: Start the attendance system

Run:

```bash
python mainsingl.py
```

The application generates facial encodings for new students, accesses the webcam, and compares detected faces with registered students.

When a registered student is recognized, their attendance is automatically recorded in an Excel spreadsheet with the time and attendance status.

Press **Q** to close the application.

## Attendance Records

Attendance is stored in Excel files containing the following fields:

| Field | Description |
|---|---|
| Name | Student name or ID |
| Time | Attendance timestamp |
| Status | Attendance status |

The attendance files are organized by date and hour.

## Configuration

Update the image and attendance directory paths in the Python scripts to match your local computer before running the application.

Ensure that a working webcam is connected and accessible.

## Future Enhancements

- Graphical user interface for easier operation
- Database integration for student and attendance management
- Daily and monthly attendance reports
- Improved duplicate attendance prevention
- Enhanced recognition reliability and anti-spoofing measures

## Author

**Manas Ravi Chandran**

GitHub: [@Manasrc-code](https://github.com/Manasrc-code)

Project Repository: [Mini-Project-Attendance-Marking-Using-Face-Recognition](https://github.com/Manasrc-code/Mini-Project-Attendance-Marking-Using-Face-Recognition)
