# Air Painter | Interactive Canvas

An interactive web application that allows you to draw in the air using hand gestures, powered by AI.



## 🚀 Overview

Air Painter uses your webcam and **MediaPipe Hand Landmarker** to track your finger movements in real-time. By raising your index finger, you can draw on a virtual canvas directly in front of you.

## 🛠️ Features

* **Real-time Hand Tracking:** Uses advanced AI to detect your hand and fingers.
* **Gestural Drawing:** Raise your index finger to draw; make a fist or lower your finger to stop.
* **Customizable Brush:** Adjust the stroke thickness via the UI.
* **Color Palette:** Choose from 5 vibrant colors to create your artwork.
* **Undo/Redo & Clear:** Full control over your drawing history.
* **Low Latency:** Optimized for smooth, responsive drawing.

## ⚙️ How It Works

1.  **Camera Input:** The app captures video from your webcam via the browser.
2.  **AI Processing:** MediaPipe detects hand landmarks (key points on your hand).
3.  **Gesture Detection:** The app checks if your index finger is raised (`indexTip.y < indexPip.y`) compared to other fingers.
4.  **Canvas Drawing:** If you are "pointing," the app draws lines based on the movement of your fingertip.



## 🛠️ Technology Stack

| Component | Technology |
| :--- | :--- |
| **Frontend** | HTML5, Tailwind CSS |
| **AI/ML** | Google MediaPipe Hands |
| **Scripting** | Vanilla JavaScript |
| **Icons** | Lucide Icons |

## 🖥️ Setup & Installation

This is a client-side web application. You do not need to install a backend.

1.  Clone this repository or download the `index.html` file.
2.  Open `index.html` in a modern web browser (Chrome, Edge, Firefox, etc.).
3.  **Allow Camera Access** when prompted by your browser.

## 🕹️ User Instructions

| Action | Gesture |
| :--- | :--- |
| **Draw** | Raise your Index Finger. |
| **Stop Drawing** | Make a Fist or lower your hand. |
| **Change Color** | Click on the colored circles in the top menu. |
| **Change Size** | Use the slider next to the brush icon. |
| **Undo/Redo** | Click the arrow buttons in the top menu. |
| **Clear Canvas** | Click the trash icon. |

## 📋 Permissions & Privacy

* **Camera:** This app requires webcam access to function. **No video data is sent to a server**; all processing happens locally in your browser.
* **Cookies:** This app does not use cookies.

## 🛡️ License

This project is licensed under the [MIT License](LICENSE).