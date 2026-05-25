* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
  font-family: system-ui, sans-serif;
}

body {
  background: radial-gradient(circle at top, #ffdde1, #ee9ca7);
  min-height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
}

.container {
  background: rgba(255, 255, 255, 0.9);
  padding: 40px 30px;
  border-radius: 20px;
  box-shadow: 0 20px 40px rgba(0,0,0,0.15);
  max-width: 420px;
  width: 100%;
  text-align: center;
  position: relative;
}

.step {
  display: none;
  opacity: 0;
  transform: translateY(20px);
  transition: 0.4s ease;
}

.step.active {
  display: block;
  opacity: 1;
  transform: translateY(0);
}

h1 {
  margin-bottom: 25px;
}

.buttons {
  display: flex;
  justify-content: center;
  gap: 20px;
}

.btn {
  padding: 12px 24px;
  border-radius: 999px;
  border: none;
  cursor: pointer;
  font-size: 18px;
  transition: 0.2s ease;
}

.btn:active {
  transform: scale(0.96);
}

.yes {
  background: #ff4b5c;
  color: white;
}

.no {
  background: white;
  color: #ff4b5c;
  border: 2px solid #ff4b5c;
  position: relative;
  transition: transform 0.1s linear;
}

.options {
  display: flex;
  flex-direction: column;
  gap: 10px;
  text-align: left;
  margin-bottom: 20px;
}

.options label {
  background: #ffeef2;
  padding: 8px 12px;
  border-radius: 10px;
  cursor: pointer;
}

.next, .send {
  background: #ff4b5c;
  color: white;
}

.note {
  margin-top: 10px;
  font-size: 13px;
  color: #666;
}

.hidden {
  display: none;
}
