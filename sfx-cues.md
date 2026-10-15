# Neo One reel: SFX cue sheet

For sound design in Premiere. Times are seconds from the start of the voiceover, which is frame 0 of the composition (30 fps). Every cue is driven by `src/timing.ts`; if the voiceover is re-cut, regenerate timing.ts and shift these accordingly.

Suggested palette: airy whooshes (short, filtered), soft sub hits (no click, 60 to 80 Hz), tiny UI clicks and ticks (glassy, dry), glass risers and shimmers for anything green, mechanical keyboard ticks for typing. Keep everything well under the voice. The reel is calm; most cues should sit at 10 to 20 % of the voice level.

Legend: **whoosh** = air movement for a slide or push. **sub** = low thump under a landing. **click** = short UI tap. **tick** = tiny mechanical or glass tick. **riser** = rising swell into a moment. **shimmer** = high, sparkly tail for light or green elements.

| Time (s) | Frame | Scene | Motion event | SFX |
| --- | --- | --- | --- | --- |
| 0.34 | 10 | 1 Hook | Timeline line draws left to right (20 f) | thin whoosh, very soft |
| 0.70 | 21 | 1 Hook | "Losing clients?" fades in; marker starts travelling | soft sub swell |
| 0.70 to 4.96 | 21 to 149 | 1 Hook | Marker travels toward the deadline tick | very low riser, optional |
| 3.60 to 4.20 | 108 to 126 | 1 Hook | Hook text fades out | none |
| 4.54 | 136 | 1 Hook | "Missed" rises in | soft whoosh |
| 4.96 | 149 | 1 Hook | Marker crosses the tick, tick flashes green, "deadlines." lands | sub hit + UI tick |
| 8.06 | 242 | 1 Hook | Block 1 shrinks and lifts; "Missed" rises in | soft whoosh (up) |
| 8.56 | 257 | 1 Hook | "pointers." lands; small marker drifts past below the line | soft sub, lighter than 4.96 |
| 10.38 | 311 | 1 to 2 | Soft push up to scene 2 (15 f) | airy whoosh |
| 10.92 | 328 | 2 Workflows | Eyebrow "Everyone has a workflow" fades in | none |
| 12.54 | 376 | 2 Workflows | Chip "AI notes" springs up | UI click |
| 13.20 | 396 | 2 Workflows | Chip "Handwritten minutes" springs up | UI click |
| 14.86 | 446 | 2 Workflows | Chip "An assistant" springs up | UI click |
| 15.44 | 463 | 2 Workflows | Chips dim to grey, stack settles back | soft reverse shimmer |
| 16.00 to 16.40 | 480 to 492 | 2 to 3 | Fade to black | low tail, let the room go quiet |
| 19.00 to 20.48 | 570 to 614 | 3 Reveal | Green "n" arc draws (ends on "gadget") | glass riser, resolving at 20.48 |
| 20.48 to 21.44 | 614 to 643 | 3 Reveal | Arc holds, glow breathes once | subtle hum |
| 21.44 | 643 | 3 Reveal | Arc fades, device rises into place (24 f) | sub hit + deep whoosh |
| 21.61 | 648 | 3 Reveal | Light sweep across the device (20 f) | shimmer sweep |
| 21.74 | 652 | 3 Reveal | "Neo One" fades up | soft whoosh |
| 23.74 to 24.34 | 712 to 730 | 3 to 4 | Match cut: device shrinks and moves to the top | whoosh (up), short |
| 24.21 | 726 | 4 Capture | Waveform line draws across | thin whoosh |
| 24.62 | 739 | 4 Capture | Card "Budget" springs in | UI click |
| 24.79 | 744 | 4 Capture | Card "Launch" springs in | UI click |
| 24.95 | 749 | 4 Capture | Card "Hiring" springs in | UI click |
| 25.12 | 754 | 4 Capture | Card "Pricing" springs in | UI click |
| 26.56 | 797 | 4 Capture | Waveform wakes; bright segment passes through the device; glow pulse; "Captures everything" | soft audio-texture riser + one soft pulse |
| 28.64 | 859 | 4 Capture | Card 1 flies into the memory ring; caption swaps to "Saved to memory" | short whoosh |
| 28.84 | 865 | 4 Capture | Card 2 flies in | short whoosh |
| 29.04 | 871 | 4 Capture | Card 3 flies in | short whoosh |
| 29.24 | 877 | 4 Capture | Card 4 flies in | short whoosh |
| 29.70 | 891 | 4 Capture | Ring turns green, glow fades up | soft chime + low sub |
| 30.10 | 903 | 4 to 5 | Soft push up to scene 5 (15 f) | airy whoosh |
| 30.58 | 917 | 5 Recall | Eyebrow "Next meeting" fades in | none |
| 32.84 | 985 | 5 Recall | Card "Commitments" slides up | soft UI slide |
| 33.40 | 1002 | 5 Recall | Card "Follow-ups" slides up | soft UI slide |
| 34.10 | 1023 | 5 Recall | Card "Deadlines" slides up | soft UI slide |
| 35.16 | 1055 | 5 Recall | Tick 1 draws, circle fills green | UI tick |
| 35.29 | 1059 | 5 Recall | Tick 2 | UI tick |
| 35.43 | 1063 | 5 Recall | Tick 3; faint green underglow | UI tick + sub hint |
| 35.75 to 36.02 | 1073 to 1081 | 5 to 6 | Fade to black | low tail |
| 37.52 | 1126 | 6 Creator | "As a creator" fades in | soft whoosh |
| 38.21 | 1146 | 6 Creator | Text lifts to eyebrow position | none |
| 38.54 | 1156 | 6 Creator | Side-view device slides in from the left | whoosh |
| 39.00 | 1170 | 6 Creator | Connector line draws toward the chip (14 f) | thin glide |
| 39.38 | 1181 | 6 Creator | "Claude" chip springs in | UI click |
| 39.86 | 1196 | 6 Creator | "MCP" label drops in; line flashes green | UI click + tiny shimmer |
| 40.28 | 1208 | 6 Creator | Green pulse travels device to Claude (14 f) | data blip / synth zip |
| 41.28 | 1238 | 6 Creator | Skill card rises; diagram dims to 40 % | soft whoosh |
| 41.98 to 42.76 | 1259 to 1283 | 6 Creator | Title types "Sindhu's second brain" | keyboard ticks, 21 chars |
| 43.38 to 45.14 | 1301 to 1354 | 6 Creator | Placeholder types "Hook: why clients leave" | keyboard ticks, softer |
| 45.14 | 1354 | 6 Creator | Reverse pulse Claude to device (14 f) | data blip |
| 46.22 | 1387 | 6 Creator | "Your tone." rises in | soft sub hit |
| 48.12 | 1444 | 6 Creator | "Your context." rises in | soft sub hit |
| 48.50 | 1455 | 6 to 7 | Soft push up to CTA (15 f); device fades up | airy whoosh |
| 48.98 | 1469 | 7 CTA | "neosapien.ai" fades in | shimmer + soft sub |
| 50.92 | 1528 | 7 CTA | Light sweep across the device | shimmer |
| 51.27 | 1538 | 7 CTA | Voiceover ends; glow starts breathing | music or pad tail only |
| 53.27 | 1598 | End | Last frame | everything out by here |

## Notes

- Scenes 3 and 4 are one continuous sequence in the build (the device never cuts), so there is no transition SFX at 23.28, only the match-cut whoosh as it shrinks.
- The three pushes start exactly on a script-line boundary and run 15 frames into the next line.
- The two fade-to-black cuts have a short tail past the line boundary (16.40 and 36.02) so the previous beat finishes. Keep any music swell off those tails.
- If you want a subtle music bed, the natural sections are 0 to 16.4 (problem), 16.4 to 30.1 (reveal and capture), 30.1 to 36.0 (recall), 36.0 to 48.5 (creator), 48.5 to end (CTA and hold).
