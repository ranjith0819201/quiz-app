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
