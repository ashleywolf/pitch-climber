# :mountain: Pitch Climber

Sing, hum, or scream your way up a cliff. Your voice pitch controls your altitude. Falsetto required by level 3.

## [Play Now](https://ashleywolf.github.io/pitch-climber/) (Chrome/Edge)

## What Is This

A voice-controlled climbing game. Hum low to hover near the ground. Go high to ascend. Hold a specific pitch to lock onto a ledge. The game auto-detects your vocal range in a 5-second warm-up, then builds difficulty around what your voice can actually do.

## Features

- Autocorrelation pitch detection translating your voice into altitude in real-time
- Easy, Normal, and Hard difficulty with auto-detection (warm-up calibrates your range)
- Momentum and inertia physics so your climber doesn't teleport between notes
- Tuning indicator showing how close you are to the target pitch
- Wind audio that scales with altitude (louder near the top)
- Randomized ledge pitches each playthrough so memorization won't save you
- Enhanced death sequence when you fall (it hurts to watch)
- localStorage high scores tracked per difficulty

## How to Play

- Allow mic access. Do the 5-second warm-up (just make some noise).
- Hum, sing, or yell to control altitude. Higher pitch = climb. Lower pitch = descend.
- Hit and hold the target pitch to grab a ledge. Ledges glow when you're close.
- Reach the top without falling to clear the level.

## Tech

- Web Audio API with AnalyserNode and autocorrelation-based pitch detection
- Real-time frequency analysis of microphone input
- 5-second calibration pass to map your personal vocal range
- HTML5 Canvas rendering with parallax cliff background

## Browser Support

Chrome or Edge recommended. Requires microphone access. Works best in a quiet room where the mic picks up your voice cleanly.

## Part of Browser Party Games

8 single-file browser games built with MediaPipe, Transformers.js, Web Audio, and Web Speech. No servers, no build steps, no installs.

| Game | Input | Tech |
|------|-------|------|
| [Type or Die](https://ashleywolf.github.io/type-or-die/) | Keyboard | Vanilla JS |
| [Grin Sweeper](https://ashleywolf.github.io/grin-sweeper/) | Smile (webcam) | MediaPipe Face |
| [Show & Tell](https://ashleywolf.github.io/show-and-tell/) | Real objects (webcam) | Transformers.js DETR |
| [Pitch Climber](https://ashleywolf.github.io/pitch-climber/) | Voice pitch (mic) | Web Audio API |
| [Spell Caster](https://ashleywolf.github.io/spell-caster/) | Shout spells (mic) | Web Speech API |
| [Stone Face](https://ashleywolf.github.io/stone-face/) | Don't react (webcam) | MediaPipe Face |
| [Ninja Hands](https://ashleywolf.github.io/ninja-hands/) | Hand tracking (webcam) | MediaPipe Hands |
| [Duck & Cover](https://ashleywolf.github.io/duck-and-cover/) | Duck + yell (webcam+mic) | MediaPipe Pose + Web Audio |

---
Built with vanilla JS + browser ML. Each game is one HTML file. Fork it, break it, make it yours.
