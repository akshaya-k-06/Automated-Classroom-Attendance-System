# 🎓 Automated Classroom Attendance System

> **Best Paper Award** — 8th International Conference on Recent Trends in Technology, Engineering and Applied Science (ICRTTEAS 2025-26), Nov 21–22, 2025
> **1st Prize** — Intra College Project Expo 2025, Dr. T. Thimmaiah Institute of Technology, KGF

---

## 📌 Overview

An AI-powered, contactless classroom attendance system that automates student identification from a single classroom photograph using a two-stage deep learning pipeline — **YOLOv8** for multi-face detection and **ArcFace** for accurate face recognition.

Designed to replace traditional manual roll-call and biometric systems with a scalable, hygienic, and efficient computer vision solution suitable for large classrooms.

---

## 👩‍💻 Authors

| Name | USN | Email |
|------|-----|-------|
| Jansi Rani J (Guide) | — | jansiranijesuprakasam@gmail.com |
| **Akshaya K** | 1GV23CS004 | akshukristy@gmail.com |
| Amulya K S | 1GV23CS007 | amulyasiri05@gmail.com |
| Asfa Hana | 1GV23CS009 | hana17asfa@gmail.com |
| Jaya Preethi J | 1GV23CS047 | jpreethi2005@gmail.com |

**Department of CSE, Dr. T. Thimmaiah Institute of Technology, KGF**

---

## 🚀 Key Features

- 📸 **Single image input** — upload one classroom photo, get full attendance
- 👥 **Simultaneous detection** of 60–70 student faces in one frame
- 🧠 **Two-stage AI pipeline** — YOLOv8 (detection) + ArcFace (recognition)
- 📊 **Auto-generates CSV** attendance report with timestamps
- 🌐 **Flask web interface** — intuitive upload portal for instructors
- 🗄️ **Centralized database** — SQLite/MySQL with secure timestamp logging
- 💻 **Lightweight** — runs on standard hardware, GPU not mandatory

---

## 📊 Performance Metrics

| Metric | Result |
|--------|--------|
| **Overall Accuracy** | 80–85% |
| **F1 Score** | Consistently > 0.85 (confidence 0.4–0.8) |
| **Precision** | > 0.9 (recall up to 0.8) |
| **YOLOv8 Face Detection** | ~82% under normal lighting |
| **ArcFace Recognition** | ~84% student identification |
| **FAR & FRR** | Both < 0.05 (minimal errors) |
| **Processing Time** | ~3–4 seconds per classroom image |
| **High-density load** | ~81% accuracy on 70–80 faces, no crash |
| **Low-light performance** | ~78–80% accuracy |

---

## 🛠️ Tech Stack

| Category | Technology |
|----------|-----------|
| **Language** | Python 3.8+ |
| **Face Detection** | YOLOv8 (Ultralytics) — anchor-free, real-time |
| **Face Recognition** | ArcFace — 512-dim embeddings, AAM-Loss |
| **Web Framework** | Flask |
| **Image Processing** | OpenCV |
| **Data Handling** | NumPy, Pandas |
| **Database** | SQLite / MySQL |
| **Deep Learning** | PyTorch |
| **IDE** | VS Code / Jupyter Notebook |
| **OS** | Windows 10/11, Linux (Ubuntu 20.04), macOS |

---

## 🔬 How It Works

```
Classroom Image
      ↓
 Pre-processing & Face Alignment
      ↓
 YOLOv8 Multi-Face Detection
      ↓
 ArcFace — 512-dim Face Embedding
      ↓
 Cosine Similarity → Student Database Match
      ↓
 Attendance Marking + Timestamp
      ↓
 CSV Report Generated
```

**Similarity threshold:** 0.8 — a detected face is matched only if cosine similarity exceeds this value.

---

## 💻 System Requirements

**Hardware (Minimum):**
- Processor: Intel Core i3 or equivalent
- RAM: 4 GB
- Storage: 10 GB free
- Camera: Standard 720p
- GPU: Not mandatory (but accelerates performance)

**Software:**
- Python 3.8+
- PyTorch, OpenCV, Flask, Ultralytics YOLOv8, NumPy, Pandas, SQLite/MySQL

---

## ⚙️ Installation & Setup

```bash
# 1. Clone the repository
git clone https://github.com/akshaya-k-06/Automated-Classroom-Attendance-System.git
cd Automated-Classroom-Attendance-System

# 2. Install dependencies
pip install -r requirements.txt

# 3. Run the Flask application
python app.py

# 4. Open browser
# Go to: http://127.0.0.1:5000
```

---

## 📁 Project Structure

```
Automated-Classroom-Attendance-System/
│
├── app.py                  # Main Flask application
├── requirements.txt        # Python dependencies
├── README.md               # Project documentation
│
├── templates/              # Flask HTML templates
│   ├── index.html
│   └── result.html
│
├── static/                 # CSS, JS files
│
├── models/                 # YOLOv8 & ArcFace model files
│   └── (add .gitignore for large .pt files)
│
├── database/               # SQLite database
│   └── attendance.db
│
├── sample_images/          # Sample classroom images for testing
│
└── docs/                   # Research paper & project report
    ├── Research_Paper.pdf
    └── Project_Report.pdf
```

---

## 🏆 Awards & Recognition

- 🥇 **1st Prize** — Intra College Project Expo 2025, Dr. TTIT, KGF (Nov 19–20, 2025)
- 🏅 **Best Paper Award** — ICRTTEAS 2025-26, 8th International Conference on Recent Trends in Technology, Engineering and Applied Science, Dr. TTIT, KGF (Nov 21–22, 2025)
- 🎖️ **Participant** — Tech Nexus 2025, Inter-College Project Expo, Dr. TTIT

---

## 📄 Research Paper

**Title:** Automated Classroom Attendance System
**Authors:** Jansi Rani J, Akshaya K, Amulya K S, Asfa Hana, Jaya Preethi J
**Conference:** 8th International Conference on Recent Trends in Technology, Engineering and Applied Science (ICRTTEAS 2025-26)
**Institution:** Department of CSE, Dr. T. Thimmaiah Institute of Technology, KGF
**Date:** November 21–22, 2025
**Award:** Best Paper

📎 Full paper available in `docs/Research_Paper.pdf`

---

## 🔮 Future Work

- [ ] Live video stream support for real-time classroom monitoring
- [ ] Liveness detection to prevent spoofing
- [ ] Expanded dataset with diverse lighting, poses, and expressions
- [ ] Continuous video-based attendance tracking during lectures
- [ ] Mobile app interface for easier deployment

---

## 📜 Keywords

`YOLOv8` `ArcFace` `Face Recognition` `Deep Learning` `Computer Vision` `Flask` `Automated Attendance` `Multi-Face Detection` `AI-Based Monitoring` `Smart Attendance System`

---

## 📬 Contact

**Akshaya K** — akshayakristy@gmail.com
[LinkedIn](https://www.linkedin.com/in/akshaya-k-6860203aa) | [GitHub](https://github.com/akshaya-k-06)

---

*Department of Computer Science Engineering, Dr. T. Thimmaiah Institute of Technology, KGF — VTU*
