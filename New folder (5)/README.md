# 🎮 Memory Match - Theme of the Day

A modern, accessible memory matching game designed for 6-year-olds, featuring AI-generated daily themes with colorful emoji sets and bubbly animations.

![Memory Match Game](https://img.shields.io/badge/Status-Ready%20to%20Play-brightgreen)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind-38B2AC?logo=tailwind-css&logoColor=white)
![Vanilla JS](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

## ✨ Features

### 🎨 AI-Powered Daily Themes
- **6 Unique Themes**: Magical Forest, Ocean Adventure, Sweet Treats, Space Explorer, Dinosaur Park, Rainbow Friends
- **Dynamic Color Palettes**: Each theme has custom CSS variables for cohesive design
- **Consistent Daily Theme**: Theme rotates based on calendar day

### 🎯 Child-Friendly UX
- **Large Interactive Cards**: Easy to tap/click for small hands
- **High-Contrast Colors**: Ensures visibility and engagement
- **Bubbly Design**: Rounded corners, bouncy animations, playful fonts
- **Positive Reinforcement**: Confetti celebration on win

### ♿ Accessibility First
- **Screen Reader Support**: ARIA labels on every card
- **Keyboard Navigation**: Full game playable with Enter/Space keys
- **Semantic HTML**: Proper roles and tabindex for assistive tech
- **Dynamic Updates**: ARIA labels update as game state changes

### 🔒 Security & Performance
- **Single External Dependency**: Tailwind CSS CDN only
- **No External API Calls**: AI theme generator simulated locally
- **Zero Build Process**: Single HTML file, ready to deploy
- **Vanilla JavaScript**: No frameworks, maximum compatibility

## 🚀 Quick Start

### Play Locally
1. Download `index.html`
2. Double-click to open in any modern browser
3. Start matching!

### Deploy to GitHub Pages
1. Fork this repository
2. Go to Settings → Pages
3. Select `main` branch as source
4. Your game will be live at `https://yourusername.github.io/memory-match`

### Deploy Anywhere
Since this is a single HTML file with no build process:
- **Netlify**: Drag and drop `index.html`
- **Vercel**: Deploy in one click
- **Any Web Server**: Upload and serve

## 🎮 How to Play

1. **Click any card** to reveal the emoji
2. **Click another card** to find its match
3. **Match all 8 pairs** to win!
4. **Track your progress** with the move counter
5. **Click "New Game"** to get a fresh theme

## 🛠️ Technical Details

### Code Architecture
```javascript
// Core Functions
generateAITheme()  // Simulates Gemini 1.5 Flash API
shuffleCards()     // Fisher-Yates shuffle algorithm
checkMatch()       // Match validation logic
celebrateWin()     // Win celebration with confetti
```

### Theme Structure
Each theme includes:
- **Name**: Display title with emoji
- **8 Emojis**: Kid-friendly symbols
- **Color Palette**: Primary, secondary, and gradient colors

### Accessibility Features
- `aria-label` on all interactive elements
- `role="button"` for card elements
- `tabindex="0"` for keyboard focus
- Dynamic ARIA updates on state changes

## 📱 Browser Compatibility

- ✅ Chrome/Edge (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

## 🎨 Customization

### Add New Themes
Edit the `generateAITheme()` function in `index.html`:

```javascript
{
    name: "🌸 Your Theme",
    emojis: ["🎈", "🎁", "🎊", "🎉", "🎀", "🎪", "🎭", "🎨"],
    colors: {
        primary: "#FF1744",
        secondary: "#C51162",
        bgStart: "#FCE4EC",
        bgEnd: "#F8BBD0"
    }
}
```

### Adjust Difficulty
Change the grid size in the HTML:
```html
<!-- Easy: 3x4 grid (6 pairs) -->
<div id="game-board" class="grid grid-cols-3 gap-4">

<!-- Medium: 4x4 grid (8 pairs) - Default -->
<div id="game-board" class="grid grid-cols-4 gap-4">

<!-- Hard: 5x4 grid (10 pairs) -->
<div id="game-board" class="grid grid-cols-5 gap-4">
```

## 📄 License

MIT License - Feel free to use, modify, and distribute!

## 🤝 Contributing

Contributions welcome! Ideas for improvement:
- Add sound effects toggle
- Implement difficulty levels
- Add timer mode
- Create more themes
- Add multiplayer support

## 👨‍💻 Author

Created with ❤️ for young learners everywhere

---

**⭐ Star this repo if you enjoyed the game!**
