# Trial Rider GP — R1 Edition (v7)

A Trials-style physics motorcycle game built for the Rabbit R1's 240×282 screen.

**Play:** https://mrghostguy.github.io/trial-rider-gp-r1/

## v7 — themed tracks, void crosses, rocket boost
- **Every track looks like its name** — Neon Foundry is now a neon city at night (glowing cyan track ribbon, lit skyline), Summit Ridge and Apex Ridge are snow-capped alpine, Midnight Foundry is dark steel with factory silhouettes, the quarries are bare rock. New per-track theme system drives ground, edge, strata and skyline decor.
- **Void crosses everywhere** — the old over-ground beam sections on every track became ramp-launched floating-platform crosses over open chasms with the terrain removed: fall short and you fault back to the checkpoint. Plus extra flow ramps on every track.
- **Rocket booster (Long Jump)** — one tank per attempt: hold B / Shift / the BOOST pedal. The speed governor makes room while it burns; the test bot jumps 8.6 m unboosted vs 16.0 m boosted. Long Jump also gets Flip Frenzy's curved kicker profile, and Hill Climb grows kicker lips every ~600 units.
- **More juice** — checkpoint sparkle bursts, finish confetti (bigger for gold), extra landing dust, boost flames, and a boost fuel gauge.

## v6 — ramps, floating platforms, lava
- **Wedge ramps (kickers)** — a new obstacle type that launches you onto platform lines.
- **Floating platform crosses** — Deep Quarry, Midnight Foundry and Apex Ridge each hide a lava pit crossed by tilted floating platforms (descending chains on T5/T6; T7 adds a step-up mid-chain). Touching the lava is a fault — checkpoints sit right before each cross, per classic Trials design.
- **Remix mode grows up** — remix runs now also scatter procedurally placed ramps and 3-platform floating lines over flat stretches, so remix laps genuinely reroute the track.
- Track design informed by research into Trials Fusion/Rising: platform chains where early platforms ride on momentum, hazards as the floor under crossings, checkpoints within sight of hard sections, ~75% throttle precision hops.

## v5 — more tracks, more reasons to replay
- **3 new career tracks, progressively harder and longer** — Deep Quarry (8.4 km of twin seesaws, log stairs and mud climbs), Midnight Foundry (seesaw-to-beam combos, a mover-bridged pit, twin walls) and Apex Ridge, a 12.4 km finale with a triple seesaw chain and every obstacle in the game.
- **Daily Climb** — Hill Climb seeded by the date: the same hill all day, a daily best, and fresh medal bolts every day.
- **Remix mode** (Settings) — career tracks shuffle their log and barrel placement every run; pays bolts, never touches your records or ghosts.
- **Achievements** — 8 trophies (First Finish, Gold Rush, Completionist, Flip Master, Mountain Goat…) paying bonus bolts, listed in the Garage.

## v4 — the big overhaul
- **New physics feel** — lighter gravity, floatier arc, suspension-soak landings (the bike crouches on big drops instead of slamming), stronger air control.
- **Trials tech** — bunny hop (flick lean back→forward, double-tap GAS, or K), wheelie holds, brake-pivot turns.
- **Real trials obstacles** — ride-over logs, pipes and tyres, balance beams over barrel pits, moving elevator platforms, mud patches that sap your drive, seesaws, loose barrels, bounce-tyre zones, wall steps.
- **Career tracks** — checkpoints, medals and finish-to-unlock progression.
- **Skill games** — Long Jump, Flip Frenzy (rebuilt kicker — backflips actually work now), Hill Climb (a new hill every run).
- **Bolts & crates** — medals pay bolts ⚙; spend them on cosmetic crates in the Garage. 22 unlockables across COMMON / RARE / EPIC / LEGENDARY with a pity guarantee (EPIC+ within 12 opens); duplicates refund bolts.
- **Ghost racing** — your best medal run on each track races beside you as a translucent ghost.
- **QoL** — live medal-pace readout in the HUD, checkpoint restart from the pause menu (or C), scrollable menus, ghost & effects toggles.

## Controls (R1)
- **Scroll wheel** — lean (sensitivity + flip direction in Settings)
- **Side button** — quick restart
- **GAS / BRAKE** pedals on screen; in the air, GAS pitches back, BRAKE pitches forward

Faults send you back to the last checkpoint and add +5s to your medal time.

## v8 — weight transfer, extreme tracks, boost you can SEE (2026-11-12)
- **Weight transfer physics**: gas loads the rear wheel (wheelies lift easier, hold longer), braking dives the front (stoppies, pivot turns) — and the rider's body visibly shifts on the bike. The camera look-ahead is hard-capped so boost speed no longer pushes the bike off-screen.
- **Rocket boost, visible edition**: three-layer flame jet (white-hot core), speed streaks, bigger flame particles, draining fuel gauge — frame-verified this time.
- **Two EXTREME tracks**: T8 VERTIGO FOUNDRY (14,200) and T9 NINJA RIDGE (16,800) — hop gaps you can't roll, step-up staircases, short-platform precision crosses, a mover over a void, a mud climb, a curved near-vertical wall. Advanced mechanics are mandatory; the test bot finishes both (with cooldown hop tech), and clean 0-fault runs are on record.
- **Detailed rider + bike**: suit with chest stripe, helmet peak, boots and gloves, engine block, exhaust with muffler, twin front forks, spoked hubs, number plate.
- **Crates grew**: 32 cosmetics — animated Galaxy Shift (LEGENDARY) and Molten Core frames, Demon Horns helm (with actual horns), Skull King, Neon Spectre, Void Rims, Inferno Rims, Lightning and Toxic trails.

## v9 — no more safety nets (2026-11-12)
- **Every floating platform now has real danger under it.** The audit found the big crosses were honest but plenty of smaller platforms still had track underneath: T6's beam floated 12 units over a bump, T7's beam had barrels parked under it, and five mover bridges (T2/T3/T5/T7) were decorative high lines you could ride under or fall off for free.
- **Conversions**: T2, T3 and T5 movers became ramp-launched floater crosses over chasms (350/360/280 wide — too far to jump, the platforms are the only way; negative-tested: remove the platforms and the test bot fault-loops forever). T6 and T7 beams became chasm crosses. T7's high mover line became a cross too.
- **Mover pits became fault pits**: T4, T6 and T7 mover bridges now span deepened pits with void floors — fall off the mover and you fault instead of riding out. Movers were widened so the exit is bridged, and T7's pit checkpoint moved out of the pit (7200 → 7140).
- **Remix lines too**: remix floater lines now get a launch ramp and a chasm cut under them at runtime (skipped only where a checkpoint, seesaw, mover or existing hazard sits in the span, so a respawn can never land you in a chasm).
- All 9 career tracks + skill games bot-verified again after the surgery.
