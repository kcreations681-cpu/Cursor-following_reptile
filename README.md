# Cursor-following_reptile
# 🦎 Sci-Fi Procedural Reptile

A super cool interactive animation of a glowing sci-fi creature that follows your mouse! Built with **p5.js** and powered by real animation techniques used in games and movies.

> *(Move your mouse around the screen and watch it chase you!)*

---

## ✨ What It Does

- 🐍 **Follows your cursor** — the creature aggressively chases your mouse using a chain of body segments
- 🦿 **8 realistic legs** — each leg has its own "brain" that decides when to lift and step forward
- 💀 **Sci-fi skull head** — glowing red slit-pupil eyes, neon teeth, and bony plates
- 🌀 **Circles you when idle** — stop moving and it coils around your cursor like a predator
- 💡 **Neon glow effects** — cyan ridge lines, pulsing eye glow, and drop shadows

---

## 🧠 Cool Tech Inside

This project uses real techniques from game development and animation:

| Technique | What It Does |
|---|---|
| **Inverse Kinematics (IK)** | Makes each body segment smoothly follow the one in front of it — like a real spine |
| **Leg Anchoring** | Each foot stays "glued" to the ground until the body moves too far, then it steps forward in an arc |
| **Sine Wave Slither** | A math wave makes the body wiggle side to side so it feels alive even when still |
| **Procedural Animation** | None of the movement is hand-animated — the code figures it all out automatically! |

---

## 🚀 How to Run It

No installs needed! It's just one HTML file.

1. **Download** `scifi-reptile.html`
2. **Double-click** it to open in your browser
3. **Move your mouse** around and watch the creature follow!

That's it. Done. 🎉

---

## 📁 File Structure

```
scifi-reptile/
│
└── scifi-reptile.html    ← the entire project (yes, just one file!)
```

Everything — the animation, the physics, the drawing — lives in that single file.

---

## 🛠️ How It Was Built

- **[p5.js](https://p5js.org/)** — a beginner-friendly JavaScript library for creative coding and graphics
- **Vanilla JavaScript** — no frameworks, no install needed
- Loaded directly from a CDN (the internet), so you don't need to download p5.js separately

---

## 🧩 How the Code Works (Simple Version)

```
Every frame (60 times per second):
  1. Move the HEAD toward the mouse
  2. Pull each BODY SEGMENT to follow the one in front (IK chain)
  3. Add a WIGGLE sine wave to make it slither
  4. Check each FOOT — is it too far from the body?
       → YES: Lift the foot and step it forward (anchoring logic)
       → NO:  Keep it planted on the ground
  5. Draw everything with glow effects
```

---

## 💡 Things You Can Try Changing

Open the file in any text editor (like Notepad or VS Code) and look for these numbers near the top:

```javascript
const NUM_SEGMENTS = 18;   // ← more segments = longer body
const SEG_LEN = 22;        // ← bigger = more stretched out
const NUM_LEGS = 8;        // ← try 6 or 12!
const STEP_DIST = 55;      // ← smaller = legs step more often
const BODY_FOLLOW = 0.12;  // ← bigger = faster (max 1.0)
const SLITHER_AMP = 6;     // ← bigger = more wiggly
```

---

## 🙋 About This Project

Made with help from **Claude AI** (by Anthropic) using a prompt about procedural animation and inverse kinematics.

I'm 13 years old and this is one of my first creative coding projects. If you think it's cool, give it a ⭐ star!

---

## 📜 License

Free to use, remix, and share. Just credit the original if you post it somewhere! 😊
