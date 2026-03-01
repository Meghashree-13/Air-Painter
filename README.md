# Air Painter | Interactive Canvas

A browser-based interactive application that allows you to draw on a digital canvas using hand gestures, captured via your webcam.



## 🚀 Overview

Air Painter uses **MediaPipe Hands** to detect hand landmarks in real-time. By tracking the position of your index finger, it maps gestures to a digital drawing canvas, allowing for a touchless painting experience directly in your browser.

## 🛠️ Features

* **Touchless Drawing:** Draw in the air using your index finger.
* **Pause Control:** Lower your finger or make a fist to stop drawing.
* **Color Palette:** Choose from 5 vibrant neon colors.
* **Adjustable Brush:** Change the brush size dynamically.
* **Canvas History:** Undo and Redo your strokes (`MAX_HISTORY = 20`).
* **Clear Canvas:** Wipe the canvas clean instantly.
* **Save Screenshot:** Download your masterpiece as a PNG image directly to your device.

## ⚙️ How It Works

1.  **Detection:** The webcam feed is processed using MediaPipe to identify hand landmarks (`8` for index finger tip).
2.  **Smoothing:** Exponential Moving Average (EMA) is applied to the coordinates to prevent shaky lines.
3.  **Rendering:** The drawing canvas renders lines based on the smoothed coordinates when the "pointing" gesture is detected.
4.  **Export:** The canvas context is converted to a PNG data URL for saving.



## 🛠️ Technology Stack

| Component | Technology |
| :--- | :--- |
| **Framework** | Vanilla JS, HTML5, CSS |
| **Styling** | Tailwind CSS |
| **AI/ML** | MediaPipe Hands |
| **Icons** | Lucide Icons |

## 🖥️ Setup & Installation

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/your-username/air-painter.git](https://github.com/your-username/air-painter.git)
    ```

2.  **Run locally:**
    Since this uses browser-based modules, you must serve it using a local server (e.g., Live Server extension in VS Code). **It will not work by just double-clicking the HTML file.**

3.  **Permissions:** Allow webcam access when prompted by your browser.

## 🛡️ License

This project is licensed under the [MIT License](LICENSE).
