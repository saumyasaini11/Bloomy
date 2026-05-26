<div align="center">

# 🌸 Bloomy 🌸
### *Nurture your garden. Reach the bloom.*

<br/>

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white)
![Canvas API](https://img.shields.io/badge/Canvas_API-orange?style=for-the-badge&logo=html5&logoColor=white)

<br/>

> *"Every flower must grow through dirt. 🩷 Keep growing. Keep glowing!"*

</div>

---

## 🌱 What is Growth Journey?

**Growth Journey** (codename: *Bloomy*) is a cozy, pixel-art browser game where you play as a gardener tending a magical pot plant through **10 increasingly chaotic levels**. Catch sunlight ☀️ and water 💧, dodge vicious bugs 🐛 and sneaky decoys 🦋, and grow your plant from a tiny sprout all the way to a full bloom 🏵️ — all while competing for glory on a live leaderboard!

Built entirely in **vanilla HTML, CSS, and JavaScript** with a Canvas-based gameplay engine, a synthesized chiptune BGM, a Gachapon reward system, a cinematic intro, and a Supabase-powered online leaderboard — all packed into a **single `index.html` file**.

---

## ✨ Features

| Feature | Description |
|---|---|
| 🎮 **10 Unique Levels** | Each level introduces a new flower, character, and gameplay hazard |
| 🌦️ **Dynamic Hazards** | Wind gusts, rainstorms, night mode, drought, bug trails, and lumberjacks |
| 🐝 **Bee Helpers** | Friendly bees fly in and boost your plant growth |
| 🎡 **Gachapon Machine** | Spend coins to spin the gacha for exclusive flower unlocks |
| 🪙 **Coin Economy** | Earn coins by completing levels; spend them in the Gacha Shop |
| 🏆 **Live Leaderboard** | Powered by Supabase with real-time updates |
| 🎵 **Synthesized BGM** | Full chiptune soundtrack generated via the Web Audio API — no files needed |
| 📖 **Cinematic Intro** | A typewriter-style triptych story before the game begins |
| 🐱 **10 Unlockable Characters** | Each level reveals a unique pixel-art gardener character |
| 🌿 **Pot Skins** | Unlock and equip different pot styles (Clay, Gold, Pink, Ocean) |
| 📱 **Touch Friendly** | Full mobile/touchscreen support |
| 💾 **Progress Saving** | Auto-save via `localStorage` — pick up where you left off |
| 🎊 **Confetti Celebration** | Confetti rains down when you complete the full garden |

---

## 🎮 How to Play

```
1. 🌸  Enter your name on the Home Screen
2. 🗺️  Select a level from the World Map
3. 🕹️  Move your pot left/right to catch falling items
4. ☀️  Catch SUN tokens   → +15 pts, fills growth bar
5. 💧  Catch WATER drops  → +10 pts, fills growth bar faster
6. 🐛  AVOID bugs         → they drain your hearts (3 lives)
7. 🌱  Fill the growth bar to 100% to win the level!
8. 🎉  Unlock a new character and earn coins after every win!
```

### Controls

| Input | Action |
|---|---|
| `←` / `A` | Move pot left |
| `→` / `D` | Move pot right |
| `Touch / Drag` | Move pot (mobile) |
| `Escape` | Pause game |

---

## 🌍 The 10 Levels

```
Level 1  🌸  Cherry Blossom    —  Sleepy Napper         (Speed ×1.0)
Level 2  🌻  Sunflower Field   —  Froggy Blooms  💨      (Wind Gusts)
Level 3  🌷  Tulip Garden      —  Rosy Kitty     🌧️      (Rain Storm)
Level 4  🌺  Hibiscus Bay      —  Apple Paw      🐝      (Bee Helpers)
Level 5  🪷  Lotus Pond        —  Cottontail Zen 🌙      (Night Mode)
Level 6  🌹  Rose Valley       —  Midnight Paws  🐛      (Bug Trails + Slime)
Level 7  💐  Bouquet Meadow    —  Breezy Whiskers ✨     (Combo Power)
Level 8  🌼  Daisy Hills       —  Fluffy Tail    🦋      (Decoy Drops)
Level 9  🌿  Wildflower Way    —  Jam Bunny      🏜️      (Drought Mode)
Level 10 🏵️  Golden Bloom Peak —  Lovebird Legend 🌟     (ALL Hazards!)
```

---

## ⚔️ Hazards & Mechanics

### Falling Items
- ☀️ **Sun** — Safe! Gives 15 points and boosts growth
- 💧 **Water** — Safe! Gives 10 points and boosts growth even more
- 🐛 **Bug** — Dangerous! Costs 1 heart; leaves slime puddles in later levels
- 🦋 **Decoy Drop** — Looks like water… but isn't! (Level 8+)

### Environmental Hazards
- 💨 **Wind Gusts** — Items drift sideways; catch them before they fly off screen!
- 🌧️ **Rain** — Increases water items but reduces visibility
- 🌙 **Night Mode** — Dark overlay makes items glow; times your reactions
- 🏜️ **Drought** — Water becomes extremely rare; sun becomes plentiful
- 🐛 **Bug Trails** — Slime patches persist on the ground and drain HP over time
- 🪓 **Lumberjacks** — Pixelated villains march toward your pot swinging their axes!

### Combo System (Level 7+)
Chain 5+ catches in a row to trigger **COMBO x2** — your points double! 🔥

---

## 🎡 Gachapon System

After completing levels you'll earn 🪙 **coins**:

| Level | First Clear | Repeat |
|---|---|---|
| 1 | 50 coins | 12 coins |
| 2 | 75 coins | 18 coins |
| … | … | … |
| 10 | 500 coins | 125 coins |

Spend coins at the **Garden Gachapon** machine to unlock rare flower prints for your collection. Turn the knob, watch the capsule drop, and discover what's blooming inside! 🎉

---

## 🏆 Leaderboard

Growth Journey features a **real-time online leaderboard** powered by [Supabase](https://supabase.io). Your score, name, level reached, and unlocked character are submitted after completing the game.

> If no Supabase credentials are configured, the game falls back to a local `localStorage` leaderboard automatically.

### Setting up Supabase (optional)

1. Create a free project at [supabase.com](https://supabase.com)
2. Create a table called `scores` with these columns:

```sql
create table scores (
  id uuid primary key default gen_random_uuid(),
  name text,
  score integer,
  level_reached integer,
  character_unlocked text,
  timestamp timestamptz default now()
);
```

3. In `index.html`, fill in your credentials:

```js
const SUPABASE_URL = "https://your-project.supabase.co";
const SUPABASE_ANON_KEY = "your-anon-key-here";
```

---

## 🎵 Audio

The game features a **fully synthesized chiptune soundtrack** built using the **Web Audio API** — no external audio files needed for music! The relaxing ambient garden melody shifts between two harmonic phrases with a warm bass line.

Additional sound effects:
- `happy-happy-happy-cat.mp3` — Victory fanfare
- `oh-my-god-bro-oh-hell-nah-man.mp3` — Game-over reaction
- `mixkit-winning-a-coin-video-game-2069.wav` — Coin collection chime

---

## 🚀 Getting Started

Because Growth Journey is a single HTML file with no build step, getting started is effortless:

```bash
# Option 1: Just open it!
# Double-click index.html in your file explorer

# Option 2: Serve it locally for best results
npx serve .
# then visit http://localhost:3000
```

That's it. No `npm install`. No webpack. No dependencies. Pure browser magic. 🌿

---

## 📁 Project Structure

```
Bloomy-main/
│
├── index.html                          ← The entire game (HTML + CSS + JS)
│
├── char_l1.png  ...  char_l10.png     ← Pixel-art character unlock cards
├── lily.png                            ← Flower asset
├── lotus.png                           ← Flower asset
├── roses.png                           ← Flower asset
│
├── happy-happy-happy-cat.mp3           ← Win sound
├── oh-my-god-bro-oh-hell-nah-man.mp3  ← Game-over sound
├── mixkit-winning-a-coin-video-game-2069.wav  ← Coin sound
│
├── Judge Cat Reaction GIF.gif          ← Reaction GIF on hit
├── gif.gif                             ← Reaction GIF on decoy hit
│
└── Gemini_Generated_Image_*.png        ← Background image asset
```

---

## 🛠️ Tech Stack

| Technology | Usage |
|---|---|
| **HTML5 Canvas** | Core gameplay rendering — items, pot, plant, lumberjacks, particles |
| **Web Audio API** | Synthesized BGM + all SFX, zero audio file dependencies for music |
| **CSS Animations** | UI animations (bounce, float, sparkle, confetti, coin burst) |
| **LocalStorage** | Persistent save state — name, progress, coins, characters |
| **Supabase JS SDK** | Online leaderboard with real-time Postgres subscriptions |
| **Press Start 2P** | Google Font giving the whole game its retro pixel-art personality |
| **Vanilla JS** | 100% framework-free, runs natively in any modern browser |

---

## 🎨 Design Philosophy

Growth Journey was designed around a few core principles:

- 🌻 **Cozy but challenging** — The aesthetic is warm and garden-themed, but the difficulty ramps up hard by Level 8+
- 🧩 **Single file simplicity** — Everything lives in one `index.html`. No build tools, no bundler, just open and play
- 🎶 **Audio without files** — BGM is computed note-by-note using oscillators, making the game self-contained for the music
- 📱 **Mobile-first gameplay** — Touch drag controls are first-class citizens alongside keyboard controls
- 🏆 **Replayable by design** — The Gacha system and leaderboard give players a reason to come back and improve their score

---

## 🌼 Screenshots

> *Every flower must grow through dirt.* 🩷

The Home Screen features a warm gingham pattern, pixel-art stamp decorations, a live leaderboard preview, and a charming "How to Play" guide at the bottom.

The World Map is a hand-drawn canvas with a winding golden path connecting 10 animated level nodes — completed levels glow with sparkling flowers, locked levels are shrouded in animated gloom clouds.

---

## 🤝 Contributing

Got ideas for new levels, hazards, or characters? PRs and issues are welcome!

1. Fork the repo
2. Edit `index.html` directly
3. Test in your browser
4. Open a Pull Request with a description of what you changed

---

## 📄 License

This project is open source. Use it, remix it, grow something beautiful with it. 🌸

---

<div align="center">

Made with 💚 and way too much caffeine

**🌱 → 🌿 → 🌸 → 🏵️**

*Plant seeds. Water daily. Help grow. Earn stars.*

</div>
