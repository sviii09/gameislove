# 🌟 Catch the Stars Game

A fun browser-based game built with vanilla HTML, CSS, and JavaScript, deployed using Docker and Nginx.

## 🎮 Game Description

Catch falling stars to earn points while avoiding bombs! Test your reflexes as the game gets progressively harder. How high can you score?

### Features
- ⭐ Catch stars to earn +10 points
- 💣 Avoid bombs or lose a life
- ❤️ Start with 3 lives
- 📈 Increasing difficulty as you progress
- 🎨 Colorful and smooth animations
- 🔄 Restart option when game ends

### Controls
- **Arrow Keys** (← →) or **A/D keys** to move left and right
- Move your basket to catch the stars!

## 🚀 Getting Started

### Prerequisites
- [Docker Desktop](https://www.docker.com/products/docker-desktop/) installed and running

### Installation & Running

1. **Clone or download this repository**

2. **Navigate to the project directory**
   ```bash
   cd gameislove
   ```

3. **Build the Docker image**
   ```bash
   docker build -t star-game -f dk.dockerfile .
   ```

4. **Run the container**
   ```bash
   docker run -d -p 8080:80 --name game star-game
   ```

5. **Open your browser and visit**
   ```
   http://localhost:8080
   ```

## 🛠️ Project Structure

```
gameislove/
├── index.html      # Main game file (HTML, CSS, JS)
├── dk.dockerfile   # Docker configuration
└── README.md       # This file
```

## 🐳 Docker Commands

### Stop the container
```bash
docker stop game
```

### Start the container again
```bash
docker start game
```

### Remove the container
```bash
docker rm game
```

### View running containers
```bash
docker ps
```

### View all containers (including stopped)
```bash
docker ps -a
```

### Remove the image
```bash
docker rmi star-game
```

## 🎯 Game Rules

1. Use arrow keys or A/D to move your basket
2. Catch yellow stars to gain points (+10 each)
3. Avoid red bombs - they cost you a life
4. Missing a star also costs you a life
5. Game ends when you run out of lives
6. Try to beat your high score!

## 🔧 Technologies Used

- **HTML5 Canvas** - For game rendering
- **CSS3** - For styling and animations
- **Vanilla JavaScript** - Game logic
- **Docker** - Containerization
- **Nginx Alpine** - Lightweight web server

## 📝 License

This project is open source and available for educational purposes.

## 🤝 Contributing

Feel free to fork this project and make improvements! Some ideas:
- Add sound effects
- Include power-ups
- Add different difficulty levels
- Create a leaderboard
- Add mobile touch controls

## 👨‍💻 Author

Created as a learning project for Docker deployment and game development.

---

Enjoy the game! 🎮✨
