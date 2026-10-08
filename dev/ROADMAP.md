# rt-lang - Roadmap

> Path from scaffold to a stable 1.0. Hard parts are front-loaded; each phase has hard exit criteria.
> Master plan: ../_lexersketch/ROADMAP.md and ../_lexersketch/NEW-LIBS.md
>
> **Anti-deferral rule:** no listed hard task moves to a later phase unless this file records the move and the reason.

## v0.1.0 - Scaffold (DONE)
Compiles, CI green, structure correct, no domain logic.
- [x] Manifest, README, CHANGELOG, REPS, dual license, CI, deny, clippy, rustfmt, DIRECTIVES, ROADMAP.

## v0.2.0 - Foundation
- [ ] Runtime model and descriptors; platform layer interface; entry/exit and allocation as IR, testable on the VM first.
- [ ] Blocked on ir-lang 2.0 for the full runtime; recorded per the anti-deferral rule.

## v0.5.0 - Implementation
- [ ] Strings, panics/unwinding, threads, GC hooks; per-OS platform layers.

## v0.9.0 - Hardening
- [ ] Differential tests against the VM; fuzzing; ABI conformance per OS.

## v1.0.0 - Stable
- [ ] Frozen after Zero and a Kraken subset run natively on all three OSes (D18).
