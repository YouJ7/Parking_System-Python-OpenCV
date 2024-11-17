# **Parking Space Detection and Counter**

A real-time parking space detection and counting system built using **Python** and **OpenCV**. This project identifies parking spaces in a video feed and counts the available spots dynamically, providing a visual representation of occupied and free spaces.

---

## **Features**
- Detects parking spaces in a video or image feed.
- Counts available (free) parking spots in real time.
- Visualizes parking spaces with bounding boxes:
  - **Green**: Free spots.
  - **Red**: Occupied spots.
- Interactive parking space selection using a GUI.

---

## **Demo**
![Demo Screenshot](carPark.png)

*The system displays the number of free parking spaces and overlays boxes on detected spots.*

---

## **How It Works**
1. **Parking Space Picker:**
   - Use the **ParkingSpacePicker.py** script to manually mark parking spaces in an image.
   - Save the positions of parking spots to a file (`CarParkPos`).

2. **Parking Space Detector:**
   - The **main.py** script processes a video feed to analyze parking spaces.
   - It uses adaptive thresholding and morphological operations to detect parked vehicles.

---

## **Technologies Used**
- **Programming Language:** Python
- **Libraries:**
  - OpenCV: For image and video processing.
  - cvzone: For overlaying text and rectangles on images.
  - pickle: For storing and loading parking space coordinates.

---

## **Project Structure**
.
├── main.py                 # Detects parking spaces in the video feed
├── ParkingSpacePicker.py   # GUI tool to select parking spaces
├── carPark.mp4             # Sample video for parking space detection
├── carParkImg.png          # Image used for marking parking spaces
├── CarParkPos              # Saved parking positions (generated dynamically)
├── requirements.txt        # Required Python packages
└── README.md               # Project documentation


## **Setup Instructions**

### **Prerequisites**
- Python 3.6 or higher.
- Required Python packages: OpenCV, cvzone, NumPy.

### **Installation**
1. Clone this repository:
   ```bash
   git clone https://github.com/YouJ7/parking-space-detection.git
   cd parking-space-detection
   
2. Navigate to Project Directory:
  ```bash
   cd ParkingSpaceDetection
```

3. Activate virtual environmnet (Optional but Recommended):
  ```bash
    venv\Scripts\activate
```
4. Install Required libraries:
  ```bash
pip install opencv-python cvzone numpy
```

4. Run the project:
  ```bash
python main.py
```

## License

© Udit Joshi
