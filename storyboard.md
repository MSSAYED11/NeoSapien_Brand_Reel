# Neo One reel: storyboard (for approval)

1080x1920, 30 fps. Duration = voiceover 51.27 s + 2.0 s logo hold = **53.27 s (1598 frames)**, set by `calculateMetadata` from the audio file.
All times below come from `src/timing.ts` (Whisper word timestamps matched to the 12 script lines). Frames are shown for reference only; the code reads milliseconds from timing.ts and converts with the composition fps.

Global, every scene: #0A0A0A background, Inter (weights 500 and 600 only), 4 to 6 % film grain overlay, soft radial vignette, slow push-in 1.00 to 1.06 across each scene, all easing `cubic-bezier(0.16,1,0.3,1)` or springs with damping 200. Safe zone x 72 to 1008, y 260 to 1500. Hero text 160 px, secondary 64 px, labels 48 px. Glows are pre-baked radial gradients, never animated CSS blur.

Transition legend: **push** = soft push up with 20 % parallax, 15 f. **ftb** = fade-through-black, 18 f. **match** = no cut, elements re-flow in place.

---

## Scene 1: Hook. `0.00 to 10.38 s` (f0 to 311). Script lines 1 and 2

**Layout.** Empty stage. A 2 px #8A8A8A horizontal timeline at y 1120, from x 72 to 1008, with a short vertical tick at 70 % (the deadline). A 12 px #F5F5F2 marker dot sits at the left end. Hero text block at y 760, left-aligned to the 72 px margin, two lines max.

**Text.**
- 4.54 s ("missing"): **"Missed"** rises in.
- 4.96 s ("deadlines"): **"deadlines."** in #00DF79 rises in 5 f later.
- 8.06 s ("missing"): block 1 shrinks to 64 px #8A8A8A and slides up 140 px. **"Missed"** rises in at the hero position.
- 8.56 s ("pointers"): **"pointers."** in #00DF79.

**Motion.**
- 0.34 s: timeline draws left to right over 20 f.
- 0.70 s ("businesses") to 4.96 s: the marker travels along the line with a decelerating ease and crosses the deadline tick exactly at 4.96 s. The tick flashes #00DF79 for 10 f and stays green. The marker continues 80 px past it and settles.
- 8.56 s: a second, smaller marker 40 px below the line drifts right and fades (pointers slipping past).
- Push-in 1.00 to 1.06 across the scene.

**Accent budget.** Two green words plus the tick. Well under 10 %.

**Out.** 10.38 s: **push** to Scene 2 (15 f).

---

## Scene 2: Workflows. `10.38 to 15.70 s` (f311 to 471). Script line 3

**Layout.** Three outlined chips stacked vertically, centred, 88 px tall, fill #1A1A1A, 1 px border rgba(245,245,242,0.10), 24 px radius, 56 px Inter 500, 32 px gap. Stack centre y 900. Eyebrow label at y 640: "Everyone has a workflow", 48 px #8A8A8A.

**Text.**
- 12.02 s ("workflows"): eyebrow fades in.
- 12.54 s: chip **"AI notes"**.
- 13.20 s: chip **"Handwritten minutes"**.
- 14.86 s: chip **"An assistant"**.
- Each chip springs up 40 px with opacity. Stagger is driven by the voiceover, not fixed frames.

**Motion.** 15.44 s ("notes"): chips and eyebrow dim to #8A8A8A text and 50 % border over 12 f, staggered 5 f. The stack scales to 0.96. No green in this scene.

**Out.** 15.70 s: **ftb** (18 f). Scene 3 opens on black.

---

## Scene 3: Neo One reveal. `15.70 to 23.28 s` (f471 to 698). Script lines 4 and 5

**Layout.** Black stage, centre y 880. The "n" arc is a stroked SVG path, 180 px wide, 16 px stroke, #00DF79, matching the glyph on the device. Device (neo1-front.png) 620 px tall, centred, with a pre-baked radial green glow behind it (900 px, peak alpha 0.35). Hero text "Neo One" 160 px Inter 600 at y 1380.

**Text.** 21.74 s ("One"): **"Neo One"** fades up (18 f, 20 px rise). Only text on screen.

