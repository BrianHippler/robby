# R.O.B.B.Y.
### Robotic Operating Buddy Born Yours

A voice-controlled desktop robot companion, inspired by the NES R.O.B. peripheral, 
being built for my daughter. R.O.B.B.Y. is a local-first, privacy-by-design AI 
hardware project — combining mechanical design, embedded electronics, and (eventually) 
a custom-trained conversational model.

**Status: Active build — V1 in progress.** This repo is a real build log, not a 
finished product. Expect it to grow messily and honestly over time.

---

## Project Structure

- **`/CAD`** — Fusion 360 design files for R.O.B.B.Y.'s physical housing
- **`/Code`** — Voice input, servo control, and orchestration logic (not yet started)
- **`/Parts`** — Bill of materials and component sourcing
- **`/Docs`** — Roadmap, architecture notes, and design rationale

## Roadmap

### V1 — Physical Build *(current)*
A R.O.B.B.Y. that physically moves in response to voice commands.

- Reference model: scaled/modified version of a mini R.O.B. design (see Attribution), 
  scaled to ~266% (~240mm total height)
- Base redesigned from scratch in Autodesk Fusion, using the original STL as a mesh 
  reference for tracing geometry
- Electronics split across two housings to solve a space-constrained base:
  - **Base bottom:** Raspberry Pi Zero 2W
  - **Base top:** micro servos, mounted via the model's existing pillar structure
- Core components: Raspberry Pi Zero 2W, MG90S/MG92B micro servos, ReSpeaker mic 
  array, small powered speaker

See [`Docs/roadmap.md`](Docs/roadmap.md) for full detail.

### V2 — Conversational AI Layer
Natural language conversation via an AI/API layer, gated behind a multi-layer safety 
architecture (system prompt constraints, input/output filtering, logging, model 
selection) — since this will be used by a child, scope is being finalized jointly 
before build begins.

### V3 — Custom Fine-Tuned Model
Fine-tuning a small open-source model to replace third-party API dependency. Dual 
purpose: a personal deep-dive into LLM training, and the technical foundation for a 
privacy-first, parent-controlled AI companion concept — local inference, no cloud 
dependency by design.

## Parts & Components

See [`Parts/BOM.md`](Parts/BOM.md) for the full bill of materials and sourcing notes.

## Attribution

The mechanical base reference for R.O.B.B.Y. was originally designed by 
**RabbitEngineering**, published on Thingiverse as 
["Mini Nintendo R.O.B."](https://www.thingiverse.com/thing:1494964), 
licensed under **Creative Commons — Attribution — Non-Commercial (CC BY-NC)**.

Original files are not redistributed here. R.O.B.B.Y.'s base is being redesigned 
from scratch in Autodesk Fusion, using the original model as a mesh reference only.

## About

Built by [Brian Hippler](https://github.com/BrianHippler) — Navy veteran, 
cybersecurity student, and builder of local-first AI/edge projects.
