<div align="center">
  <img src="https://img.icons8.com/color/150/000000/music.png" alt="Django Music App Logo"/>
  <h1>🎵 Django Music Player 🎵</h1>
  <p><em>A beautiful, responsive, and dynamic music player application built with Django and JavaScript.</em></p>
  
  [![Django](https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white)](https://www.djangoproject.com/)
  [![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
  [![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
  [![SQLite](https://img.shields.io/badge/SQLite-07405E?style=for-the-badge&logo=sqlite&logoColor=white)](https://www.sqlite.org/)
</div>

<hr/>

## 🌟 Overview

The **Django Music Player** is a full-stack web application designed to give users a seamless audio streaming experience. It boasts a sleek, modern interface with synchronized real-time lyrics, allowing you to enjoy your favorite tracks while following along with the words. 

Whether you're uploading local MP3 files or linking external audio URLs, this app handles it gracefully.

---

## ✨ Key Features

- **🎧 Audio Playback:** High-quality music streaming right in your browser.
- **🖼️ Rich Media Support:** Dynamic album cover art and artist information display.
- **🎤 Synchronized Lyrics:** Real-time lyric tracking that syncs perfectly with the playing track (powered by JavaScript & JSON).
- **⏭️ Track Navigation:** Simple and intuitive pagination to skip to the next or previous track.
- **📁 Dual Audio Sources:** Support for both uploaded audio files and direct audio links.
- **📱 Responsive UI:** Styled elegantly with custom CSS and media queries for a great experience on any device.

---

## 🛠️ Tech Stack

### Backend
- **Framework:** [Django](https://www.djangoproject.com/) (Python)
- **Database:** SQLite3 (Default, easily scalable to PostgreSQL/MySQL)

### Frontend
- **Structure:** HTML5 Django Templates (`{% include %}`, template tags)
- **Styling:** Custom CSS, Font Awesome Icons, Google Fonts (Sofia)
- **Interactivity:** Vanilla JavaScript, jQuery, MediaElement.js

---

## 🚀 Getting Started

Follow these steps to get a local copy up and running.

### Prerequisites

Ensure you have Python installed on your system.
```bash
python --version
```

### Installation & Setup

1. **Clone the repository** (if you haven't already):
   ```bash
   git clone <your-repo-url>
   cd "MUSIC APP-- DJANGO"
   ```

2. **Create a Virtual Environment** (Recommended):
   ```bash
   python -m venv .venv
   .\.venv\Scripts\activate  # On Windows
   # source .venv/bin/activate  # On macOS/Linux
   ```

3. **Install Dependencies**:
   ```bash
   pip install django
   ```

4. **Apply Database Migrations**:
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```

5. **Create a Superuser** (To access the Django Admin panel and add songs):
   ```bash
   python manage.py createsuperuser
   ```

6. **Run the Development Server**:
   ```bash
   python manage.py runserver
   ```

7. **Access the App**:
   - Web App: `http://127.0.0.1:8000/`
   - Admin Panel: `http://127.0.0.1:8000/admin/` (Login and add some `Song` objects to get started!)

---

## 📂 Project Structure

```text
📦 MUSIC APP-- DJANGO
 ┣ 📂 App                # Main Django Application
 ┃ ┣ 📂 migrations       # Database migrations
 ┃ ┣ 📂 static           # CSS, JS, and static assets
 ┃ ┣ 📂 templates        # HTML templates (index.html, main.html)
 ┃ ┣ 📜 models.py        # Database schema (Song model)
 ┃ ┣ 📜 views.py         # Business logic & rendering
 ┃ ┗ 📜 urls.py          # App-level routing
 ┣ 📂 MusicPlayer        # Django Project Configuration
 ┃ ┣ 📜 settings.py      # Main project settings
 ┃ ┗ 📜 urls.py          # Global routing
 ┣ 📂 media              # User-uploaded files (images, audio)
 ┣ 📜 manage.py          # Django execution script
 ┗ 📜 README.md          # Project documentation
```

---

## 💡 How It Works (The Lyrics Engine)
The app uses a custom JavaScript engine to synchronize lyrics. The Django backend passes the lyrics as a JSON object into a `data-lyrics` HTML attribute. The frontend script parses this JSON, listens to the native audio element's `timeupdate` event, and dynamically updates the DOM to display the lyric that matches the current timestamp!

---

## 🤝 Contributing
Contributions, issues, and feature requests are welcome! Feel free to check the issues page or submit a pull request.

<div align="center">
  <p>Made with ❤️ using Django and Python</p>
</div>