**Motion.**
- 17.58 s ("but"): the arc starts drawing (stroke-dashoffset) and completes at 20.48 s ("gadget"), about 3 s, slow and deliberate. A faint green point glow (alpha 0.15) sits behind it from the start.
- 20.48 to 21.44 s: arc holds, glow breathes once.
- 21.44 s ("Neo"): arc fades out over 8 f while the device rises from 160 px below, opacity 0 to 1, 24 f, spring damping 200. The device's own white-blue "n" lands where the green arc was: a match-on-shape reveal.
- 21.60 s: light sweep, a 160 px wide diagonal white band at 12 % alpha masked to the device, passes left to right over 20 f.
- 21.44 to 23.28 s: push-in 1.00 to 1.06 on device and glow. Glow breathes 0.25 to 0.35 with a 2.4 s period.

**Accent budget.** The arc, then the glow. Device image untouched.

**Out.** 23.28 s: **match**. No cut. The device scales to 300 px and moves to y 620 over 18 f while Scene 4 builds around it.

---

## Scene 4: Capture. `23.28 to 30.10 s` (f698 to 903). Script lines 6 and 7

**Layout.** Device small at top centre (y 620) with a 1 px #D9D9D9 waveform line across the full width behind it. Four agenda cards (glass: #1A1A1A, 1 px 10 % white border, 440 x 120 px, 48 px #D9D9D9 labels) in a 2 x 2 grid at y 900 to 1100. A memory ring at y 1340: 260 px circle, 2 px #8A8A8A stroke, with a pre-baked green glow behind it that is off until 29.70 s. Text block at y 1480, 64 px Inter 500 #F5F5F2.

**Text.**
- 26.56 s ("captures"): **"Captures everything"**.
- 28.64 s ("saves"): cross-fades (12 f, 16 px rise) to **"Saved to memory"** with "memory" in #00DF79.

**Motion.**
- 23.74 s ("meeting"): waveform line draws across the width.
- 24.62 s ("four") to 25.60 s: cards spring in, staggered 5 f, labelled "Agenda 1" to "Agenda 4" in grey.
- 26.56 s ("captures"): waveform amplitude ramps 0 to 28 px and a bright segment travels through the device, which brightens with a 6 f glow pulse.
- 28.64 s ("saves"): cards leave the grid one by one (stagger 6 f), shrink to 0.4 and fly along curved paths into the ring, fading as they enter.
- 29.70 s ("memory"): ring stroke turns #00DF79 and the green glow behind it fades in to alpha 0.3 and holds.
- Push-in across the scene.

**Accent budget.** Ring, glow, one word.

**Out.** 30.10 s: **push** (15 f).

---

## Scene 5: Recall. `30.10 to 35.42 s` (f903 to 1063). Script line 8

**Layout.** Eyebrow at y 560: "Next meeting", 48 px #8A8A8A. Three glass cards stacked, 936 x 180 px, #1A1A1A fill, 1 px 10 % white border, 28 px radius, centred, stack centre y 980. Each card: label 64 px Inter 500 #F5F5F2 at left, 56 px tick circle at right (grey outline, later green fill with an animated check path).

**Text.**
- 30.58 s ("next time"): eyebrow.
- 32.84 s: card **"Commitments"**.
- 33.40 s: card **"Follow-ups"**.
- 34.10 s: card **"Deadlines"**.
- Each slides up 80 px with opacity, spring damping 200.

**Motion.** 35.16 s ("automatically"): the three ticks draw in (stroke path, 10 f each), staggered 5 f, circles fill #00DF79. A faint green underglow fades in behind the stack at alpha 0.12. Push-in across the scene.

**Accent budget.** Three ticks and a faint glow.

**Out.** 35.42 s: **ftb** (15 f).

---

## Scene 6: Creator. `35.42 to 48.50 s` (f1063 to 1455). Script lines 9 to 11

The longest scene, three beats on one stage.

