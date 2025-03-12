# 🎬 Movie Watchlist & Review Manager

## 📌 Project Overview
The **Movie Watchlist & Review Manager** is a command-line application that allows users to:
- Add movies to a watchlist
- Mark movies as watched and rate them
- Write and edit reviews for movies
- Get recommendations based on genre
- Manage users in the system

Built using **Python, SQLAlchemy, SQLite, and Click**, this CLI-based app helps users efficiently track their movie-watching experience.

---

## 🚀 Features
✅ **User Management** – Add and list users.  
✅ **Movie Management** – Add, list, and update movies.  
✅ **Review System** – Write, edit, and list movie reviews.  
✅ **Movie Recommendations** – Get suggestions based on genre.  
✅ **Watched Movies Tracking** – Mark movies as watched and rate them.  

---

## 🛠 Technologies Used
- **Python 3**
- **SQLAlchemy ORM**
- **SQLite** (Database)
- **Click** (Command-line interface)
- **Alembic** (Database migrations)

---

## 🔧 Installation & Setup
1. **Clone the repository:**
   ```sh
   git clone https://github.com/Calvince22/movie-recommendation-system
   cd movie-recommendation-system
   ```
2. **Set up a virtual environment:**
   ```bash
   python -m venv env
   source env/bin/activate  
   ```
3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```
4. **Run database migrations:**
   ```bash
   alembic upgrade head
   ```
---

## 🎯 Usage
Run the CLI tool using:
```bash
python main.py
```
You'll be presented with a **menu**, where you can choose actions like adding movies, writing reviews, and getting recommendations.

---

## 📜 CLI Commands
### 1️⃣ Add a User
```bash
python main.py add-user
```
### 2️⃣ Add a Movie
```bash
python main.py add-movie
```
### 3️⃣ List Movies
```bash
python main.py list-movies
```
### 4️⃣ Mark Movie as Watched
```bash
python main.py mark-watched --title "Inception"
```
### 5️⃣ Write/Edit Review
```bash
python main.py write-review --title "Inception" --text "Amazing movie!" --rating 5 --user_id 1
```
### 6️⃣ Recommend a Movie by Genre
```bash
python main.py recommend-movie --genre "Sci-Fi"
```

---

## 📌 Database Schema
- **User** (id, name, email)
- **Movie** (id, title, genre, release_year, watched, rating)
- **Review** (id, user_id, movie_id, review_text, rating)
- **Recommendation** (id, movie_id, genre)

---

## 🛠 Future Enhancements
🚀 Add authentication for users.  
🚀 Improve recommendation algorithm.  
🚀 Implement a web interface.  

---

## 📄 License
This project is licensed under the **MIT License**.

---

## 💡 Contributing
Pull requests are welcome! Feel free to open an issue if you find a bug or want to suggest an enhancement.

---
