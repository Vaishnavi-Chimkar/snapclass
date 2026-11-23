# 🎓 SnapClass – AI-Powered Smart Attendance System

<p align="center">
  <b>Smart Attendance Management Using Face Recognition & Voice Recognition</b>
</p>

<p align="center">
  <a href="https://snapclass-main-vaishnavi.streamlit.app/">
    <img src="https://img.shields.io/badge/Live-Demo-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white" alt="Live Demo">
  </a>
  <a href="https://github.com/Vaishnavi-Chimkar/snapclass">
    <img src="https://img.shields.io/badge/GitHub-Repository-black?style=for-the-badge&logo=github" alt="GitHub">
  </a>
</p>

---

## 📌 About the Project

**SnapClass** is an AI-powered smart attendance management system designed to simplify and automate the traditional classroom attendance process using **Face Recognition and Voice Recognition**.

The system provides dedicated interfaces for teachers and students, allowing teachers to manage subjects, enroll students, and record attendance through AI-powered recognition.

Instead of manually taking attendance, teachers can identify students using facial or voice recognition, making classroom attendance faster, easier, and more efficient.

SnapClass combines Artificial Intelligence, Machine Learning, and cloud database integration to deliver a smarter attendance management experience.

## ✨ Key Features

### 👨‍🏫 1. Teacher Module
- Teacher login and authentication.
- Create and manage classroom subjects.
- Add and enroll students.
- Generate and share classroom joining links.
- Manage student enrollment.
- Mark attendance using face and voice recognition.
- View attendance results.

### 👨‍🎓 2. Student Module
- Student login and authentication.
- Join classrooms using unique joining codes.
- Enroll in subjects through shared links.
- Access the student interface.

### 🤖 3. AI-Based Face Recognition
- Capture student photographs.
- Process facial images.
- Extract facial features.
- Identify registered students through the face recognition pipeline.
- Support automated attendance workflows.

### 🎤 4. Voice Recognition
- Capture student voice input.
- Process voice recordings.
- Extract voice features.
- Identify registered speakers using the voice recognition pipeline.
- Support voice-based attendance.

### 📊 5. Attendance Management
- Face-based attendance.
- Voice-based attendance.
- Automated attendance workflow.
- Attendance result management.

### 📱 6. QR Code Integration
- Generate QR codes for classroom joining.
- Share subject enrollment links.
- Simplify student enrollment.

### 🔐 7. Database & Security
- Supabase cloud database integration.
- Secure password hashing.
- Teacher and student authentication.
- Session management.
- Centralized database operations.

---

## 🛠️ Technology Stack

| Technology | Application |
|---|---|
| Python | Core programming language |
| Streamlit | Web application interface |
| OpenCV | Image processing |
| Dlib | Facial feature processing |
| Face Recognition | Facial identification |
| Scikit-learn | Machine learning |
| Resemblyzer | Voice feature extraction |
| NumPy | Numerical computations |
| Pandas | Data management |
| Supabase | Cloud database |
| bcrypt | Password hashing |
| Segno | QR code generation |
| Pillow | Image processing |

---

## 🏗️ Project Architecture

SnapClass follows a modular architecture that separates user interfaces, reusable components, database operations, and AI recognition pipelines.

```text
snapclass/
│
├── .devcontainer/
│
├── .streamlit/
│   ├── config.toml
│   └── secrets.toml
│
├── src/
│   │
│   ├── components/
│   │   ├── dialog_add_photo.py
│   │   ├── dialog_attendance_results.py
│   │   ├── dialog_auto_enroll.py
│   │   ├── dialog_create_subject.py
│   │   ├── dialog_enroll.py
│   │   ├── dialog_share_subject.py
│   │   ├── dialog_voice_attendance.py
│   │   ├── footer.py
│   │   ├── header.py
│   │   └── subject_card.py
│   │
│   ├── database/
│   │   ├── config.py
│   │   └── db.py
│   │
│   ├── pipeline/
│   │   ├── face_pipeline.py
│   │   └── voice_pipeline.py
│   │
│   ├── screens/
│   │   ├── home_screen.py
│   │   ├── student_screen.py
│   │   └── teacher_screen.py
│   │
│   └── ui/
│       └── base_layout.py
│
├── .gitignore
├── app.py
├── requirements.txt
└── README.md
```

