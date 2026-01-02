# Jan-30 Runbook (Checklist + Fallback Plan)

## Success Criteria
- Runs full-screen reliably
- Readable from the back of the room
- Silent-movie pacing: action → intertitle → laugh beat
- Resets without reloading

---

## A) Asset Checklist
- [ ] Background: 1920×1080 PNG
- [ ] Gavel sprite: 4 frames @ 200×200
- [ ] Cowboy+horse sprite: 6 frames @ 400×400
- [ ] Lasso wind-up: 2 frames
- [ ] Lasso throw: 2 frames
- [ ] Rope arcs: static overlay(s)
- [ ] Text cards:
  - [ ] SO CLOSE!
  - [ ] ALMOST!
  - [ ] THAT WAS CLOSE!
  - [ ] GAVEL ESCAPED!
  - [ ] Donations Required

## B) Timing Checklist
- [ ] Gavel: 200ms per frame
- [ ] Cowboy: 150ms per frame
- [ ] Wind-up: 500ms total
- [ ] Throw: 200ms total
- [ ] Freeze: 1500ms
- [ ] Fade out: 500ms
- [ ] Total run: ≤ 15 seconds

## C) Logic Checklist
- [ ] Attempt #1 = miss (100%)
- [ ] Attempt #2 = miss (70%) or near-hit (30%)
- [ ] Attempt #3 = escape (100% for Jan-30)
- [ ] No network calls
- [ ] No user input required
- [ ] One-button start + one-button reset

## D) OBS Setup Checklist (if using OBS)
- [ ] Browser Source size: 1920×1080
- [ ] FPS: 30
- [ ] “Shutdown source when not visible” OFF
- [ ] “Refresh browser when scene becomes active” OFF
- [ ] Test scene switch does not reset animation unexpectedly

## E) Day-Before Checklist
- [ ] Run it 3 times in a row (no edits)
- [ ] USB backup copy of project
- [ ] MP4 fallback ready
- [ ] Static fallback slide ready
- [ ] HDMI/adapter/charger packed

---

# Fallback Failure Plan (No Panic Edition)

## Level 1: Minor glitch (stutter / timing odd)
Say: “Let’s see if the gavel gets lucky this time.”  
Action: restart. Keep moving. No apologies.

## Level 2: Won’t start (blank source / JS error)
Action: instantly switch to **Static Fallback Slide**  
Say: “The gavel escaped so fast the computer couldn’t keep up.”  
Proceed with fundraiser beat.

## Level 3: Total tech death (laptop/OBS/projector failure)
Say: “Just like last year… the gavel got away.”  
Proceed with fundraiser using real gavel / photo. Tech-free win.