**Layout.** Top band (y 320 to 700): the system diagram. Device (neo1-side.png, 240 px tall) at x 260. A 2 px connector line from the device to a chip at x 760. Chip **"Claude"** (text only, 56 px, #1A1A1A, 1 px 10 % white border). A small **"MCP"** label chip (48 px, outlined, #8A8A8A) hangs below the line's midpoint. Middle (y 800 to 1200): a glass skill card 936 x 400, #1A1A1A, 1 px border. Card header: "Skill" eyebrow 48 px #8A8A8A, title 64 px Inter 600 #F5F5F2, then a typing line (48 px, #D9D9D9) with a blinking 2 px caret. Bottom (y 1400): hero block, 120 px Inter 600, two short lines.

**Beat A, 35.42 to 38.18 s (line 9).**
- 37.52 s ("creator"): a single centred line at y 960, **"As a creator"**, 64 px #D9D9D9, fades in. At 38.18 s it rises to the eyebrow position and fades to 40 %.

**Beat B, 38.18 to 42.76 s (line 10).**
- 38.54 s ("connected"): device slides in from the left, 60 px, with opacity.
- 39.00 s: connector line draws from device to chip position over 14 f.
- 39.38 s ("Claude"): **"Claude"** chip springs in at the line's end.
- 39.86 s ("MCP"): **"MCP"** label chip drops in under the line. The line tints #00DF79 for 12 f then settles to #D9D9D9.
- 40.28 s ("connector"): one green pulse travels along the line, device to Claude.
- 41.28 s ("skill"): skill card rises in, 80 px, 20 f.
- 41.98 s ("Sindhu") to 42.76 s: title types out **"Sindhu's second brain"**, about 22 characters over 0.8 s.

**Beat C, 42.76 to 48.50 s (line 11).**
- 43.38 s ("write") to 45.14 s: the typing line types a muted placeholder, "Hook: why clients leave", grey, caret blinking at 1 Hz. It stops at 45.14 s ("Claude") and the caret keeps blinking.
- 45.14 s: a second green pulse travels from the Claude chip back to the device.
- 46.22 s ("tone"): hero line 1 **"Your tone."** rises in at y 1400 with "tone" in #00DF79. The "As a creator" eyebrow fades out here to keep at most two text blocks on screen.
- 48.12 s ("context"): hero line 2 **"Your context."** rises in beneath it.
- Push-in 1.00 to 1.06 across the whole scene.

**Accent budget.** Two pulses on the line, one green word per hero line. Chips stay grey.

**Out.** 48.50 s: **push** (15 f).

---

## Scene 7: CTA and hold. `48.50 to 53.27 s` (f1455 to 1598). Script line 12, then silence

**Layout.** **"neosapien.ai"** 120 px Inter 600 at y 860, "neosapien" in #F5F5F2 and ".ai" in #8A8A8A. Device (neo1-front.png) 360 px tall at y 1180 with a pre-baked green glow behind it (alpha 0.25). Nothing else. Vignette slightly stronger at the edges.

**Text.** 48.98 s ("neosapien"): **"neosapien.ai"** fades in with a 20 px rise over 18 f. No green on text.

**Motion.**
- 48.98 s: device fades up from scale 0.9 with the text.
- 50.92 s ("get this"): one soft light sweep across the device, 20 f.
- 51.27 s: voiceover ends. From here to 53.27 s nothing moves except the glow, which breathes alpha 0.20 to 0.30 with a 2.0 s period and ends mid-cycle so the last frame is calm.

**Accent budget.** Glow only.

---

## Open questions before I write code

1. Scene 1 has about 4 s before the first on-screen word (the voiceover's "deadlines" is at 4.96 s). I have filled it with the marker travelling toward the deadline. If you want a text hook sooner, I can put "Missed" up at 0.70 s instead.
2. Scene 4 card labels: "Agenda 1" to "Agenda 4", or four short real words (for example "Budget", "Launch", "Hiring", "Pricing")?
3. Scene 6 typing placeholder: "Hook: why clients leave". Keep, or supply a line?
4. Inter is assumed. Geist is also available via @remotion/google-fonts if you prefer.

---

## Build notes (as implemented)

- Scenes 3 and 4 are one component, `RevealCaptureScene`, so the device is continuous through the match cut.
- Each soft push starts exactly on the script-line boundary and runs 15 f into the next line. The outgoing scene's last beat (memory ring, ticks, "Your context.") therefore completes before it is pushed away.
- The two fade-to-black cuts carry a short tail past the boundary (to 16.40 s and 36.02 s) so the dim-down and the ticks finish before black. The next scene is black until its first cue anyway.
- Reveals begin on the exact cue frame, so at the spoken word the element is at opacity 0 and fully in 0.6 s later. If you prefer visuals to lead the voice, a 3-frame lead in `src/reel/anim.ts` is a one-line change.
- Grain is a dark 512 px noise tile screened over the frame at ~5 % and jittered per frame. It also dithers the vignette and glow gradients, which band otherwise on #0A0A0A.
