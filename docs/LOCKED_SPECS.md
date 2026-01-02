# Locked Specs (Jan 30, 2026 Build)

These specs are **locked** for the Mid-Winter Conference build. If something isn’t listed here, it’s not required for Jan-30.

## Build Goal
A **silent-movie** style auto-playing chase scene:
- gavel runs
- cowboy chases
- lasso misses (scripted), near-hit (sometimes), final escape (fundraiser beat)
- freeze-frame + intertitle cards
- resets cleanly

## Display Target
- 1920×1080
- 30 FPS (OBS Browser Source or Chrome full screen)
- Offline / local assets only

## Visual Layer Stack (Bottom → Top)
1. **Background** (static): 1920×1080  
2. **Dust / ground FX** (optional): small puffs under feet/hooves (cut first if risky)  
3. **Gavel sprite** (star): 200×200 frames  
4. **Cowboy + horse**: 400×400 frames  
5. **Lasso rope overlay**: 600×400 arc layer  
6. **UI / text overlay** (intertitle cards + title)  
7. **Freeze-frame effect** (pick ONE effect only)

## Sprite Frame Counts (Locked)
### Gavel (run/escape)
- **4 frames**
- 200ms per frame (~5 FPS)
- Stick legs: **allowed** (visual-only upgrade)

### Cowboy + horse (run/chase)
- **6 frames**
- 150ms per frame (~6.6 FPS)

### Lasso wind-up
- **2 frames**
- 250ms per frame (500ms total)

### Lasso throw
- **2 frames**
- 100ms per frame (200ms total)

### Rope arc
- **1 static arc** per attempt (no physics)

### Freeze frame
- **1.5 seconds**
- Effects: choose ONE (zoom OR shake OR flash)

### Reset
- Fade out: 0.5 seconds
- Snap back to start (no rewind animation)

## Outcome Probabilities (Locked)
These are stage-managed comedy beats (deterministic outcomes with minor visual randomness allowed).

### Attempt #1
- **Miss: 100%**
- Text: “SO CLOSE!”
- Gavel speeds up slightly after miss (+10% visual)

### Attempt #2
- Clean Miss: **70%**
- Near-Hit (graze): **30%**
- Text: “ALMOST!” or “THAT WAS CLOSE!”

### Attempt #3 (Jan-30 default: Fundraiser Mode)
- **Gavel Escapes: 100%**
- Freeze-frame text:
  - “GAVEL ESCAPED!”
  - “Donations Required”

## DO-NOT-SHIP (Before Jan-30)
- Phone stat entry
- Leaderboards / saving
- Network dependencies
- Sound effects / sync
- Physics-based collisions
- Config menus

## Allowed “Fake Randomness”
Randomize ONLY cosmetic elements:
- tiny timing offsets (±150ms)
- dust puff choice
- which run frame starts first
- slight rope arc variation (pre-baked)
