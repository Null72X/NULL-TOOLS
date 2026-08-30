# 🛠️ NULL TOOLS

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
![Platform: Browser](https://img.shields.io/badge/Platform-Cross--Platform-brightgreen.svg)
![Technologies: HTML / CSS / JS](https://img.shields.io/badge/Tech-HTML%20%7C%20CSS%20%7C%20JS-orange.svg)

A clean, high-performance, web-based utility suite designed for reverse engineers, game developers, and binary analysts. **NULL TOOLS** offers a seamless interface to convert Array of Bytes (AOB) patterns between C#, C++, and Python formats, and to calculate relative 3D skeletal bone offsets instantly.

Built as a single, lightweight, offline-first client application, it requires no installation, server backend, or external dependencies.

---

## ⚡ Features

### 1. Byte Forge (AOB Converter)
Easily translate memory patterns and byte arrays between different languages while maintaining wildcards/masks.
*   **Supported Formats:**
    *   **C#**: Space-separated hex format (e.g., `90 90 ?? AB`)
    *   **C++**: Comma-separated array format (e.g., `0x90, 0x90, '?', 0xAB`)
    *   **Python**: Hex-escaped regex/string format (e.g., `\x90\x90.\xAB`)
*   **Live Translation:** Outputs update in real-time as you type or paste.
*   **Byte Counter:** Automatically counts and displays the active payload length.
*   **Instant Actions:** Clear the workspace or copy converted buffers directly to the clipboard with one click.

### 2. 🦴 External Bones Finder
An offset calculator optimized for external memory writing/reading. By providing a base chest offset, the tool computes other adjacent skeletal bones relative to it:
*   **Head Offset:** `Chest - 0x4`
*   **Neck Offset:** `Chest + 0x4`
*   **Neck Left Offset:** `Chest + 0x34`
*   **Neck Right Offset:** `Chest + 0x30`
*   **Left Shoulder Offset:** `Chest + 0x40`
*   **Right Shoulder Offset:** `Chest + 0x44`

### 3. Modern Dark Theme
*   **Immersive Design:** Futuristic dark theme with subtle glowing gradients, glassmorphism, and red accent cues.
*   **Responsive Layout:** Fully optimized for desktop monitors, tablets, and mobile devices.
*   **Notification Toasts:** Non-intrusive status toast alerts acknowledging successful calculations, format changes, and clipboard actions.

---

## 🛠️ Technical Details & Stack

*   **Markup & Layout:** Semantic HTML5 structured for fast rendering and accessibility.
*   **Styling:** Pure CSS3 custom properties (variables), radial backgrounds, and layout flexing. No heavy external frameworks (like Tailwind or Bootstrap) required.
*   **Logic:** Native Vanilla JavaScript (ES6+) for ultra-low latency inputs and memory-efficient conversions.
*   **Fonts:** Interfaced with Google Fonts (`Plus Jakarta Sans` for clean UI typography and `JetBrains Mono` for precise hex data displays).

---

## 🚀 Getting Started

Since **NULL TOOLS** is client-side only, you can run it directly:

1.  Clone or download the project repository.
2.  Locate `index.html`.
3.  Double-click to open it in any modern web browser (Chrome, Firefox, Edge, Safari, Brave, etc.).

No compilation, local servers, or package installations required.

---

## 📂 Project Structure

```text
NULL-TOOLS/
├── index.html     # Single-page application (All styling, scripting, and structure)
└── README.md      # Documentation
```

---

## ⚖️ License

Distributed under the MIT License. See `LICENSE` (if available) or the badge above for more details.
