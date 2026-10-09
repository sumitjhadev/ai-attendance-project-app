# AI Attendance Project App.

An AI-powered attendance management system that uses facial recognition to automatically mark and track attendance, eliminating the need for manual roll calls or biometric hardware.

---

## 📌 Overview

- Traditional attendance systems (manual roll call, ID cards, fingerprint scanners) are slow, error-prone, and easy to manipulate (proxy attendance).
- This project uses **computer vision and facial recognition** to detect and identify individuals in real time via a webcam, then automatically logs their attendance with a timestamp.
- Built as part of the **Apna College Prime AI/ML Course** capstone project.

---

## ✨ Features

- Real-time face detection and recognition using a webcam feed
- Automatic attendance marking with date and time stamps
- Prevents duplicate attendance entries for the same session
- Simple Flask-based web interface to interact with the system
- Stores attendance records for easy tracking and export
- Lightweight and easy to set up locally

---

## 🛠️ Tech Stack

| Component        | Technology            |
|-------------------|------------------------|
| Backend           | Python, Flask          |
| Face Detection/Recognition | OpenCV, face-recognition library |
| Data Storage      | CSV / local file storage |
| Frontend          | HTML, CSS (via Flask templates) |

---

## 📂 Project Structure

```
ai-attendance-project-app/
│
├── src/                  # Core application logic and helper modules
├── app.py                # Main Flask application entry point
├── requirements.txt      # Python dependencies
└── README.md             # Project documentation
```

---

## ⚙️ Installation & Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/sumitjhadev/ai-attendance-project-app.git
   cd ai-attendance-project-app
   ```

2. **Create a virtual environment (recommended)**
   ```bash
   python -m venv venv
   venv\Scripts\activate       # Windows
   source venv/bin/activate    # macOS/Linux
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Run the application**
   ```bash
   python app.py
   ```

5. **Open in browser**
   ```
   http://127.0.0.1:5000
   ```

---

## ▶️ How It Works

1. User faces are registered/enrolled into the system beforehand.
2. When the webcam feed detects a face, it compares it against the stored/known faces.
3. If a match is found, the system marks that person as "present" along with the current timestamp.
4. Attendance data is saved and can be reviewed or exported.

---

## 🚀 Future Improvements

- Add a proper database (SQLite/MongoDB) instead of flat-file storage
- Add admin authentication and role-based access
- Export attendance reports as PDF/Excel
- Deploy the app with a public-facing landing page (see companion repo: [ai-attendance-project-landing](https://github.com/sumitjhadev/ai-attendance-project-landing))
- Improve recognition accuracy in low-light conditions

---

## 🙌 Acknowledgements

Built as part of the **Apna College Prime AI/ML Course**.

---

## 📄 License

This project is for educational purposes as part of a course capstone project.

