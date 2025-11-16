# 🚀 YOLOv8 Real-Time Object Detection

This project uses the **YOLOv8 (You Only Look Once)** deep learning model to perform **real-time object detection** using your webcam.  
It detects multiple objects simultaneously such as people, laptops, bottles, chairs, phones, vehicles, and more — all in real-time.

---

## ⭐ Features

- Real-time multi-object detection  
- Uses the ultralytics YOLOv8 model  
- Fast and lightweight (YOLOv8n version)  
- Draws bounding boxes, labels, and confidence scores  
- Runs on CPU or GPU  
- Fully beginner-friendly implementation  

---

## 🛠️ Technologies Used

- **Python 3.11**
- **OpenCV (cv2)**
- **Ultralytics YOLOv8**
- **PyTorch**

---

## 📂 Project Structure

YOLO-Detection/
│── obj_detection_yolo.py
│── README.md
---

## 📦 Installation

Install required libraries:

bash
pip install ultralytics opencv-python

Verify YOLO is installed:

python -c "from ultralytics import YOLO; print('YOLO Installed')"

▶️ How to Run

1.Clone or download this repository

2.Open the folder in Terminal or CMD

3.Run the script:

python obj_detection_yolo.py

4.Your webcam will open and start detecting objects

5.Press ESC to exit

🧠 How YOLOv8 Works (Simple)

1.YOLO performs all tasks in a single forward pass:

2.Finds objects

3.Predicts bounding boxes

4.Assigns class labels

5.Calculates confidence score

6.Removes duplicate detections (NMS)

That's why YOLO = You Only Look Once.

🧠 Code Explanation (Simple)

model = YOLO("yolov8n.pt")

- Loads the pre-trained YOLOv8 Nano model.

results = model(frame)

- Runs detection on the current frame.

cv2.imshow("YOLOv8", results[0].plot())

- Plots bounding boxes and labels on the frame.

🧪 Example Output

You will see bounding boxes with:

- Object Name

- Confidence Score

- Tracking in real-time

Example detections:

- Person

- Laptop

- Bottle

- Chair

- TV

- Phone

- Vehicle

🚀 Future Improvements

- Add object tracking (SORT/DeepSORT)

- Count objects

- Add region-of-interest alerts

- Use custom-trained YOLOv8 model

- Save detected frames/video

🤝 Contributing

Pull requests and suggestions are welcome!

📜 License

Open-source under the MIT License.
