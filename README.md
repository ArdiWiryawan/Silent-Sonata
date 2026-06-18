# Silent Sonata 🎹
> **An Atmospheric 3D Psychological Rhythm-Reaction Web Experience**

[![Status](https://img.shields.io/badge/Status-Prototype-yellow?style=for-the-badge)](https://github.com/ArdiWiryawan/Silent-Sonata)
[![Stack](https://img.shields.io/badge/Stack-Three.js_/_Web_Audio_API-blueviolet?style=for-the-badge&logo=javascript)](https://developer.mozilla.org/en-US/docs/Web/API/Web_Audio_API)
[![Demo](https://img.shields.io/badge/Live_Demo-Play_in_Browser-orange?style=for-the-badge&logo=github)](https://ArdiWiryawan.github.io/Silent-Sonata/)

Silent Sonata is an immersive psychological fantasy rhythm-reaction browser game. Designed around an auditory narrative, players guide a young pianist trapped inside a coma to recover three core musical notes and reconstruct the Final Sonata. 

*“Vision lies. Music tells the truth.”*

---

## 🌟 Key Features

### 🎧 1. Interactive Audio Synthesis
- Built using the **Web Audio API** to generate real-time spatial audio notes (Low, Mid, High directions).
- Auditory-based gameplay where players must listen, remember, and identify sound frequencies to proceed.
- Fully integrated assist accessibility options, including mono audio mode and audio timing buffers.

### 🌐 2. Browser-Ready 3D Render
- Real-time 3D environments rendered directly in the browser using **Three.js**.
- Fluid interactive elements and visual reaction cues (timing rings, glow feedback) synced to musical notes.
- Pure single-file architecture (`index.html`) loaded via fast CDN resources.

### 📜 3. Storytelling & Narrative Progression
- Stage-by-stage progression from Prologue to Epilogue detailing the protagonist's sub-conscious recovery.
- Bilingual interface (Indonesian and English) with customizable volume, assist timing overlays, and gameplay preferences.

---

## 🎨 Visual & Sound Philosophy
- **Atmosphere**: Dark, moody, and melancholic fantasy theme reflecting trauma, recovery, and performance pressure.
- **Auditory Clarity**: Headphones are highly recommended to differentiate spatial stereo locations of musical notes.

---

## 🛠️ Tech Stack
- **Graphics**: [Three.js](https://threejs.org/) (WebGL 3D engine)
- **Audio**: Native [Web Audio API](https://developer.mozilla.org/en-US/docs/Web/API/Web_Audio_API)
- **Styling**: Tailwind CSS & Google Fonts (`Playfair Display` & `Inter`)
- **Language**: Vanilla JavaScript (ES6)

---

## 📂 Project Structure
```text
Silent-Sonata/
├── index.html                                            # Main game application file
├── Silent_Sonata_Full_Game_Execution_Documentation.md    # Extensive GDD & technical specs
├── assets/                                               # Game sprites & graphic assets
└── README.md                                             # Project documentation
```

---

## 🚀 Running Locally
Because this game utilizes external resources and media rendering, running a local HTTP server is recommended to bypass browser file origin (CORS) policy:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/ArdiWiryawan/Silent-Sonata.git
   cd Silent-Sonata
   ```
2. **Start a local development server:**
   *Using Node.js:*
   ```bash
   npx serve .
   ```
   *Using Python:*
   ```bash
   python -m http.server 8000
   ```
3. Open `http://localhost:8000` or `http://localhost:3000` in your web browser.

---

## 🧠 Technical Learnings
- **Audio Node Hooking**: Gained experience in chaining GainNodes, OscillatorNodes, and StereoPannerNodes to build interactive sound boards.
- **3D Render Optimizations**: Integrated RequestAnimationFrame loops with Three.js camera controllers to maintain a consistent 60FPS refresh rate on web browers.

---

## 📄 License
This project is open-source and licensed under the [MIT License](LICENSE).
