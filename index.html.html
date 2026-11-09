<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Web Development Quiz</title>
  <style>
    :root {
      --bg: #f9fafb;
      --card: #ffffff;
      --text: #1f2937;
      --muted: #6b7280;
      --accent: #2563eb;
      --border: #e5e7eb;
      --correct: #15803d;
      --correct-bg: #dcfce7;
      --wrong: #b91c1c;
      --wrong-bg: #fee2e2;
    }

    * { box-sizing: border-box; margin: 0; padding: 0; }

    body {
      font-family: "Segoe UI", Calibri, Arial, sans-serif;
      background: linear-gradient(135deg, #1e3a8a 0%, #2563eb 50%, #7c3aed 100%);
      color: var(--text);
      min-height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
      padding: 1.25rem;
    }

    .quiz {
      background: var(--card);
      border-radius: 16px;
      width: 100%;
      max-width: 620px;
      padding: 2rem;
      box-shadow: 0 20px 50px rgba(0, 0, 0, 0.25);
    }

    .quiz h1 {
      font-size: 1.75rem;
      margin-bottom: 0.25rem;
      color: var(--accent);
    }
    .subtitle { color: var(--muted); font-size: 0.95rem; margin-bottom: 1.5rem; }

    .progress-track {
      background: #eef2ff;
      border-radius: 999px;
      height: 8px;
      overflow: hidden;
      margin-bottom: 0.5rem;
    }

    .progress-fill {
      background: var(--accent);
      height: 100%;
      width: 0%;
      transition: width 0.3s ease;
    }

    .progress-text {
      color: var(--muted);
      font-size: 0.85rem;
      margin-bottom: 1.5rem;
    }

    .question {
      font-size: 1.15rem;
      font-weight: 600;
      margin-bottom: 1.25rem;
    }

    .options {
      display: flex;
      flex-direction: column;
      gap: 0.75rem;
    }

    .option {
      border: 1px solid var(--border);
      border-radius: 8px;
      background: var(--card);
      padding: 0.8rem 1rem;
      text-align: left;
      font-size: 1rem;
      color: var(--text);
      cursor: pointer;
      transition: border-color 0.2s ease, background 0.2s ease;
    }

    .option:hover:not(:disabled) {
      border-color: var(--accent);
      background: #eff6ff;
      transform: translateX(4px);
    }

    .option:disabled { cursor: default; }

    .option.correct { background: var(--correct-bg); border-color: var(--correct); }
    .option.wrong { background: var(--wrong-bg); border-color: var(--wrong); }

    .feedback {
      min-height: 1.5rem;
      margin-top: 1rem;
      font-weight: 600;
    }

    .feedback.correct { color: var(--correct); }
    .feedback.wrong { color: var(--wrong); }

    .btn {
      background: var(--accent);
      color: #fff;
      border: none;
      border-radius: 6px;
      padding: 0.7rem 1.4rem;
      font-size: 1rem;
      font-weight: 600;
      cursor: pointer;
      margin-top: 1rem;
    }

    .btn {
      background: linear-gradient(90deg, #2563eb, #7c3aed);
      box-shadow: 0 4px 12px rgba(37, 99, 235, 0.35);
      transition: transform 0.15s ease, box-shadow 0.15s ease;
    }

    .btn:hover {
      transform: translateY(-2px);
      box-shadow: 0 8px 18px rgba(37, 99, 235, 0.45);
    }
    .btn[hidden] { display: none; }

    .result { text-align: center; }
    .result .score { font-size: 3rem; font-weight: 700; color: var(--accent); margin: 0.5rem 0; }
    .result p { color: var(--muted); margin-bottom: 1rem; }

    @media (max-width: 480px) {
      .quiz { padding: 1.25rem; }
      .quiz h1 { font-size: 1.25rem; }
    }
  </style>
</head>
<body>

  <main class="quiz">
    <h1>Web Development Quiz</h1>
    <p class="subtitle">Test what you know about HTML, CSS, and JavaScript.</p>

    <div id="quizView">
      <div class="progress-track"><div class="progress-fill" id="progressFill"></div></div>
      <p class="progress-text" id="progressText"></p>

      <h2 class="question" id="questionText"></h2>
      <div class="options" id="optionsList"></div>
      <p class="feedback" id="feedback"></p>
      <button class="btn" id="nextBtn" hidden>Next</button>
    </div>

    <div id="resultView" class="result" hidden>
      <h2>Quiz complete</h2>
      <div class="score" id="finalScore"></div>
      <p id="finalMessage"></p>
      <button class="btn" id="restartBtn">Try Again</button>
    </div>
  </main>

  <script>
    // The quiz questions. To add or change questions, edit this array.
    const questions = [
      {
        question: "What does HTML stand for?",
        options: ["Hyper Text Markup Language", "High Tech Modern Language", "Home Tool Markup Language", "Hyperlinks and Text Markup Language"],
        answer: 0
      },
      {
        question: "Which tag is used for the largest heading?",
        options: ["<heading>", "<h6>", "<h1>", "<head>"],
        answer: 2
      },
      {
        question: "Which CSS property changes the text colour?",
        options: ["background-color", "color", "font-style", "text-align"],
        answer: 1
      },
      {
        question: "Which keyword declares a variable in modern JavaScript that cannot be reassigned?",
        options: ["var", "let", "const", "static"],
        answer: 2
      },
      {
        question: "Which CSS layout system arranges items in rows and columns?",
        options: ["Flexbox only", "CSS Grid", "Float", "Position: absolute"],
        answer: 1
      },
      {
        question: "Which JavaScript method selects an element by its id?",
        options: ["document.querySelectorAll()", "document.getElementByName()", "document.getElementById()", "document.findId()"],
        answer: 2
      },
      {
        question: "Which Git command saves staged changes with a message?",
        options: ["git push", "git commit -m", "git add", "git clone"],
        answer: 1
      },
      {
        question: "Which HTML tag is used to link an external stylesheet?",
        options: ["<script>", "<style>", "<link>", "<css>"],
        answer: 2
      }
    ];

    // Keep track of the quiz state.
    let currentIndex = 0;
    let score = 0;
    let answered = false;

    // Get the elements we need from the page.
    const progressFill = document.getElementById("progressFill");
    const progressText = document.getElementById("progressText");
    const questionText = document.getElementById("questionText");
    const optionsList = document.getElementById("optionsList");
    const feedback = document.getElementById("feedback");
    const nextBtn = document.getElementById("nextBtn");
    const quizView = document.getElementById("quizView");
    const resultView = document.getElementById("resultView");
    const finalScore = document.getElementById("finalScore");
    const finalMessage = document.getElementById("finalMessage");
    const restartBtn = document.getElementById("restartBtn");

    // Show the current question and its answer buttons.
    function showQuestion() {
      answered = false;
      const current = questions[currentIndex];

      questionText.textContent = current.question;
      progressText.textContent = `Question ${currentIndex + 1} of ${questions.length}`;
      progressFill.style.width = `${(currentIndex / questions.length) * 100}%`;

      optionsList.innerHTML = "";
      current.options.forEach((text, index) => {
        const button = document.createElement("button");
        button.className = "option";
        button.textContent = text;
        button.addEventListener("click", () => checkAnswer(index));
        optionsList.appendChild(button);
      });

      feedback.textContent = "";
      feedback.className = "feedback";
      nextBtn.hidden = true;
    }

    // Check the chosen answer and highlight right and wrong options.
    function checkAnswer(chosenIndex) {
      if (answered) return;
      answered = true;

      const current = questions[currentIndex];
      const buttons = optionsList.querySelectorAll(".option");

      buttons.forEach(btn => btn.disabled = true);
      buttons[current.answer].classList.add("correct");

      if (chosenIndex === current.answer) {
        score++;
        feedback.textContent = "Correct!";
        feedback.classList.add("correct");
      } else {
        buttons[chosenIndex].classList.add("wrong");
        feedback.textContent = "Not quite. The correct answer is highlighted.";
        feedback.classList.add("wrong");
      }

      nextBtn.hidden = false;
      nextBtn.textContent = currentIndex === questions.length - 1 ? "See Results" : "Next";
    }

    // Move to the next question, or show results at the end.
    function nextQuestion() {
      currentIndex++;
      if (currentIndex < questions.length) {
        showQuestion();
      } else {
        showResults();
      }
    }

    function showResults() {
      progressFill.style.width = "100%";
      quizView.hidden = true;
      resultView.hidden = false;

      finalScore.textContent = `${score} / ${questions.length}`;

      const percent = (score / questions.length) * 100;
      if (percent === 100) {
        finalMessage.textContent = "Perfect score. Excellent work!";
      } else if (percent >= 60) {
        finalMessage.textContent = "Well done. A bit more practice and you'll be ready.";
      } else {
        finalMessage.textContent = "Keep practising. Try again to improve your score.";
      }
    }

    // Reset everything and start again.
    function restartQuiz() {
      currentIndex = 0;
      score = 0;
      resultView.hidden = true;
      quizView.hidden = false;
      showQuestion();
    }

    nextBtn.addEventListener("click", nextQuestion);
    restartBtn.addEventListener("click", restartQuiz);

    // Start the quiz when the page loads.
    showQuestion();
  </script>
</body>
</html>
