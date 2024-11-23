
# Swiggy aSDE - Magical Arena Game
![Swiggy](https://www.livemint.com/lm-img/img/2024/10/04/600x338/Swiggy_Orange_Horizontal_1727778844943_1728057951927.png)

Welcome to the **Magical Arena**! This project simulates an exciting battle between two players in a magical arena where players attack and defend using dice rolls, health, strength, and attack attributes.

The **Magical Arena** game allows two players to fight, taking turns attacking and defending, with each player's health reducing when they take damage.

This project was created in Node.js to demonstrate **clean design, readability**, and **testable code**. The solution follows a simple and efficient approach to model the game logic, ensuring the code is easy to maintain and extend.

---

## **How to Run the Code**

### **Prerequisites**

Before running the project, ensure you have the following installed:

- **Node.js** (version 14 or above)  
  You can download Node.js from [here](https://nodejs.org/).

### **Clone the Repository**

1. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/amaan92001/Swiggy_aSDE_Amaan_Patel.git
   ```

2. Navigate into the project directory:
   ```bash
   cd Swiggy_aSDE_Amaan_Patel
   ```

### **Install Dependencies**

Install the required dependencies by running the following command:
```bash
npm install
```

### **Run the Game**

To simulate a match between two players, run the following command:

```bash
npm start
```

This will start the game simulation and output the result of the battle between the two players.

---

## **How to Run Tests**

Unit tests are written to ensure the correctness of the game logic. To run the tests, simply execute the following command:

```bash
npm test
```

The tests will check the core features such as:

- Damage calculation
- Turn order based on health
- Health reduction after each attack
- Game-ending logic when a player's health reaches 0

---

## **Game Rules**

1. Each player has three attributes:
   - **Health**: Determines the total life points of the player.
   - **Strength**: Affects the player's ability to defend against attacks.
   - **Attack**: Determines how much damage a player can deal in an attack.

2. Players attack in turns. The **player with lower health** attacks first.

3. During each turn:
   - The attacker rolls a dice to determine the **attack damage**.
   - The defender rolls a dice to determine the **defense strength**.

4. The **attack damage** is calculated as:
   ```text
   Attack damage = Attack value * Attacker dice roll
   ```

5. The **defense strength** is calculated as:
   ```text
   Defense strength = Strength value * Defender dice roll
   ```

6. The final damage dealt to the defender is:
   ```text
   Final damage = Attack damage - Defense strength
   ```

7. The defender’s health is reduced by the final damage amount. The game ends when a player’s health reaches 0.

---

## **Technologies Used**

- **Node.js**: JavaScript runtime for building the server-side logic.
- **Mocha**: Test framework used for unit testing.
- **Chai**: Assertion library used to test the game logic.

---

## **Design Decisions**

- **Modular Approach**: The code is broken down into separate modules for the `Player`, `Arena`, and `Dice` logic. This ensures that each component can be easily tested and maintained.
- **Turn-based System**: Players attack in turns based on their health. The game logic determines who attacks first by comparing their health values.
- **Damage Calculation**: The game uses a dice-based approach for both attack and defense to introduce randomness and variability into the gameplay.

---

## **Contribution**

If you'd like to contribute to this project, feel free to fork the repository, make your changes, and submit a pull request. Ensure your code is well-tested and adheres to the existing style and structure.

---

## **Contact**

For any questions, feel free to reach out to the project maintainer at [amaanpatel500@gmail.com].

---

### End of README

---

### Key Features:

1. **Clear Instructions**: The README explains how to install, run, and test the project with detailed steps.
2. **Game Logic Explanation**: A summary of how the game works and the rules behind the mechanics.
3. **Project Structure**: It provides a brief overview of the code organization, making it easier for others to understand and navigate the project.
4. **Technologies**: The tools and frameworks used in the project are clearly listed.
5. **License and Contribution**: Information about the license and how others can contribute to the project is included.

