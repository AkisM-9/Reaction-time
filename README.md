# Arduino Reaction Time Game for Two Players

This is a simple **reaction time game** built with an **Arduino**, **buttons**, **LEDs**, and a **16x2 I2C LCD display**. Two players compete to press their button as soon as an LED turns on — the fastest wins the round.

---

## 🎮 Gameplay

- The game randomly lights up one of three LEDs after a short delay.
- Players must wait for the LED to turn on and press their button **as quickly as possible**.
- First to press after the LED wins the round.
- First to **5 points** wins the game.

---

## 🧰 Components

- 🧠 Arduino Uno/Nano/Mega
- 🔘 2 Push buttons (normally open)
- 💡 3 LEDs (with current-limiting resistors)
- 🖥️ 16x2 I2C LCD module (address usually `0x27`)
- ⚡ Jumper wires & breadboard
- 📦 One box for the buttons if possible 

---

## ⚙️ Wiring Overview

- **Buttons:**  
  - Player 1 → Digital pin 2  
  - Player 2 → Digital pin 4  
  - Connect other button terminal to GND  

- **LEDs:**  
  - LED1 → Pin 7  
  - LED2 → Pin 8  
  - LED3 → Pin 9  

- **LCD:**  
  - Connect via I2C (SDA → A4, SCL → A5 on Uno)

---

## 🔁 How It Works

1. Each round starts with a short randomized delay.
2. One of the LEDs lights up.
3. Players press their buttons as fast as possible.
4. The player who presses first after the LED wins the round.
5. LCD shows live scores and winner after 5 rounds.

## 🛠️ Tips & Troubleshooting

- **LCD not working?** Try changing the I2C address (`0x27` → `0x3F`).
- **False button presses?** Add external pull-down resistors or enable internal pull-ups.
- **LEDs not lighting?** Check resistor values and LED polarity.

---

## ✅ Improvements & Add-ons

- Add a buzzer for sound effects.
- Record and display reaction time in milliseconds.
- Add a reset button to replay the game.

---

Images🖼️
![alt text](r-front.jpg)
![alt text](r-top.jpg)
![alt text](r-side.jpg)

Have fun building and improving your Arduino reaction time game!


