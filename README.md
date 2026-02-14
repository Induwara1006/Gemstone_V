# 💎 Gemstone Detection using YOLOv8

An end-to-end **object detection system** built using YOLOv8 to identify multiple types of gemstones from images. This project demonstrates practical implementation of computer vision techniques including data annotation, class balancing, model training, and evaluation.

---

## 🚀 Project Overview

- Developed a custom dataset with **469 images** and **1074 annotated objects**
- Implemented **deterministic + class-balanced data splitting**
- Addressed class imbalance using **data augmentation and duplication**
- Trained a **YOLOv8m model** using Ultralytics
- Evaluated model with detailed performance metrics

---

## 📊 Results

| Metric        | Value |
|--------------|------|
| Precision     | 0.737 |
| Recall        | 0.775 |
| mAP@50        | **0.763** |
| mAP@50-95     | **0.604** |

---

## 🧠 Classes Detected

- Tigers_Eye  
- Obsidian  
- Lapis_Lazuli  
- Rose_Quartz  
- Red_Jasper  
- Clear_Quartz  
- Amethyst  
- Aventurine  

---

## 🛠 Tech Stack

- Python  
- PyTorch  
- YOLOv8 (Ultralytics)  
- OpenCV  
- Label Studio  
- Kaggle  

---

## 📂 Project Structure

gemstone-detection-yolov8/
│
├── notebooks/
│   └── training_notebook.ipynb
│
├── models/
│   └── yolov8m_gemstone.pt
│
├── data/
│   ├── images/
│   └── labels/
│
├── reports/
│   └── gemstone_detection_report.pdf
│
├── requirements.txt
├── data.yaml
└── README.md

---

## ▶️ How to Run

### 1️⃣ Clone the repository
```bash
git clone https://github.com/your-username/gemstone-detection-yolov8.git
cd gemstone-detection-yolov8
```
2️⃣ Install dependencies
```bash
pip install -r requirements.txt
```
3️⃣ Train the model
```python
from ultralytics import YOLO

model = YOLO("yolov8m.pt")
model.train(data="data.yaml", epochs=150, imgsz=640)
```
4️⃣ Run inference
```python
model.predict(source="test.jpg", save=True)
```

## 📈 Key Features
✔ Custom labeled dataset using Label Studio  
✔ Class-balanced deterministic data splitting  
✔ Advanced augmentation (Mosaic, MixUp, HSV)  
✔ Strong detection performance across multiple classes  
✔ Detailed per-class evaluation

## ⚠️ Challenges & Solutions
**Class Imbalance:**
- Some classes had fewer samples
- Solved using duplication and augmentation techniques

**Data Quality:**
- Ensured high-quality annotations through manual verification

## 🔮 Future Improvements
- Increase dataset size for underrepresented classes
- Use larger models (YOLOv8l)
- Apply hyperparameter tuning for further performance gains

## 📄 Report
Full project report is available in:
- `reports/gemstone_detection_report.pdf`

## 🤝 Acknowledgements
- Ultralytics YOLOv8
- Kaggle for training environment
- Label Studio for annotation

## 📬 Contact
Induwara Abhisheka  
Feel free to connect on LinkedIn 🚀

⭐ If you found this project useful, consider giving it a star!

---

# 🔥 Why this README is powerful

✔ Clean structure  
✔ Shows results immediately (recruiters love this)  
✔ Explains your thinking (very important)  
✔ Easy to run  
✔ Looks like a **real ML project repo**

---

## 💡 Final tip (VERY IMPORTANT)

After pushing:

👉 Add **GitHub repo link to your LinkedIn project**  
👉 Pin this repo on your profile  

---

If you want next:
✅ I can create a **GitHub banner image (🔥 looks amazing)**  
✅ Add **demo images section**  
✅ Help you prepare **interview answers from this project**

Just tell me 👍
