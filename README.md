# 🎬 Movie Watchlist & Review Manager

A CLI tool to manage a personal movie watchlist, track watched movies, write reviews, and receive recommendations.

## 📌 Features

✅ Add movies to a watchlist
✅ Mark movies as watched
✅ Write and edit reviews
✅ Get movie recommendations based on genre
✅ List movies, reviews, and users
✅ Delete movies and reviews

## 🛠️ Technologies Used
- Python
- SQLAlchemy (ORM)
- SQLite
- Click (CLI framework)

## 📂 Project Structure
```
📦 movie-watchlist-cli
├── models.py         # Database models
├── cli.py            # CLI commands
├── README.md         # Project documentation
├── requirements.txt  # Dependencies
├── alembic/          # Database migrations
└── movie_rcmdn.db    # SQLite database
```

## 🚀 Installation & Setup

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/Calvince22/movie-recommendation-system
cd movie-recommendation-system
```

### 2️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```

### 3️⃣ Initialize the Database
```bash
python -m models
```

## 📜 Usage
Run the CLI using:
```bash
python cli.py [command] [options]
```

### 🎥 Add a Movie
```bash
python cli.py add-movie --title "Inception" --genre "Sci-Fi" --release_year 2010 --watched False
```

### ✅ Mark a Movie as Watched
```bash
python cli.py mark-watched "Inception" --rating 5
```

### 📝 Write/Edit a Review
```bash
python cli.py write-review "Inception" --text "Amazing movie!" --rating 5 --user_id 1
```

### 🎭 Get Recommendations
```bash
python cli.py recommend-movie --genre "Sci-Fi"
```

### 📜 List Movies
```bash
python cli.py list-movies
```

### 🗑️ Delete a Movie
```bash
python cli.py delete-movie "Inception"
```

## 🛠️ Future Enhancements
- Add support for multiple users with authentication
- Implement a web UI for easier access
- Integrate with external movie APIs (e.g., TMDb)

## 📜 License
This project is licensed under the MIT License.

---


