🧠 NEUROPHAGE — Sector 13
Dr. Heinrich was dying, so he injected himself with his own experimental serum.It worked — and it changed him. Crimson skin. Horns. A hunger for brains.You are Max. You are locked in the dark with him.Don't let him hear you run.

NEUROPHAGE is a top-down stealth-horror escape game that runs entirely in yourbrowser — one HTML file, zero dependencies, zero asset files. Every sprite is drawnpixel-by-pixel in code, every sound is synthesized live with the Web Audio API, and themonster has a real brain: he hears you, predicts you, remembers you, and checks theshadows you duck into.

🎮 Gameplay
Sneak through 12 sectors of a sealed laboratory. Each sector is a self-containedobjective — collect research notes, find keycards, solve a blood-sigil terminal, crafta blade, sabotage security, survive lockdowns — all while the Doctor patrols thedark. He can't be killed. He can be distracted, stunned, avoided… and in the end,cured.

🕶️ Hide in shadow zones — but if he saw you hide, he'll walk straight to that shadow
🔊 Noise is real — sprinting rings the dinner bell; walking is nearly silent
🔪 Craft the blade — one stun window, then run
💉 The finale — synthesize the antidote and inject it while he's chasing you
✨ Features
🧠 Smart AI	5-state brain (patrol → investigate → chase → hunt → search) with BFS pathfinding, predictive intercept, line-of-sight checks, noise memory, objective guarding & stuck-recovery
🌑 Dynamic lighting	Flashlight cone, flickering & failing lights, full blackout sectors
🔊 100% synthesized audio	Ambient drone, proximity heartbeat, chase drums, roars, growls, crafting sparks — no audio files
🎨 Code-generated pixel art	Animated player, a hand-built pixel demon (walk / attack / stunned sets), CRT scanlines, blood decals, particles, screen shake
🎚️ 3 difficulty modes	Easy / Medium / Hard scale monster speed, hearing, prediction, damage, timers, puzzle rounds & stamina
🗺️ Convenience UI	Live minimap, awareness "eye", objective arrow, contextual prompts, skippable intros
💾 Persistence	Sector progress + difficulty saved to localStorage; age check per session
📱 Touch support	Virtual joystick + action buttons on mobile
🚫 Zero dependencies	No frameworks, no builds, no downloads — open the file and play
🕹️ Controls
Key	Action
WASD / Arrows	Move
SHIFT	Sprint (loud — drains stamina)
E	Interact / hold to inject the cure
F	Blade stun (once crafted)
ESC	Pause
M	Mute
1–9	Blood Sigil terminal input
Any key	Skip sector intro
⚙️ Difficulty
Easy	Medium	Hard
Monster speed	78%	100%	115%
Hearing radius	65%	100%	135%
Chase prediction	low	medium	high
Damage per hit	8	14	20
Sprint recovery	fast	normal	slow
Guards objectives	never	sometimes	often
🧩 The 12 Sectors
01 Awakening · 02 Blackout · 03 Lockdown · 04 The Sigil · 05 Scrap & Steel06 Confrontation · 07 The Antidote · 08 Sabotage · 09 Power Surge10 Mirror Halls · 11 The Gauntlet · 12 The Cure

🚀 Run it
Download index.html (the whole game is that one file)
Open it in any modern browser — Chrome, Edge, Firefox, Safari
Enter your age (9+ recommended; the game checks) → pick a difficulty → survive
🎧 Headphones strongly recommended — the heartbeat, footsteps and chase drumsare half the horror.

👹 Optional: drop any monster.png next to index.html and it's used as themonster automatically. Delete it and the built-in pixel demon takes over.

🛠️ Tech & Architecture
Rendering: HTML5 Canvas 2D, imageSmoothingEnabled=false for crisp pixels
Lighting: offscreen "darkness" layer with destination-out punched lights, cached radial sprites
AI: grid-based 8-direction BFS (pre-allocated arrays, zero per-frame allocation), corner-cut prevention, path string-pulling
Performance: pre-rendered floor/wall/minimap layers, persistent blood-stain canvas, cached gradients
Audio: pure Web Audio API oscillators + filtered noise buffers
Storage: localStorage (progress, difficulty) · sessionStorage (age check)
No frameworks. No build step. ~1 file.

📄 License
MIT — do whatever you like, attribution appreciated.

Walk. Always walk.
