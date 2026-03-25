# 🏎️ R1 Racing

**R1 Racing** is a 2D top-down car racing game built as a **Rabbit R1 Creation** — a tiny HTML/CSS/JS app that runs natively inside the R1's built-in WebView.

---

## 🎮 Gameplay

Your car auto-accelerates to top speed. You steer with the scroll wheel and brake with the side button. Each lap has a countdown timer — run out of time and it's game over. Survive as many laps as you can while dodging traffic and collecting powerups.

### Controls

| Input | Action |
|---|---|
| **Scroll UP** | Steer up |
| **Scroll DOWN** | Steer down |
| **Side button tap** | Brake (short pulse) |
| **Side button hold** | Hold brake |

### Rules

- **Off-road** — driving on grass slows you down but won't end your run
- **Collisions** — each NPC hit drains 1 HP from your health bar (8 HP total)
- **Timer** — complete each lap before the countdown hits zero
- **Difficulty** — laps get longer every lap; one more NPC car joins the road every 2 laps (up to 10)
- **Powerups** — grab ⏱ to add time and ♥ to restore HP; they get rarer each lap

---

## 🐇 Installing on your R1

Scan the QR code below to install R1 Racing directly on your Rabbit R1:

![Install QR Code](https://jdmasa.github.io/R1Racing/qrcode.png)

Or visit [rabbit.tech/creations](https://rabbit.tech/creations) and deploy `index.html` manually.

---

## 🛠️ Built with Claude

This project was built entirely using the **Rabbit R1 Creations Claude Skill** — a custom Claude skill that provides the SDK constraints, API patterns, and device-specific gotchas needed to build great R1 Creations without trial and error.

👉 **[Get the skill on GitHub](https://github.com/jdmasa/rabbit-r1-creations_claude_skill)**

The skill teaches Claude about:
- The fixed 240×282px canvas and WebView constraints (no WebGL, no inline `onclick`, etc.)
- Hardware events: `scrollUp`, `scrollDown`, `sideClick`, `longPressStart`, `longPressEnd`
- Native bridges: LLM, accelerometer, storage, camera, microphone
- Proven patterns for PTT voice assistants, vision apps, and interactive games

---

## 📁 Project structure

```
index.html   ← the entire game (single-file Creation)
README.md    ← this file
```

---

## 📝 License

MIT — do whatever you want with it.
