# 🕵️ UNDERCOVER
### A Social Deduction Party Game

---

## What is it?

Undercover is a party game where most players share the same secret word, but one or more **spies** have a slightly different word — and **Mr. White** has no word at all. Everyone gives clues, and the group tries to figure out who's lying.

Built as a single HTML file. No app install, no internet required (word bank is built-in), works on any phone browser.

---

## How to Play

### 1. Setup
- Toggle players **IN** or **OUT** (default roster is pre-loaded)
- Add new players with the **＋** button
- Set how many **Undercover** and **Mr. White** roles you want
- Optionally pick a **theme** (Food, Animals, Sports, Movies, Places, Tech) or type your own

### 2. Word Reveal
- Pass the phone to each player **one by one**
- Each player taps to privately see their word
- **Civilians** see the real word
- **Undercover** sees a *similar but different* word — they don't know they're undercover
- **Mr. White** sees a blank screen with no word

### 3. Discussion Round
- Players speak in a **random shuffled order** (Mr. White is never first)
- Each player gives **one clue** about their word — vague enough not to expose yourself, specific enough to signal you know the word
- Tap **✓ [NAME] DONE** after each person, or tap **⚡ SKIP — EVERYONE DONE** to move on faster

### 4. Vote
- The group discusses who they think is the spy
- Tap the player the group agrees to eliminate
- Confirm the vote

### 5. Elimination
| Who was eliminated | What happens |
|---|---|
| 👥 **Civilian** | **"SHIT."** — wrong person, spy still loose |
| 🕵️ **Undercover** | **"GOTCHA BADMAN! 🎉"** — spy caught |
| ⬜ **Mr. White** | Gets one chance to **guess the civilian word** |

- If Mr. White **guesses correctly** → Mr. White wins
- If Mr. White **guesses wrong** → eliminated, game continues

### 6. Repeat
Rounds continue until someone wins.

---

## Win Conditions

| Winner | Condition |
|---|---|
| 👥 Civilians | All Undercover and Mr. White players eliminated |
| 🕵️ Undercover | Special roles equal or outnumber civilians |
| ⬜ Mr. White | Eliminated but correctly guesses the civilian word |

---

## Default Players



Displayed alphabetically. Toggle anyone out before starting.

---

## Word Generation

- When played on **Claude.ai** — AI generates a fresh word pair every game (unlimited variety)
- When hosted elsewhere — falls back to a built-in bank of **100+ word pairs** across 7 categories
- Either way, no two rounds repeat the same pair until all pairs are exhausted

---

## Hosting

### Option 1 — Netlify Drop (easiest)
1. Go to [netlify.com/drop](https://netlify.com/drop)
2. Drag and drop `undercover_game.html`
3. Share the link — done

### Option 2 — GitHub Pages
1. Create a new GitHub repository
2. Upload `undercover_game.html`, rename it to `index.html`
3. Go to **Settings → Pages → Deploy from branch → main**
4. Your link: `https://yourusername.github.io/repo-name`

### Option 3 — Just share the file
Upload to Google Drive and share the link. Others download and open in their browser — works fully offline.

> **Note:** AI word generation only works on Claude.ai. On self-hosted versions it uses the built-in word bank automatically.

---

## Tips for a Fun Game

- **Civilians:** Be specific enough to show you know the word, but not so obvious you hand it to the spies
- **Undercover:** Your word is similar — use that similarity to blend in
- **Mr. White:** Listen hard to the first few clues and try to piece together the word before your turn
- Best with **5–10 players** and **1–2 undercover** roles
- Add **Mr. White** for an extra layer of chaos

---

## Tech Stack

- Pure HTML + CSS + JavaScript — single file, zero dependencies
- Google Fonts (Bebas Neue, Space Grotesk)
- Anthropic Claude API for word generation (with offline fallback)
