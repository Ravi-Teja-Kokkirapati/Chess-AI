# Chess-AI

I have built a deep learning-based chess AI that you can play against, featuring a PyGame GUI, models trained on Lichess data, and a clean, modular Python codebase for experimentation and learning.

## Features

✅ Play chess against a neural network-based AI locally  
✅ PyGame-powered intuitive GUI  
✅ Models trained on large-scale Lichess database  
✅ Modular and easy-to-understand Python implementation  
✅ Suitable for learning AI + game development fundamentals

## Getting Started

### 1️⃣ Clone the repository
```bash
git clone https://github.com/YOUR_USERNAME/chess-ai.git
cd chess-ai
```

### 2️⃣ Set up your environment
Create and activate a virtual environment:
```bash
python -m venv .
# Windows
Scripts\activate
# Mac/Linux
source bin/activate
```

### 3️⃣ Install dependencies
```bash
python -m pip install -r requirements.txt
```

### 4️⃣ Launch the game
```bash
cd gui
python main.py
```

Enjoy playing against your AI!

---

## How It Works

### Data
- Uses the official **Lichess PGN database** for training.
- Processing steps:
  - Convert PGN to FEN for each move.
  - Extract “from” and “to” squares.
  - Prepare training samples for the model.

### Model
The chess AI uses **two deep learning models**:
- **From-model:** Predicts the square to move from.
- **To-model:** Predicts the square to move to.

For each legal move:
```
Score = P(from_square) * P(to_square)
```
The move with the highest score is executed.

**Architecture:**
- 6 convolutional layers
- 2 dense layers + output
- Softmax outputs over an 8x8 matrix
- Trained using TensorFlow/Keras

---

## GUI

Built using **PyGame** and **python-chess** for an interactive chess-playing experience.

---

## Why This Project

I am passionate about chess and AI, and this project combines both while reinforcing my skills in:
- Deep learning model design
- Data preprocessing
- Game development
- Clean, scalable Python coding practices

---

## Contributing

Pull requests and suggestions are welcome for:
- Improving model performance
- Adding new training pipelines
- Enhancing GUI features

---


## Contact

For questions or discussions, reach out via:
- GitHub Issues
- kokkirpatiraviteja@gmail.com 

---
