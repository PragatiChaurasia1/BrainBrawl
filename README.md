# 🧠 Trivia Quiz Master

A modern, responsive trivia quiz application built with vanilla JavaScript, HTML5, and CSS3. Test your knowledge across multiple categories with varying difficulty levels!

## 🌟 Features

- **Multiple Categories**: General Knowledge, Science & Nature, History, Sports, Entertainment, Geography
- **Three Difficulty Levels**: Easy, Medium, Hard
- **Interactive Timer**: 30-second countdown per question
- **Real-time Scoring**: Live score tracking and progress visualization
- **Responsive Design**: Optimized for desktop, tablet, and mobile devices
- **Modern UI/UX**: Clean, intuitive interface with smooth animations
- **Detailed Results**: Comprehensive performance analytics and statistics

## 🚀 Live Demo

[View Live Demo](https://PragatiChaurasia1.github.io/trivia-quiz-master)

## 🛠️ Technologies Used

- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **Styling**: CSS Grid, Flexbox, CSS Animations
- **Design**: Responsive Web Design, Mobile-First Approach
- **Architecture**: Object-Oriented Programming, Modular Code Structure

## ⚡ Quick Start

1. **Clone the repository**
   ```bash
   git clone https://github.com/PragatiChaurasia1/trivia-quiz-master.git
   ```

2. **Navigate to project directory**
   ```bash
   cd trivia-quiz-master
   ```

3. **Open in browser**
   ```bash
   # Simply open index.html in your browser
   # Or use Live Server extension in VS Code
   ```

4. **Start quizzing!**
   - Choose your category and difficulty level
   - Answer questions within the time limit
   - View your results and try again!

## 📁 Project Structure

```
trivia-quiz-master/
│
├── index.html              # Main HTML file
├── assets/
│   └── screenshots/        # App screenshots
├── README.md              # Project documentation
├── LICENSE                # MIT License
└── .gitignore            # Git ignore file
```

## 🎮 How to Play

1. **Select Category**: Choose from 6 different knowledge categories
2. **Pick Difficulty**: Select Easy, Medium, or Hard difficulty level
3. **Answer Questions**: You have 30 seconds per question
4. **View Results**: See detailed performance analytics
5. **Play Again**: Try different categories and difficulties

## 🔧 Code Highlights

### Object-Oriented Architecture
```javascript
class TriviaQuiz {
    constructor() {
        this.currentQuestion = 0;
        this.score = 0;
        this.questions = [];
        this.selectedCategory = 'general';
        this.selectedDifficulty = 'medium';
        // ... initialization code
    }
}
```

### Dynamic Question Loading
```javascript
loadQuestions() {
    const categoryQuestions = this.questionDatabase[this.selectedCategory];
    const difficultyQuestions = categoryQuestions[this.selectedDifficulty];
    this.questions = this.shuffleArray([...difficultyQuestions]).slice(0, 10);
}
```

### Timer Management
```javascript
startTimer() {
    this.timeLeft = 30;
    this.timer = setInterval(() => {
        this.timeLeft--;
        if (this.timeLeft <= 0) {
            this.selectAnswer(-1); // Auto timeout
        }
    }, 1000);
}
```

## 📊 Performance Features

- **Responsive Design**: Adapts to all screen sizes
- **Fast Loading**: Lightweight vanilla JavaScript implementation
- **Smooth Animations**: CSS transitions and transforms
- **Intuitive UX**: Clear visual feedback and navigation

## 🌟 Future Enhancements

- [ ] Integration with Open Trivia Database API
- [ ] User authentication and profile system
- [ ] Global leaderboards and rankings
- [ ] Social media sharing functionality
- [ ] Progressive Web App (PWA) features
- [ ] Multiplayer quiz battles
- [ ] Custom quiz creation tools
- [ ] Advanced analytics and insights

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 📧 Contact

Your Name - [pragativns2308@gmail.com](mailto:pragativns2308@gmail.com)

Project Link: [https://github.com/PragatiChaurasia1/trivia-quiz-master](https://github.com/PragatiChaurasia1/trivia-quiz-master)

## 🙏 Acknowledgments

- Design inspiration from modern quiz applications
- Question categories inspired by popular trivia games
- CSS animations and effects from contemporary web design trends

---

⭐ **Star this repository if you found it helpful!**