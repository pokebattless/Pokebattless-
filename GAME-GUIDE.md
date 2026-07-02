# Game Guide

A quick walkthrough of PokeBattles' screens and flow.

## 1. Home Screen

The landing screen shows the animated PokeBattles logo, a live online-player counter, and a menu grid to choose a game mode: **Ranked**, **Casual**, **History**, and **Leaderboard**.

## 2. Matchmaking / Lobby

Selecting a battle mode queues you into matchmaking. Once an opponent is found, you'll see a lobby entry showing both trainers before the battle begins.

## 3. Battle Screen

- **HP Panels** — top bars show your active Pokémon and the opponent's, with animated HP drain.
- **Move Buttons** — choose a move each turn; damage is calculated using type effectiveness.
- **Battle Log** — a scrolling log narrates each action, including AI-generated commentary.
- **Hit Effects** — particles and floating damage numbers play on each hit.

## 4. Result Screen

After the battle ends, a results overlay shows Victory/Defeat, KO counts, and (in Ranked mode) points gained or lost.

## 5. Match History & Leaderboard

Past matches are saved to a history list, and the leaderboard section shows top-ranked trainers.

## Architecture Notes

The entire app lives in a single `index.html` file:

- **CSS** (inline `<style>`) — theming, layout, animations
- **HTML** — one `.screen` element per app "page", toggled via `showScreen()`
- **JavaScript** (inline `<script>`) — game state object `G`, battle logic, DOM rendering, and the `aiNarrate()` function that calls the Claude API for dynamic commentary
