# STM32-LIS302DL Motion Tracker

This project uses an **STM32F4 Discovery Board** and its onboard **LIS302DL 3-axis accelerometer** to detect motion and indicate tilt direction in real time using LEDs.

---

## 📌 Features
- SPI interface between STM32 and LIS302DL
- Real-time X and Y axis tilt detection
- LED indication for tilt direction
- Configurable sensitivity (±2g or ±8g)

---

## 🛠 Hardware Used
- STM32F4 Discovery Board (STM32F405xx)
- LIS302DL Accelerometer (onboard sensor)
- Onboard LEDs (PD12–PD15)

---

## 🔌 Pin Connections
| Signal | STM32 Pin | Description |
|--------|-----------|-------------|
| CS     | PE3       | Chip Select |
| SCK    | PA5       | SPI Clock   |
| MISO   | PA6       | SPI Data In |
| MOSI   | PA7       | SPI Data Out |
| LEDs   | PD12–PD15 | Motion Direction |

---

## ⚙️ How It Works
1. Initializes SPI in 16-bit mode.
2. Configures LIS302DL to ±2g sensitivity.
3. Reads X, Y, Z acceleration values.
4. Lights LEDs based on motion direction:
   - PD12 → +X tilt
   - PD13 → -X tilt
   - PD14 → +Y tilt
   - PD15 → -Y tilt

---

## 📂 File Description
- `main.c` → Main application code
- `lis302dl.h` → Sensor register definitions
- `output_demo/` → Photos & videos of output

---

## 🚀 Build & Flash
1. Open in **STM32CubeIDE**.
2. Build project (`Ctrl + B`).
3. Connect board via ST-LINK.
4. Flash to board (`Run → Debug`).

---

## 📸 Output Demo


---

## 📜 License
MIT License – free to modify and use.
# STM32-LIS302DL-Motion-Tracker
