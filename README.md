# Quantum Mo — Pocket Quantum Circuit Lab

Drag quantum gates onto a 2-qubit circuit and watch superposition, phase and entanglement happen live — real state-vector math, running 100% in your browser. No backend, no API key, no build step.

**Live demo:** https://artzdesignmo.github.io/quantum-mo/

![Quantum Mo — Bell pair circuit with live Bloch spheres](screenshot.png)

## Features

- **Drag-and-drop circuit builder** — 9 gates (H, X, Y, Z, S, T, Rx, Ry, CNOT), tap-to-place fallback for touch screens
- **Live quantum readouts** — state vector with phase-coloured amplitudes, measurement probabilities, per-qubit Bloch spheres (drag to spin)
- **Entanglement meter** — concurrence of the 2-qubit state, from separable to maximally entangled
- **Time scrubber** — drag the step slider (or hit ▶) to watch the state evolve gate by gate
- **1000-shot sampler** — measure the final state 1000 times, histogram included
- **Recipes** — one-tap presets: quantum coin, Bell pair, phase dance, bit flip, plus 🎲 random circuits
- **Shareable circuits** — every circuit encodes into the URL hash; copy-link included
- **Gate glossary** — every gate's matrix and a plain-language explanation, EN/繁中
- **Learn cards** — qubit, superposition and entanglement explained for beginners
- **Export** — Bloch spheres as PNG, circuit as JSON
- Single `index.html`, vanilla JS + Canvas 2D, zero dependencies, works fully offline

## The math

- 2-qubit state vector of complex amplitudes, `index = q0 + 2·q1`
- Single-qubit gates applied as 2×2 unitaries; CNOT flips q1 iff q0 = 1
- Bloch vectors from the partial trace; entanglement via concurrence `C = 2|ad − bc|`

## Honest framing

Quantum Mo is an **educational simulator of ideal qubits**. It runs the real linear algebra — but it is not a real quantum computer, and it never claims to be. (Concept demo per project policy: no real-function claims.)

## Run

Open `index.html` in any modern browser. That's it.

## Part of OpenX

Quantum Mo is Project 13 of the [OpenX series](https://openx-mo.vercel.app/) — an open-source lab by [artzdesignmo](https://github.com/artzdesignmo). MIT licensed.

## Support

These open-source Mo projects are built in the open and free to use.
If one of them saved you time or made you smile, you can support the next build:

**[Buy Me a Coffee — @whynotartmoney](https://buymeacoffee.com/whynotartmoney)**

Support is optional and never gates any feature — every project stays MIT-licensed and fully offline.
