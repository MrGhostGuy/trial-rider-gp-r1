# Trial Rider GP — R1 Edition (v3)

A Trials-style physics moto game built for the Rabbit R1's 240×282 screen.
Ride at **https://mrghostguy.github.io/trial-rider-gp-r1/** or scan the creation
code on your R1 (Creations → Create → "add via QR code").

## What's in v3

- **Career mode** — 3 tracks (Training Grounds, Rocky Quarry, Summit Ridge) with
  checkpoints, medals (faults add +5s), best times and unlock progression.
- **Skill games** — Long Jump, Flip Frenzy (backflips off a big kicker, 75 seconds,
  loop resets each attempt) and Hill Climb (a procedurally generated hill that
  steepens to a wall — new layout every attempt).
- **Real trials obstacles** — working seesaws that tip as you cross, loose barrels
  you can knock around (they spawn in slightly different spots each run), and
  bounce-tyre zones.
- **Garage** — bike frame, rider suit and helmet colours, saved on the device.
- **Synth engine audio** and sound effects (mutable in Settings).

## Controls (R1)

- **Scroll wheel** — lean. Scroll one way to lean back, the other to lean forward.
  Tune it under Settings → Scroll/Lean Sensitivity (Low / Normal / High / Max),
  and flip the direction there too if it feels backwards.
- **Side button** — quick restart to the start of the track.
- **GAS / BRAKE** — on-screen pedals. In the air, GAS pitches you back and BRAKE
  pitches you forward.
- **⏸ button** — pause menu (resume, restart, settings, quit).

Desktop keys: W/↑ gas, S/↓ brake, A/D or ←/→ lean, R restart, Esc pause.

## Physics

Position-based two-wheel physics at 240 Hz with render interpolation: analogue
ramped throttle, frame-axis lean torque (works at any bike angle — that's what
makes backflips possible), air control, landing-impact absorption, wheelie/stoppie
balance, spin/speed safety caps and a "paddle assist" that unsticks you if you're
wedged at full throttle. Headless auto-driver verified: all 3 tracks finish with
0 faults, Long Jump ~10.8 m, Hill Climb ~84 m, Flip Frenzy scores full backflips.
