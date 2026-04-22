🧠 Quiz App

A fun and interactive quiz application that tests your general knowledge with multiple choice questions.

## ✨ Features

- 🎯 **Multiple Choice Questions** - 4 answer options per question
- ✅ **Instant Feedback** - Know immediately if your answer is correct
- 📊 **Score Tracking** - Track your score throughout the quiz
- 🔄 **Auto Progress** - Automatically moves to next question
- 🏆 **Final Score** - Shows your total score at the end
- 📱 **Responsive Design** - Works on all screen sizes
 🛠️ Technologies Used

- **HTML5** - Structure
- **CSS3** - Styling with transitions and hover effects
- **JavaScript (ES6)** - Quiz logic and DOM manipulation

## ⚙️ Installation & Setup

1. **Clone the repository**
```bash
git clone https://github.com/karnemanideep/quiz-app.git
cd quiz-app
```

2. **Run the app**
   - Simply open `index.html` in your browser
   - No installation needed!

## 📁 Project Structure

```
quiz-app/
│
├── index.html
├── style.css
├── script.js
└── README.md
```

## 🎯 How It Works

1. **Start Quiz** - Quiz starts automatically on page load
2. **Read Question** - Each question is displayed with 4 options
3. **Select Answer** - Click any answer button to submit
4. **Score Update** - Score updates automatically for correct answers
5. **Next Question** - Moves to next question automatically
6. **Final Score** - Shows total score after all questions

## 📝 Questions Included

```
1. Which is the largest animal in the world?
   → Blue Whale ✅

2. Which is the smallest country in the world?
   → Vatican City ✅

3. Which is the largest desert in the world?
   → Sahara ✅

4. Which is the smallest continent in the world?
   → Australia ✅
```

## 🎨 Key Implementation Details

### Dynamic Question Rendering
```javascript
function showQuestion() {
    let currentQuestion = questions[currentQuestionIndex];
    questionElement.innerHTML = questionNo + ". " + currentQuestion.question;
    currentQuestion.answers.forEach(answer => {
        const button = document.createElement("button");
        button.innerText = answer.text;
        qanswerButton.appendChild(button);
    });
}
```

### Score Tracking
```javascript
function selectAnswer(e) {
    const correct = selectedButton.dataset.correct === 'true';
    if (correct) {
        score++;
    }
}
```

## 🚀 Future Improvements

- [ ] Add more questions
- [ ] Add timer for each question
- [ ] Add difficulty levels (Easy, Medium, Hard)
- [ ] Add question categories
- [ ] Add animations for correct/wrong answers
- [ ] Add high score leaderboard
- [ ] Add restart button after quiz ends
- [ ] Shuffle questions randomly

## 👨‍💻 Author

**Manideep Karne**
- GitHub: [@karnemanideep](https://github.com/karnemanideep)

## 🙏 Acknowledgments

- Built with ❤️ using vanilla JavaScript
- Questions based on general knowledge

---

⭐ **Star this repo** if you found it helpful!
```
