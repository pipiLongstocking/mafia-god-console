# Mafia God — Local-first Web App (Dark, Mobile-friendly)

## Overview
This project is a **dark-themed, mobile-friendly, local-first web app** that assists the game master ("God") in running the popular social deduction game **Mafia**. It solves common problems like remembering roles, tracking players, guiding night/day phases, and logging events.

## Key Features
1. **Role Reveal Center** — Private, mobile-optimized screen to show each player their role without leaking info to others.
2. **Role Randomization** — Automatically assign Mafia, Police, Doctor, and Villagers.
3. **Auto-suggest Role Mix** — Suggests a balanced role distribution based on player count.
4. **Alive/Dead Tracking** — Toggle player status.
5. **God Dashboard** — Color-coded list of players with their roles (God-only view).
6. **Night Phase Wizard** — Guides God through Mafia → Doctor → Police actions in correct order.
7. **Day Voting System** — Tally votes; in case of a tie or no-votes, the game proceeds without elimination.
8. **Logs** — Separate Night and Day logs, plus last-game recap.
9. **Custom Role Naming** — Rename "Police" to any role name and support multiple Doctors/Police.
10. **Role Balance Warnings** — Alerts if Mafia/Police count is unbalanced for the number of players.
11. **Local Storage Persistence** — Players, settings, and ongoing game state survive page refreshes.

## How to Use
1. **Setup Players**
   - Enter player names.
   - Set counts for Mafia, Police, Doctor (or use **Auto-suggest Roles**).
   - Click **Randomize Roles**.

2. **Role Reveal**
   - Switch to the **Role Reveal** tab.
   - Tap a player to reveal their role privately.

3. **Night Phase**
   - Follow step-by-step prompts to select Mafia victim, Doctor save, and Police check.
   - Resolve night actions to update statuses and logs.

4. **Day Phase**
   - Record each alive player's vote.
   - Tally votes — ties or no-votes mean no one is eliminated.
   - Confirm elimination if there’s a clear majority.

5. **Logs & Recap**
   - View Night and Day logs in real-time.
   - End the game to save a single recap of the last game.

## Running Locally

### Option 1: Open Directly
1. Save the `index.html` file locally.
2. Double-click to open in your browser.

### Option 2: Run a Local Server
**Python**
```bash
python3 -m http.server 8000
```
Visit: `http://localhost:8000`

**Node.js (npx serve)**
```bash
npx serve .
```
Visit the printed local URL.

**VS Code Live Server**
- Install the Live Server extension.
- Right-click `index.html` → **Open with Live Server**.

### Mobile Access
1. Start your local server.
2. Find your computer’s local IP (e.g., `192.168.1.20`).
3. On your phone, open `http://192.168.1.20:8000`.

---
**Enjoy running smooth, error-free Mafia games without forgetting a single detail!**

