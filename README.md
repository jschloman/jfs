# Overview

I've got a few projects going.  Here's some info on what's going on.

# Retro Arcade

> **6 polished classic games. Custom high-definition avatars. One codebase. Works at 30,000 feet.**

A cross-platform mobile game suite for iPhone (iOS) and Android, built with React Native + Expo. Fully offline, no accounts, no ads — just timeless casual games rebuilt with smooth animation, clean design, and a personal stats system.

---

## The Games
All six core titles are fully playable, featuring unique win animations, persistent state, and tailored difficulty settings.

| Game | Type | Key Details |
| :--- | :--- | :--- |
| **Klondike Solitaire** | Card | Draw-1 and draw-3 modes. |
| **FreeCell** | Card | All 32,000 solvable deals. |
| **Snake** | Arcade | 3 speed modes. Swipe or D-pad controls. |
| **Minesweeper** | Puzzle | Easy / medium / hard grids. Safe first tap. |
| **2048** | Puzzle | Standard 4×4. Persistent best scores. |
| **Sudoku** | Puzzle | 4 difficulty tiers. Note mode included. |

---

## Key Features

### 🎭 High-Definition Avatars & Outfits
The character system features high-fidelity **448 x 768 pixel avatars** designed to look sharp on modern mobile displays.
* **Custom Outfits:** Users can choose from a variety of outfits to personalize their player profile. 
* **Profile Integration:** Your active avatar appears in the home screen header, stats dashboard, and win screen celebration.

### 📊 Precision Stat Tracking
A fully offline record book that tracks your progress with granular detail.
* **Score Segregation:** Performance is tracked individually by **avatar** and **outfit**, allowing you to see which "look" brings you the most luck. 
* **Shared Stats:** Total games played, win rate, and all-time streaks across all profiles.
* **Per-Game Data:** Specific metrics like "Fewest Moves" in Solitaire or "Highest Tile" in 2048.

### ✈️ True Offline-First UX
Designed to pass the "airplane mode test."
* **Zero Loading:** All assets are bundled at build time for instant access.
* **Instant Resume:** Game state is written to MMKV on **every move**. If you take a call or force-quit, you'll be exactly where you left off.
* **Privacy by Design:** Your data stays on your device—no accounts or third-party cloud dependencies.

---

## Technical Stack
This project serves as a showcase for high-performance React Native development.

* **Framework:** React Native + Expo (Single TypeScript codebase).
* **Animations:** Reanimated 3 (UI-thread execution for 60fps gameplay).
* **Graphics:** React Native Skia (GPU-accelerated canvas loop for Snake).
* **Storage:** MMKV (High-speed storage for millisecond-perfect state saving).
* **Theming:** Dark mode inherits automatically from the System OS.

---

## 🚀 Roadmap: Coming Soon

### P2P Leaderboard (via Gun.js)
We are currently developing a decentralized, serverless leaderboard.
* **No Central Server:** Uses **Gun.js** to sync scores between devices via P2P.
* **Self-Hosted Relays:** Users will be able to host their own lightweight Node.js relay to sync with friends.
* **Privacy-First:** No SaaS, no Firebase, and no third-party tracking.

---
*Built for the love of the arcade. Designed for people. Works anywhere.*
