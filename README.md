<p align="center">
  <img src="https://img.icons8.com/?size=200&id=22540&format=png&color=4CAF50" width="120" />
</p>

<h1 align="center">🛣️ Autonomous Lane Follower Robot</h1>
<p align="center"><b>A fast, stable, and intelligent Arduino-based lane detection robot</b></p>

<p align="center">
  <img src="https://img.shields.io/badge/Arduino-Mega/UNO-blue?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Sensors-IR-black?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Motor_Driver-TB6612/L298N-orange?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Language-C/C++-brightgreen?style=for-the-badge" />
</p>

---

## ⚡ Overview  
An **autonomous lane-following robot** designed to detect and track a black line using IR sensors.  
The robot adjusts its motor speeds in real-time to stay centered on the lane, making it ideal for robotics competitions, demos, and automation learning.

---

## 🚀 Key Features  

- 🔍 **Dual/5-channel lane detection**  
- ⚡ **Fast real-time correction** using IR feedback  
- 🧭 **Smooth left/right turning algorithm**  
- 🎛️ **TB6612 / L298N motor driver support**  
- 🔋 **Lightweight + low power consumption**  
- 🛠️ **Simple, clean, modular codebase**  

---

## 🧩 Components Used  

| Component | Qty | Purpose |
|----------|-----|----------|
| Arduino Mega / UNO | 1 | Main microcontroller |
| IR Sensor Module (2-ch / 5-ch) | 1 | Line detection |
| TB6612FNG / L298N | 1 | Motor driver |
| DC Motors | 2 | Locomotion |
| Battery (7.4V/12V) | 1 | Power supply |

---

## ⚙️ Wiring & Pin Mapping  

| Arduino Pin | Connected To | Description |
|-------------|--------------|-------------|
| 8, 9 | IR Sensor | Left & Right detection |
| 22, 24, 5 | AIN1, AIN2, PWMA | Left motor control |
| 26, 28, 6 | BIN1, BIN2, PWMB | Right motor control |
| 30 | STBY | Motor driver standby enable |

---

## 🧠 Working Principle  

1. **IR sensors** detect black line (absorbs IR) vs white surface (reflects IR).  
2. Based on sensor output:  
   - ⚪ **Both HIGH** → Move **Forward**  
   - 🔴 Left detects line → Turn **Left**  
   - 🔵 Right detects line → Turn **Right**  
   - ⚫ No line → Stop or search  
3. **Arduino** processes input and adjusts PWM motor speed via motor driver.  
4. The robot constantly corrects itself to stay centered on the lane.

---

## 🧪 Setup Instructions  

### 1️⃣ Clone the repository  
```bash
git clone https://github.com/Sir-dragmaster-j/lane-follower-robot.git
cd lane-follower-robot
```

### 2️⃣ Open in Arduino IDE  
- Open the `.ino` file  
- Select board → **Arduino UNO/Mega**  
- Select correct **COM port**  

### 3️⃣ Upload the code  
Click **Upload** → Wait for successful flash.

### 4️⃣ Test your robot  
Place it on a black-tape track and watch it follow the lane automatically.

---

## 🧰 Tools & Technologies  
- Arduino IDE  
- C/C++  
- TB6612 / L298 motor driver  
- IR sensor modules  

---

## 📸 (Optional) Add Robot Photos  
You can place photos in `/images` and embed them here.

---

## 👨‍💻 Author  
**Sujay J**  
📍 Mysore, Karnataka  
🎓 B.E. AI & Data Science — MIT Mysore (VTU)  
🔗 [GitHub](https://github.com/Sir-dragmaster-j)  
🔗 [LinkedIn](https://www.linkedin.com/in/sujay-j-b59959357)

---

## 📜 License  
This project is licensed under the **MIT License** — free to use, modify, and distribute.

---
