# Chess-AI

A deep learning-based chess AI that you can play against, featuring a PyGame GUI, a clean modular codebase, and models trained on the Lichess database.

---

## 📂 Project Structure

```
chess-ai/
│
├── data_cleaning/
│   ├── extract_fen.py
│   ├── get_moves.py
│   └── README.md
│
├── gui/
│   ├── draw.py
│   ├── globals.py
│   ├── main.py         # Entry point for playing the game
│   ├── players.py
│   ├── test.py
│   └── images/, models/
│
├── train/
│   ├── model_parts.py
│   ├── model.py
│   ├── save_weights.py
│   ├── test.py
│   └── logs/
│
├── .venv/
└── .idea/
```

---

## 🚀 Features

✅ Play chess against an AI locally via GUI  
✅ Models trained on Lichess PGN data  
✅ Clean, modular Python for learning and experimentation  
✅ Uses TensorFlow/Keras, PyGame, and python-chess

---

## 🎮 Running the Game

### 1️⃣ Clone the repository
```bash
git clone https://github.com/YOUR_USERNAME/chess-ai.git
cd chess-ai
```

### 2️⃣ Create and activate a virtual environment
```bash
python -m venv .venv
# Windows:
.venv\Scripts\activate
# Mac/Linux:
source .venv/bin/activate
```

### 3️⃣ Install dependencies
```bash
pip install -r requirements.txt
```

### 4️⃣ Run the game
```bash
cd gui
python main.py
```

---

## 🛠️ How It Works

### 📑 Data
- Uses Lichess PGN database for real-game data.
- `data_cleaning/` scripts convert PGN to FEN and extract move pairs for training.

### 🧠 Model
- Two deep learning models:
  - **From-model:** predicts the source square.
  - **To-model:** predicts the destination square.
- For each legal move:
  ```
  Score = P(from_square) * P(to_square)
  ```
  The move with the highest score is executed.

### 🎨 GUI
- Built using **PyGame** and **python-chess**.
- Simple, clean interface to play against your AI.

---

## ✏️ Future Improvements

✅ Add difficulty levels by adjusting model thresholds  
✅ Support for custom board setups  
✅ Online multiplayer with AI move suggestions  
✅ Visual move explanations using heatmaps

---

## 🤝 Contributing

Pull requests are welcome for:
- Improving model accuracy
- Optimizing training scripts
- Enhancing GUI features
- Adding testing scripts

---

## 📧 Contact

For discussions, improvements, or collaborations:
- GitHub Issues
- kokkirapatiraviteja@gmail.com

---

Enjoy playing chess while learning deep learning fundamentals!
