:root {
  font-family: Inter, 'Segoe UI', sans-serif;
  line-height: 1.5;
  font-weight: 400;
  color: #e5eefb;
  background: linear-gradient(135deg, #081425 0%, #12263f 100%);
  font-synthesis: none;
  text-rendering: optimizeLegibility;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

* {
  box-sizing: border-box;
}

html, body, #root {
  margin: 0;
  min-height: 100%;
  min-height: 100vh;
}

body {
  min-height: 100vh;
  display: grid;
  place-items: center;
}

button,
input {
  font: inherit;
}

.app-shell {
  width: 100%;
  min-height: 100vh;
  display: grid;
  place-items: center;
  padding: 32px 16px;
}

.panel {
  width: min(100%, 720px);
  background: rgba(15, 23, 42, 0.9);
  border: 1px solid rgba(148, 163, 184, 0.25);
  border-radius: 20px;
  padding: 32px;
  box-shadow: 0 24px 80px rgba(2, 6, 23, 0.45);
}

.header-block {
  margin-bottom: 28px;
}

.eyebrow {
  margin: 0 0 8px;
  color: #7dd3fc;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  font-size: 0.72rem;
  font-weight: 700;
}

h1 {
  margin: 0;
  font-size: clamp(2rem, 4vw, 2.8rem);
  font-weight: 800;
  color: #f8fbff;
}

.folder-form {
  display: grid;
  gap: 22px;
}

.folder-picker {
  display: grid;
  gap: 10px;
  background: rgba(15, 23, 42, 0.8);
  border: 1px solid rgba(148, 163, 184, 0.2);
  border-radius: 14px;
  padding: 16px 18px;
}

.field-label {
  font-weight: 700;
  color: #f8fbff;
}

.picker-row {
  display: flex;
  align-items: center;
  gap: 12px;
  flex-wrap: wrap;
}

.select-button {
  appearance: none;
  border: none;
  border-radius: 10px;
  background: linear-gradient(135deg, #38bdf8, #2563eb);
  color: white;
  font-weight: 700;
  padding: 12px 18px;
  cursor: pointer;
  transition: transform 0.2s ease, box-shadow 0.2s ease;
  box-shadow: 0 10px 22px rgba(37, 99, 235, 0.35);
}

.select-button:hover {
  transform: translateY(-1px);
}

.selected-value {
  color: #dbeafe;
  background: rgba(30, 41, 59, 0.9);
  border: 1px solid rgba(148, 163, 184, 0.22);
  border-radius: 10px;
  padding: 10px 12px;
  min-height: 44px;
  display: inline-flex;
  align-items: center;
  min-width: 220px;
}

.field-hint {
  color: #a5b4cf;
}

.hidden-input {
  display: none;
}

.submit-button {
  margin-top: 10px;
  border: none;
  border-radius: 12px;
  padding: 14px 18px;
  font-weight: 800;
  font-size: 1rem;
  background: linear-gradient(135deg, #22c55e, #16a34a);
  color: #f0fdf4;
  cursor: pointer;
  transition: opacity 0.2s ease, transform 0.2s ease;
}

.submit-button:hover:not(:disabled) {
  transform: translateY(-1px);
}

.submit-button:disabled {
  opacity: 0.5;
  cursor: not-allowed;
}

@media (max-width: 560px) {
  .panel {
    padding: 22px 18px;
  }

  .picker-row {
    display: grid;
  }

  .selected-value {
    width: 100%;
  }
}
