# 034 · LCR Dice

A fully-featured browser implementation of the classic dice game Left Center Right, built as part of the [AppADay](https://augustineiacopelli.github.io/appaday/) project.

## How to Play

Players sit in a circle. On your turn, roll one die per chip you hold (max 3 dice). Each die result moves chips:

- **L** — Pass one chip to the player on your left
- **C** — Place one chip in the center pot
- **R** — Pass one chip to the player on your right
- **·** (dot) — Keep your chip, nothing happens

If you have no chips, skip your turn but stay in the game — other players can still pass chips to you. The last player holding any chips wins the pot.

## Features

- **3–8 players** with custom names
- **Circular table layout** — players displayed clockwise around an overhead-view oval so left/right passing is visually intuitive
- **House Rules** (each individually toggleable):
  - **· · · Dot-Dot-Dot** — Roll all dots, collect 1 chip from every other player
  - **L–C–R Jackpot** — Roll one L, C, and R (any order), pay 2 chips in each direction in order until you run out
  - **L–L–L Triple Left** — Pay 6 chips left instead of 3
  - **R–R–R Triple Right** — Pay 6 chips right instead of 3
  - **C–C–C Triple Center** — Pay 6 chips to the pot instead of 3
- **Starting chips** — adjustable from 3 (traditional) to 15
- **Lifetime chip bank** — chip totals persist across games via localStorage; winners keep their winnings, losers never go below 0
- **Tutorial Mode** — post-roll breakdown modal showing every chip movement and new totals
- **Responsive** — portrait and landscape layouts for phone, tablet, and desktop

## Tech

Single-file vanilla HTML/CSS/JS. No frameworks, no dependencies, no build step. Deployable directly to GitHub Pages.

## Live

[augustineiacopelli.github.io/appaday/appaday-034-lcr-dice/](https://augustineiacopelli.github.io/appaday/appaday-034-lcr-dice/)

## Part of AppADay

Daily web app challenge — one complete, functional, mobile-friendly app every day.  
[View the full portfolio →](https://augustineiacopelli.github.io/appaday/)
