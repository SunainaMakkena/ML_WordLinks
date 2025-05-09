# Word Links: ML-Powered Word Association Game
A dynamic, machine learning-enhanced word puzzle game inspired by the New York Times Connections. This project uses a Ridge Regression model to adjust puzzle difficulty adaptively based on puzzle features and player behavior.

## 🎯 Project Overview
This game presents word association puzzles where players group related words. A machine learning model dynamically predicts the difficulty level of each puzzle based on its content and player data.

Key Features:-

1.ML-driven adaptive difficulty (Easy, Medium, Hard)

2.Interactive web frontend powered by FastAPI

3.Real-time puzzle generation

4.Gameplay adapts to player's skill over time

## 🧠 Machine Learning Model
We used Ridge Regression due to its robustness against multicollinearity. It predicts expected puzzle solve time, which is then mapped to difficulty levels.

Training Features:-

1.connection_complexity (scale of 1–10)

2.word_rarity_value (common to extremely rare)

3.semantic_distance between words

4.num_words in the puzzle

5.Player behavior: time_of_day, hints_used

Over 1000 synthetic puzzles were generated to simulate realistic player scenarios.

## 🕹 Gameplay Flow
1.Puzzle generated with varying complexity

2.Player interacts via a responsive interface

3.ML model predicts expected solve time

4.Puzzle assigned a difficulty level (Easy/Medium/Hard)

5.Game adapts difficulty based on ongoing performance

<img width="818" alt="image" src="https://github.com/user-attachments/assets/901577e1-5924-4cef-bce4-1163ed0b26d0" />

<img width="761" alt="image" src="https://github.com/user-attachments/assets/1d402bde-0ccb-4dab-9263-abdc74ef04b8" />

<img width="785" alt="image" src="https://github.com/user-attachments/assets/2ab49a09-3e1e-42ac-980d-1f936b645d25" />




## 🧩 Puzzle Generation Logic
Puzzles are created using:

  1.Predefined connection types (e.g., synonyms, themes)

  2.Word rarity and semantic analysis to ensure meaningful groupings

## 🧱 System Architecture
1.Frontend: Web-based UI for gameplay

2.Backend: FastAPI server for game logic & ML model inference

3.ML Module: Ridge Regression trained on synthetic data

## ⚙️ Technical Highlights
1.Clean API design for puzzle and gameplay management

2.Scalable ML integration via FastAPI

3.Semantic distance computation using NLP techniques

## 🚧 Challenges
1.Generating semantically meaningful synthetic puzzles

2.Balancing puzzle difficulty using player behavior

3.Ensuring real-time performance with ML integration

## 🚀 Future Enhancements
1.Real user data collection and model retraining

2.Additional puzzle types and themes

3.Leaderboards and social gameplay features

4.UI/UX enhancements based on player feedback
