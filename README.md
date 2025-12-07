# 🎹 Smart Piano Practice System

A smart piano practice system based on **Digital Piano + LED Key Lights + Local Control + Multiple Practice Modes**.  
The system lights up the keys you should press, reads what you actually play via MIDI, and helps you practice step-by-step or in real-time follow mode.

---

## 🚀 Project Goal

To build an intelligent piano practice system that:

- ✅ Uses **LED lights** to guide which keys to press  
- ✅ Uses **MIDI input from a digital piano** to track real performance  
- ✅ Supports **multiple practice modes**  
- ✅ Can be extended with **AI-based analysis & feedback**

The goal is to upgrade piano practice from *reading sheet music* to:

> **Lights + Real-time Interaction + AI-assisted Training**

---

## 🎯 Core Features

### 1️⃣ Step Practice Mode (Press to Advance)

- Only the **current target key or chord** is lit
- ✅ **The system waits until the correct key(s) are pressed**
- Wrong notes:
  - Can be ignored
  - Or flash red as feedback (without moving forward)
- Best for:
  - Beginners
  - Finger training
  - Hands-separate practice

---

### 2️⃣ Follow / Playalong Mode (Lights Follow the Rhythm)

- Keys light up **according to the song’s timing**
- ✅ **The system does NOT wait for the player**
- The user follows the lights in real time
- Best for:
  - Rhythm training
  - Fluency development
  - Performance simulation

---

## 📥 System Input

- **Sheet Music / MIDI Files**
  - Define what *should* be played
- **Digital Piano MIDI Input**
  - Defines what the user *actually plays*

---

## 📤 System Output

- 💡 **Keyboard LED Lights**
  - Visually show which key to press
  - White & black keys must be clearly distinguishable
- 🖥️ **Screen UI (Web / App)**
  - Shows song, progress, mode, and status
- 🤖 **(Future) AI Feedback**
  - Performance insights, mistake analysis, long-term progress

---

## 🧱 Hardware Components

- 🎹 **Digital Piano (MIDI supported)**
- 💡 **Individually addressable LED strip (WS2812B / SK6812)**
- 🧠 **ESP32 controller (for LED control)**
- 🖥️ **Local Control Device**
  - Current: PC
  - Future: Small always-on device (e.g., Raspberry Pi)

---

## 🧩 Software Architecture (Current Phase)

- **Local Backend**
  - Reads MIDI input from the piano
  - Controls the LED lights
  - Manages practice state (Step / Follow)
  - Exposes HTTP & WebSocket APIs

- **Frontend UI (Web)**
  - Runs in the browser
  - Used for:
    - Start / Pause practice
    - Song selection
    - Mode switching
    - Practice visualization

---

## 🛣️ Development Roadmap

### ✅ V1 (Current)
- PC as the local controller
- Browser as the UI
- ESP32 + LED strip + Digital Piano

---

### ✅ V2
- Add cloud-based AI for advanced analysis
- Real-time control remains local

---

### ✅ V3
- Migrate local backend from PC to a **dedicated small device**
- Mobile phone becomes the main control UI

---

### ✅ V4 (Final Form)
- Mobile phone directly connects to:
  - Digital piano (Bluetooth MIDI / OTG)
  - LED controller (BLE / Wi-Fi)
- No dedicated local box required
- AI runs mainly in the cloud

---

## ❌ Not in Scope (For Now)

- Detailed scoring system
- Cloud account system
- Commercial packaging
- Heavy AI models

---

## ✅ Current Core Focus

> **Correct LEDs light up →  
> User presses the correct keys →  
> The system advances (or follows rhythm) →  
> MIDI input is accurately tracked**

---

## 📌 Keywords

- Smart Piano
- MIDI
- WS2812B LED
- ESP32
- Step Practice Mode
- Playalong Mode
- Local Control System

---

## 📄 License

MIT (can be adjusted)
