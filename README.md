# 🛣️ Lane Follower Robot  

An **autonomous lane-following robot** built using Arduino and IR sensors.  
The robot detects and follows a black track using real-time motor control logic and simple sensor feedback.

---

## 🚀 Features  

- 🔍 **Lane detection** using IR sensors  
- ⚙️ **Smooth motor control** with TB6612 / L298N driver  
- 🧭 **Automatic left/right correction** for accurate path tracking  
- ⚡ **Real-time response** to sensor input  
- 🔋 **Compact, low-cost implementation** using Arduino  

---

## 🧩 Components Used  

| Component | Quantity | Description |
|------------|-----------|-------------|
| Arduino Mega / UNO | 1 | Main controller |
| IR Sensor Module (2 or 5 channel) | 1 | Detects lane contrast |
| Motor Driver (L298N / TB6612FNG) | 1 | Controls DC motors |
| DC Motors | 2 | Drive motors |
| Power Supply | 1 | 7.4V or 12V battery pack |

---

## ⚙️ Circuit Connections  

| Arduino Pin | Component | Function |
|--------------|------------|----------|
| 8, 9 | IR Sensors | Left & Right line detection |
| 22, 24, 5 | TB6612 AIN1, AIN2, PWMA | Left motor control |
| 26, 28, 6 | TB6612 BIN1, BIN2, PWMB | Right motor control |
| 30 | TB6612 STBY | Motor driver enable |

---


---

## 🧠 Working  

1. **IR sensors** detect the black line on a white surface.  
2. **Arduino** reads the sensor values and determines deviation from the lane.  
3. **Motor driver** adjusts left and right motor speeds accordingly:  
   - Center → Move Forward  
   - Left sensor active → Turn Left  
   - Right sensor active → Turn Right  
   - No line → Stop or minor correction  

---

## 🧪 Setup  

1. Clone this repository:  
   ```bash
   git clone https://github.com/Sir-dragmaster-j/lane-follower-robot.git
   cd lane-follower-robot

Open the .ino file in Arduino IDE.

Select your Board (UNO/Mega) and Port.

Upload the code to your board.

Place the robot on a lane-marked track and test

## 🧰 Tools Used
- Arduino IDE
- Embedded C/C++

## 👨‍💻 Author
**Sujay J**  
📍 Mysore, Karnataka  
🎓 B.E. in AI & Data Science — MIT Mysore (VTU)  
🔗 [GitHub](https://github.com/Sir-dragmaster-j) | [LinkedIn](https://www.linkedin.com/in/sujay-j-b59959357)

## 📜 License
This project is licensed under the **MIT License** — free to use and modify.
