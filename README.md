🔐 Random Password Generator

A simple web app that generates strong, random passwords with one click. Built with HTML, CSS, and JavaScript.



✨ Features
Generates two random passwords at a time to choose from
Uses a mix of uppercase letters, lowercase letters, numbers, and symbols
Adjustable password length (default: 15 characters)
Click a password to copy it to your clipboard
Clean, responsive dark-themed UI
🖥️ How to Use
Click Generate Passwords.
Two random passwords appear on the screen.
Click the one you like to copy it.
Paste it wherever you need it!
🛠️ Built With
HTML5 – structure
CSS3 – styling and layout
JavaScript (ES6) – password logic and DOM manipulation
🚀 Getting Started

No installation or build tools required.

bash
# Clone the repository
git clone https://github.com/sandeepramidi/password-generator.git

# Go into the project folder
cd password-generator

Then open index.html in your browser (or use the VS Code Live Server extension).

📂 Project Structure
password-generator/
├── index.html
├── index.css
├── index.js
└── README.md
⚙️ How It Works

The app keeps an array of all allowed characters (A–Z, a–z, 0–9, and symbols). When you click the button, a loop picks a random character from the array using Math.random() and Math.floor(), repeating until the password reaches the chosen length. The results are then rendered to the page using DOM manipulation.

js
function getRandomCharacter() {
  const index = Math.floor(Math.random() * characters.length)
  return characters[index]
}
🧠 What I Learned
DOM selection and manipulation
Handling events with addEventListener
Working with arrays, loops, and Math.random()
Using the Clipboard API (navigator.clipboard.writeText)
Building responsive layouts with CSS Flexbox
🔮 Future Improvements
Toggle options for numbers and symbols
Length slider
Password strength indicator
"Copied!" toast notification

⚠️ Note: This project is for learning purposes. Math.random() is not cryptographically secure — for real-world use, consider crypto.getRandomValues().

🙏 Acknowledgements

Built as part of the Scrimba course.

👤 Author

Your Name

GitHub: @sandeepramidi
