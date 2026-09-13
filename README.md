# 🔥 FLAMES Game

> **A fun, interactive web-based game to discover the nature of your relationship!**

[![HTML](https://img.shields.io/badge/HTML-100%25-orange?style=flat-square&logo=html5)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)](LICENSE)
[![GitHub](https://img.shields.io/badge/GitHub-mkashinath13-blue?style=flat-square&logo=github)](https://github.com/mkashinath13)

---

## 📋 Table of Contents

- [About](#-about)
- [Features](#-features)
- [How to Play](#-how-to-play)
- [Game Results](#-game-results)
- [Getting Started](#-getting-started)
- [Technical Details](#-technical-details)
- [Live Demo](#-live-demo)

---

## 🎮 About

FLAMES is a classic game that predicts the nature of a relationship between two people. The game uses a simple algorithm based on the names of two individuals to reveal whether they are:
- **Friends**
- **Love** 💕
- **Affection** 💕
- **Marriage** 💍
- **Enemy** ⚔️
- **Siblings** 👥

This interactive HTML5 version features a modern UI with a **scratchable card** mechanic—scratch off the gray overlay to reveal the result!

---

## ✨ Features

### 🎨 Modern User Interface
- **Dark theme** with sleek design
- **Responsive layout** that works on desktop and mobile devices
- **Google Fonts** integration (League Spartan & Oswald)
- **Smooth animations** and transitions

### 🎯 Interactive Scratch-Off Card
- Beautiful **yellow-green (#a4dc50)** scratch card
- Smooth scratchable overlay with visual feedback
- Reveals the result image when 45% of the card is scratched
- Works on both **mouse and touch devices**

### 🔊 Immersive Experience
- **Sound effects** when the result is revealed
- **Inspirational quotes** displayed for each relationship type
- Instant visual feedback

### 📱 Mobile-Friendly
- Touch-enabled scratch functionality
- Responsive design for all screen sizes
- Optimized for both portrait and landscape modes

---

## 🎲 How to Play

### Step 1: Enter Names
1. Open the FLAMES Game application
2. Enter **your name** in the first input field
3. Enter your **crush's name** (or friend's name) in the second field

### Step 2: Click CHECK
- Click the green **"CHECK"** button to calculate the relationship type
- A gray scratch card will appear on the right side

### Step 3: Scratch to Reveal
- **Mouse**: Click and drag across the gray card to scratch it away
- **Touch**: Swipe your finger across the card on mobile devices
- Continue scratching until 45% of the card is revealed

### Step 4: Discover the Result
- The relationship result will be revealed with a beautiful image
- An inspirational quote related to your result will appear
- A sound effect will play to celebrate your discovery!

### Step 5: Try Again
- Click the **"↻ Refresh"** button in the bottom-right to start over
- Enter new names and discover different relationship outcomes

---

## 🎁 Game Results

Each result comes with its own unique image and inspirational quote:

| Result | Meaning | Quote |
|--------|---------|-------|
| **Friends** | You are best friends! | *"A true friend sees the tears behind your smile."* |
| **Love** | You are in love! ❤️ | *"Love is not about possession, it's about appreciation."* |
| **Affection** | You have affection for each other | *"Affection is the heartbeat of any relationship."* |
| **Marriage** | You are destined to marry! 💍 | *"A great marriage is not when perfect people come together, but when imperfect people learn to enjoy their differences."* |
| **Enemy** | You are enemies | *"Even an enemy teaches you strength you never knew you had."* |
| **Siblings** | You are like siblings | *"Siblings: your first friend, your forever rival."* |

---

## 🚀 Getting Started

### Option 1: Play Online
Visit the live demo: [FLAMES Game Live](https://mkashinath13.github.io/flames-game/)

### Option 2: Run Locally

```bash
# Clone the repository
git clone https://github.com/mkashinath13/flames-game.git

# Navigate to the directory
cd flames-game

# Open in your browser (choose one)
# Using Python 3
python -m http.server 8000

# Using Python 2
python -m SimpleHTTPServer 8000

# Or simply double-click index.html
```

Then open your browser and navigate to `http://localhost:8000`

---

## 🔧 Technical Details

### Project Structure
```
flames-game/
├── index.html              # Main application file
├── static/
│   ├── images/
│   │   └── logo.png       # Top-left logo
│   ├── results/
│   │   ├── friends.png
│   │   ├── love.png
│   │   ├── affection.png
│   │   ├── marriage.png
│   │   ├── enemy.png
│   │   └── siblings.png
│   └── sounds/
│       └── reveal.mp3     # Reveal sound effect
└── README.md
```

### Algorithm

The FLAMES algorithm works as follows:

1. **Remove Common Letters**: Remove all common letters between the two names
2. **Count Remaining Letters**: Sum the remaining letters from both names
3. **Apply FLAMES Formula**: Use the count to determine the relationship type through elimination

```javascript
// Simplified algorithm flow:
1. name1 = "john", name2 = "jane"
2. Remove common: n, a, e → "joh" and "j"
3. Total = 4 letters
4. Apply to ['friends', 'love', 'affection', 'marriage', 'enemy', 'siblings']
5. Result: One of the six relationship types
```

### Technologies Used

- **HTML5**: Semantic markup and canvas API
- **CSS3**: Modern styling with flexbox and animations
- **Vanilla JavaScript**: No dependencies required
- **Canvas API**: For the scratch-off effect
- **Google Fonts**: Typography
- **Web Audio API**: Sound effects

### Browser Compatibility

| Browser | Support |
|---------|---------|
| Chrome | ✅ Full Support |
| Firefox | ✅ Full Support |
| Safari | ✅ Full Support |
| Edge | ✅ Full Support |
| Mobile Browsers | ✅ Full Support |

---

## 🎬 Demo GIF / Screenshots

### Initial Screen
```
┌─────────────────────────────────────────┐
│  FLAMES LOGO                            │
│                                         │
│  Your Name: [Enter name]                │
│  Crush's Name: [Enter name]             │
│  [CHECK]                    [💛 Card]   │
│                                         │
│                              ↻ Refresh  │
└─────────────────────────────────────────┘
```

### After Scratching
```
┌─────────────────────────────────────────┐
│                                         │
│                          ┌─────────────┐│
│                          │   LOVE 💕   ││
│                          │   IMAGE     ││
│                          │             ││
│                          └─────────────┘│
│  "Love is not about possession..."      │
│                              ↻ Refresh  │
└─────────────────────────────────────────┘
```

---

## 📊 Features Breakdown

### 🎨 UI/UX
- Modern dark theme (#2a2122 background)
- Accent color: Lime Green (#a4dc50)
- Responsive flex layout
- Smooth button transitions

### 🖱️ Interaction
- Real-time scratch detection
- 45% threshold for reveal
- Mouse and touch support
- Smooth canvas clearing

### 🎵 Audio/Visual
- Reveal sound effect plays on completion
- Result images displayed
- Inspirational quotes shown
- Smooth transitions and animations

---

## 🤝 Contributing

Feel free to fork this project and submit pull requests for improvements!

### Ideas for Enhancement
- Add more relationship categories
- Customize themes and colors
- Add more sound effects
- Create personalized result messages
- Add share functionality (Twitter, Instagram)

---

## 📝 License

This project is open source and available under the MIT License.

---

## 👨‍💻 Author

**Kashinath** - [GitHub Profile](https://github.com/mkashinath13)

---

## 🌟 Star this repository if you found it fun and useful!

---

## 🎪 Have Fun!

Try the FLAMES game with your friends and share the results. Remember, it's just for fun! 😄

**[👉 Play the Game Now! 👈](https://mkashinath13.github.io/flames-game/)**

---

*Created with ❤️ by mkashinath13*
