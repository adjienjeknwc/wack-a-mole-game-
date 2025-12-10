# 🔨 Whack-a-Mole - Interactive Browser Game



> **Role:** Product Engineer (Game Logic, UX, & Frontend)
> **Stack:** HTML5, CSS3, JavaScript (DOM Manipulation)
> **Focus:** Event Handling, State Management, & Gamification

---

## 1. 💼 The Business Context (BA)

### The Concept
"Gamification" is a powerful tool for increasing user retention. This project simulates an arcade-style environment to test reaction times and engagement loops.

### The Objective
To build a lightweight, browser-based game that runs smoothly on low-end devices while maintaining high frame rates. The goal is to maximize **User Session Time** through instant feedback loops (score incrementing).

### Key Features Defined
* **Randomized Spawning Algorithm:** Ensures the gameplay is unpredictable and non-repetitive.
* **Score & Timer Logic:** Visual metrics that create urgency and competitive drive.
* **Difficulty Scaling:** (Planned V2) Speed increases as the score gets higher.

---

## 2. 🎨 User Experience & Design (UX)

### Interaction Design
* **Immediate Feedback:** When a mole is clicked, the visual state changes instantly (mole drops), confirming the action to the user.
* **Visual Clarity:** High contrast between the "Dirt" and the "Mole" ensures players can react quickly without visual confusion.

### Gamification Elements
* **The "Hook":** Short, 10-second game loops encourage "Just one more try" behavior.
* **Cursor Customization:** The mouse cursor transforms into a hammer, immersing the user in the game mechanics.

---

## 3. 🏗️ Technical Architecture (Dev)

### The Game Loop Logic
Unlike static websites, this project relies on **Asynchronous Event Handling**.

**Core Functions:**
1.  `randomTime(min, max)`: Generates a random duration for the mole to stay up.
2.  `randomHole(holes)`: Uses recursion to ensure the same hole isn't picked twice in a row (preventing logic bugs).
3.  `peep()`: The main engine that triggers the CSS class changes based on the calculated time.

### DOM Manipulation Strategy
* **Event Delegation:** `click` listeners are attached efficiently to handle rapid user input.
* **"IsTrusted" Validation:** Ensures that the clicks are real user actions (preventing script cheating).

**State Management:**
* A global `score` variable tracks progress.
* `lastHole` variable prevents repetitive spawning patterns.

---

## 4. 🚀 How to Run Locally

1.  **Clone the repo:**
    ```bash
    git clone [https://github.com/aditi-verma/whack-a-mole.git](https://github.com/aditi-verma/whack-a-mole.git)
    ```
2.  **Open the folder:**
    Navigate to the project directory.
3.  **Launch:**
    Open `index.html` in your browser.

---

## 5. 🔮 Future Roadmap

* **Persistent High Scores:** Use `localStorage` to save the best score even after the browser closes.
* **Sound Effects (SFX):** Audio cues for "Whack" and "Miss" to enhance immersion.
* **Mobile Touch Support:** Optimize click events for touch screens.

---

### 📬 Contact
* **Designed & Built by:** Aditi Verma

* **Email:** aditivermauk@gmail.com