### 📂 Folder Description

| Folder/File | Description |
|---|---|
| `app.py` | Main application entry point |
| `components/` | Reusable UI components, dialogs, enrollment and attendance features |
| `database/` | Database configuration and operations |
| `pipeline/` | Face and voice recognition processing |
| `screens/` | Home, teacher and student interfaces |
| `ui/` | Shared UI layout components |
| `.streamlit/` | Streamlit configuration and local secrets |
| `requirements.txt` | Required Python dependencies |

---

## ⚙️ How SnapClass Works

The application follows these steps:

1. **User Authentication:** Teachers and students log in through their respective interfaces.
2. **Subject Creation:** Teachers create subjects and generate classroom joining links or QR codes.
3. **Student Enrollment:** Students join the classroom using the shared joining mechanism.
4. **Recognition:** The system processes facial images or voice input using the respective recognition pipeline.
5. **Student Identification:** The system compares extracted features with registered student data.
6. **Attendance Management:** Teachers use the recognition results to manage and record student attendance.

---

## 🚀 Installation & Setup

Follow these steps to run SnapClass on your local machine.

### Step 1: Clone the Repository

```bash
git clone https://github.com/Vaishnavi-Chimkar/snapclass.git
```

### Step 2: Navigate to the Project Directory

```bash
cd snapclass
```

### Step 3: Create a Virtual Environment

```bash
python -m venv venv
```

### Step 4: Activate the Virtual Environment

For Windows:

```bash
venv\Scripts\activate
```

### Step 5: Install Dependencies

```bash
pip install -r requirements.txt
```

### Step 6: Configure Supabase

Create a Supabase project and configure your database credentials.

Create a `.streamlit/secrets.toml` file:

```toml
supabase_url = "YOUR_SUPABASE_URL"
supabase_key = "YOUR_SUPABASE_KEY"
```

Replace the placeholder values with your actual Supabase credentials.

**Important:** Never upload your actual credentials or secret keys to GitHub.

### Step 7: Run the Application

```bash
streamlit run app.py
```

Open your browser and visit:

```text
http://localhost:8501
```

---

## 🎯 Project Objectives

- Automate traditional classroom attendance using Artificial Intelligence.
- Implement face and voice recognition for student identification.
- Reduce manual attendance-taking efforts.
- Improve classroom attendance management.
- Simplify student enrollment using QR codes and joining links.
- Apply Machine Learning concepts to solve a real-world educational problem.

---

## 🔮 Future Enhancements

- Attendance analytics and graphical visualizations.
- Export attendance reports in PDF and Excel formats.
- Integration with college management systems.
- Improved recognition accuracy under different lighting and background noise conditions.
- Real-time attendance monitoring.
- Advanced attendance statistics and insights.

---

## 🌐 Live Demo

Experience SnapClass here:

<p align="center">
  <a href="https://snapclass-main-vaishnavi.streamlit.app/">
    <img src="https://img.shields.io/badge/🚀_Launch_SnapClass-Live_Application-5865F2?style=for-the-badge" alt="Launch SnapClass">
  </a>
</p>

**Live Application:** https://snapclass-main-vaishnavi.streamlit.app/

---

## 👩‍💻 Developer

**Vaishnavi Chimkar**

- GitHub: https://github.com/Vaishnavi-Chimkar
- LinkedIn: https://www.linkedin.com/in/vaishnavi-chimkar-349390328/

---

## ⭐ Show Your Support

If you like this project, please consider giving the repository a ⭐ on GitHub.

Your support motivates further development!

<p align="center">
  <b>SnapClass – Making Classroom Attendance Smarter with AI! 🚀</b>
</p>
