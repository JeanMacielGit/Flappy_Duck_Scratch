# Flappy Duck - CS50x 2025

This is my final project for **Week 0 (Scratch)** of Harvard's CS50x. 
It is a survival game where the player controls a duck navigating through 
obstacles with progressive difficulty.

## 🚀 How to Play
* **Space:** Jump.
* **C Key:** Restart the game after Game Over.
* **Goal:** Dodge the pipes! Speed and spawn frequency increase as your score grows.

## ⚙ How to Run the Project
Since this game was built using **Scratch**, the `.sb3` file cannot be opened like a standard executable. To play or view the code:

1. Download the `Flappy Duck - CS50.sb3` file from this repository.
2. Go to the [Scratch Online Editor](https://scratch.mit.edu/projects/editor/).
3. In the top menu, click on **File** -> **Load from your computer**.
4. Select the `Flappy Duck - CS50.sb3` file you just downloaded.
5. Click the **Green Flag** to start!

## 🛠️ Technical Implementation (Engineering Perspective)

1. **State Management:** I implemented a global variable `game_running` to control the game's flow. This allows the game to "freeze" upon collision, providing visual feedback to the player (UX) without stopping the entire Scratch engine.
   
2. **Algorithmic Difficulty:** Instead of static levels, I developed a dynamic difficulty system using 'My Blocks' and conditional logic that adjusts pipe speed and spawn rates based on the current score.

3. **Concurrency & Synchronization:** To avoid audio overlapping between 'Point' and 'Level Up' sounds, I used a synchronization strategy (wait 0s) to ensure the program checks the level state before firing the default score sound.

4. **Abstraction:** I used custom blocks with inputs (parameters) to handle the duck's physics, making the code more modular and meeting CS50's technical requirements.

## 📝 Academic Honesty
This project was developed by me for CS50x. I used AI as a "thought partner" to debug complex clone behaviors and to discuss software engineering patterns (like state machines), ensuring a deep understanding of every logic gate implemented.
