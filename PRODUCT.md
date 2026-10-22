# Tangga Curi Poin - Game Show Trivia Indonesia

## Purpose & Mechanism
Tangga Curi Poin is an interactive, live trivia game show host application designed for group competition (4 vs 4 or 5 vs 5 team battle arena) in Indonesian. The core mechanism is the "Anak Tangga Petunjuk" (Clue Ladder): a trivia question has 4 sequential clues that get progressively easier while the point reward decreases (400 pts -> 300 pts -> 200 pts -> 100 pts). Teams compete to buzz in, risk points early, or steal points from the opponent.

## Platform & Operating Context
- **Platform:** Web (responsive single-page application, runs locally or deployed statically).
- **Mode:** Operate & Experience (Live host dashboard displayed on primary screen or projected to contestants/audience).
- **Stack:** Pure HTML5, Tailwind CSS, Google Fonts (Plus Jakarta Sans, Cabinet Grotesk), Lucide/Phosphor/Heroicon SVG icons, Web Audio API for sound synthesizer.

## Primary Roles & Workflows
1. **Host / Game Master:** Operates round controls, clue reveals, buzzers/timers, score updates, host secret answer key, and round transitions via tactile buttons or keyboard shortcuts (`1`, `2`, `X`, `N`, `T`, `H`, `Space`).
2. **Contestants (Tim Merah & Tim Biru):** Compete for points, attempt early gambits on vague clues, or steal upon opponent lockout.
3. **Audience / Viewers:** Follows the dramatic ladder reveal, countdown timer tension, and real-time score swings.

## Key Capabilities & Features
- **Header Console:** Round tracker ("Babak X dari Y"), host answer peek toggle, sound toggle, question bank manager, rules/help modal, fullscreen toggle.
- **Battle Arena Scoreboard:** Tim Merah vs Tim Biru scores, manual adjustments (+100/-100/+50/-50), active turn indicator, lockout status badges.
- **Center Stage:** Round category banner, active turn status, circular countdown timer (15s) with Mulai/Reset/+5s controls.
- **Anak Tangga Petunjuk (Clue Ladder):** 4 tiered clue cards (400, 300, 200, 100 Pts), public answer card, host secret drawer.
- **Host Control Bar:** BENAR TIM MERAH, BENAR TIM BIRU, SALAH/LOCKOUT, Buka Clue, Buka Jawaban, Babak Baru.
- **Question Manager & Custom Import:** Pre-loaded Indonesian trivia questions across diverse categories, JSON import/export, custom question additions.
- **Audio Synthesizer:** Pure Web Audio API generated sound effects (Timer tick, Correct chime, Buzzer/lockout, Level reveal, Victory fanfare).
