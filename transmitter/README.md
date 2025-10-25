# 📡 Radio Communication System using Raspberry Pi  

This project demonstrates how to control and tune a **radio receiver using Raspberry Pi** via **I²C communication**.  
The system allows the user to set, adjust, and mute frequencies of an FM radio module connected to the Raspberry Pi.  
It is implemented in **Python 3** and provides a **keyboard-controlled interface** for real-time radio tuning.  

---

## 🎯 Project Overview  

The **Radio Communication System using Raspberry Pi** provides a hands-on implementation of wireless communication by controlling an FM tuner chip through the Raspberry Pi’s I²C interface.  
This project showcases **signal transmission concepts**, **frequency control**, and **hardware communication** using Python.  
It is ideal for enthusiasts and students learning about **embedded systems**, **IoT hardware**, and **radio frequency communication**.

---

## ⚙️ Features  

- 🎛️ Real-time frequency tuning using keyboard commands  
- 🔇 Mute and unmute radio functionality  
- ⏱️ Interactive terminal interface with instant feedback  
- 🧠 Demonstrates I²C-based hardware control via Python  
- 💡 Educational project for IoT and RF communication concepts  

---

## 🧩 Hardware Requirements  

- Raspberry Pi (Model 3, 4, or newer)  
- I²C-based FM Radio Module (e.g., **TEA5767** or similar)  
- Jumper wires and breadboard  
- Internet connection (for package installation)  

---

## 💻 Software Prerequisites  

Before running the project, execute the following setup commands in your Raspberry Pi terminal:

```
sudo apt update
sudo apt upgrade -y
sudo raspi-config     # Enable I²C under Interface Options
sudo apt install i2c-tools -y
sudo i2cdetect -y 1   # Verify I²C device connection
sudo apt install libsndfile1-dev -y
sudo apt install python3-smbus python3-pip -y
```
🚀 How to Run
Clone the Repository:
```
git clone https://github.com/yourusername/radio-communication-pi.git
cd radio-communication-pi
```

Run the Python Script:
```
python3 radio_control.py
```

Keyboard Controls:

Key	Action
f	Set frequency to 101.1 MHz
v	Set frequency to 102.1 MHz
w	Increase frequency by 1 MHz
s	Decrease frequency by 1 MHz
e	Increase frequency by 0.1 MHz
d	Decrease frequency by 0.1 MHz
m	Mute the radio
u	Unmute / resume last frequency
q	Quit and mute on exit
