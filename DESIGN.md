# Visual Design System: Tangga Curi Poin (Neo-pop EdTech / Dribbble AI Quiz Reference)

## Visual World & Reference
Directly derived from Dribbble shot `Quiz Generating Website using AI` (ID: 27079968). A playful, high-energy Neobrutalist / Neo-pop visual world characterized by crisp dark outlines, solid tactile block shadows, soft rounded corners, pure white cards on an engineering grid canvas, and vibrant pop accent colors.

## Foundations

### Canvas & Background
- **Base Canvas:** `#FAFAFC` (subtle warm light off-white).
- **Grid Pattern:** Fine geometric graph paper grid:
  `background-image: linear-gradient(to right, rgba(24, 24, 27, 0.04) 1px, transparent 1px), linear-gradient(to bottom, rgba(24, 24, 27, 0.04) 1px, transparent 1px); background-size: 24px 24px;`
- **Surface Elevation:** Cards use pure white `#FFFFFF` with `border: 2.5px solid #18181B` and tactile offset drop-shadow `box-shadow: 4px 4px 0px #18181B`.

### Typography
- **Display & Headings:** `Plus Jakarta Sans` or `Cabinet Grotesk`, `font-extrabold` (800) and `font-black` (900), tracking `-0.025em`.
- **Body & Controls:** `Plus Jakarta Sans`, 500/600/700 weight, clear legibility with high contrast (`#18181B` on `#FFFFFF` / `#FAFAFC`).
- **Numerals:** Tabular figures (`tabular-nums`) for scores and countdown timers.

### Color Palette
- **Deep Ink (Borders, Text, Shadows):** `#18181B` (zinc-900 / dark ink).
- **Punch Magenta / Raspberry:** `#E94E77` (Hero pill highlight, Tim Merah, primary CTAs).
- **Electric Blue:** `#0EA5E9` (Tim Biru, secondary CTAs).
- **Sunny Amber / Gold:** `#F59E0B` (Timer ring, Clue 2 badge, stakes).
- **Fresh Lime:** `#10B981` (Clue 3 badge, success confirmation, online status).
- **Cool Indigo / Slate:** `#6366F1` / `#64748B` (Clue 4 badge, host drawer, utility badges).

### Distinctive Signature Motifs
1. **Highlight Pill:** Pink-magenta rounded capsule with white text, e.g. `[ AI Platform ]` from Dribbble, adapted for game status and clue points.
2. **Tilted Sticker Badges:** Dark or neon badges rotated slightly (`rotate-[-3deg]` or `rotate-[4deg]`) like real stickers ("LIVE SHOW ✦", "BABAK 1").
3. **Tactile Button Physics:** High-satisfaction tactile click states:
   - Rest: `border-2 border-black shadow-[3px_3px_0px_#18181b]`
   - Hover: `hover:shadow-[4px_4px_0px_#18181b] hover:-translate-y-0.5`
   - Active: `active:translate-x-[2px] active:translate-y-[2px] active:shadow-none`
4. **"Kind of Quizzes" Clue Card Layout:**
   - 4 Clue tiers laid out in a responsive grid or structured ladder.
   - Each card features a vibrant rounded icon square (Pink for 400, Amber for 300, Lime for 200, Indigo for 100).
   - High-contrast typography and clear visual hierarchy.
5. **Scoreboard Duel Cards:**
   - Left card for Tim Merah with red/pink accents, avatar badge, tactile +100/-100 buttons.
   - Center stage for Category & Circular Timer.
   - Right card for Tim Biru with blue accents, avatar badge, tactile score controls.
