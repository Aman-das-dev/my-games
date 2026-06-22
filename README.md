# 🎮 Pong Game

A classic Pong game built with **HTML, CSS, and JavaScript**. Play against an intelligent computer AI opponent in this retro-style arcade game!

## 🎯 Game Overview

This is a modern implementation of the classic Pong game with smooth animations, realistic physics, and an AI opponent. Compete to reach 5 points first and claim victory!

## ✨ Features

- 🖱️ **Dual Control Options**: Use arrow keys or mouse to control the left paddle
- 🤖 **Intelligent AI**: Computer opponent with smart paddle movement
- ⚽ **Physics Engine**: Realistic ball bouncing with wall and paddle collision detection
- 🔄 **Ball Spin**: Dynamic ball trajectory based on where it hits the paddles
- 📊 **Live Scoreboard**: Real-time score tracking for both players
- 🎨 **Neon Visuals**: Retro arcade-style graphics with glowing effects
- 🏁 **Game Over Screen**: Victory/defeat screen with play again option
- ⚡ **Smooth Performance**: Optimized game loop using `requestAnimationFrame`

## 🕹️ How to Play

### Controls
- **Arrow Keys (↑↓)** or **W/S** - Move left paddle up and down
- **Mouse Movement** - Alternatively, move your mouse to control the left paddle

### Game Rules
- The game is played on a 1000x600 pixel court
- You control the **left (green) paddle**
- The **computer controls the right (green) paddle**
- The **magenta ball** bounces around the court
- Points are awarded when the ball passes your opponent's paddle
- **First to 5 points wins!**

## 📁 Project Structure

```
my-games/
└── pong.html          # Complete game (HTML, CSS, JavaScript all-in-one)
└── README.md          # This file
```

## 🚀 Getting Started

### Option 1: Play Online
Visit the game directly on GitHub:
```
https://github.com/Aman-das-dev/my-games/blob/main/pong.html
```

### Option 2: Play Locally
1. Clone the repository:
```bash
git clone https://github.com/Aman-das-dev/my-games.git
cd my-games
```

2. Open `pong.html` in your web browser:
```bash
# On macOS
open pong.html

# On Linux
xdg-open pong.html

# On Windows
start pong.html
```

### Option 3: Use GitHub Pages
If you have GitHub Pages enabled on your repository, access it at:
```
https://Aman-das-dev.github.io/my-games/pong.html
```

## 🎮 Game Mechanics

### Ball Physics
- Ball moves continuously across the screen
- Bounces off top and bottom walls
- Reflects off paddles with added spin based on hit position
- Resets to center when a player scores

### Paddle AI
- Computer paddle follows the ball with intelligent movement
- Features a "dead zone" to make gameplay more challenging
- Moves at 80% of player paddle speed for balance

### Collision Detection
- **Wall Collisions**: Ball bounces off top and bottom boundaries
- **Paddle Collisions**: AABB (Axis-Aligned Bounding Box) collision detection
- **Ball Spin**: Hit position on paddle affects ball trajectory

### Scoring System
- 1 point awarded when ball passes opponent's paddle
- First to 5 points wins the game
- Score resets when you play again

## 🎨 Visual Design

- **Background**: Gradient blue (#1e3c72 to #2a5298)
- **Game Court**: Black with white border
- **Center Line**: Dashed white line (classic Pong style)
- **Paddles**: Glowing green (#00ff00) with glow effect
- **Ball**: Glowing magenta (#ff00ff) with glow effect
- **Scoreboard**: Large white text with glow effect
- **Instructions**: Helpful text at bottom of screen

## 🛠️ Technical Stack

- **HTML5**: Game structure and canvas
- **CSS3**: Styling with gradients, shadows, and animations
- **Vanilla JavaScript**: Game logic, physics, and AI

### Key JavaScript Functions

| Function | Purpose |
|----------|---------|
| `updatePlayerPaddle()` | Handles player input from keyboard |
| `updateComputerPaddle()` | AI logic for computer opponent |
| `updateBall()` | Ball movement and physics |
| `checkCollision()` | AABB collision detection |
| `gameLoop()` | Main game loop using requestAnimationFrame |
| `resetBall()` | Resets ball position after scoring |
| `checkGameOver()` | Determines win conditions |
| `endGame()` | Displays game over screen |
| `resetGame()` | Resets all game variables for new game |

## 📊 Game Constants

```javascript
GAME_WIDTH = 1000px
GAME_HEIGHT = 600px
PADDLE_WIDTH = 15px
PADDLE_HEIGHT = 100px
BALL_SIZE = 15px
PADDLE_SPEED = 6px per frame
BALL_SPEED = 5px per frame
MAX_SCORE = 5 points
```

## 🎯 Tips to Win

1. **Position your paddle at the center** when the ball is far away
2. **Anticipate ball movement** based on its angle and speed
3. **Use paddle edges** to add spin and create difficult angles
4. **Stay focused** on the ball's trajectory
5. **Practice timing** your paddle movements for perfect hits

## 🐛 Known Issues

None currently! If you find any bugs, please report them.

## 🔮 Future Enhancements

- [ ] Difficulty levels (Easy, Medium, Hard)
- [ ] Two-player mode (both players on same device)
- [ ] Sound effects and background music
- [ ] Power-ups (faster ball, larger paddle, etc.)
- [ ] High score tracking with localStorage
- [ ] Mobile touch controls
- [ ] Ball speed increases over time
- [ ] Paddle boost mode (temporary speed increase)
- [ ] Game statistics (longest rally, etc.)

## 📝 License

This project is open source and available under the MIT License.

## 👨‍💻 Author

**Aman Das** - [GitHub Profile](https://github.com/Aman-das-dev)

## 🤝 Contributing

Contributions are welcome! Feel free to:
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 💬 Feedback

Have suggestions or found a bug? Please open an issue on the GitHub repository!

---

**Enjoy the game! 🎮 May the best player win!**