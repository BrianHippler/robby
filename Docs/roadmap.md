# R.O.B.B.Y. — Roadmap

**R.O.B.B.Y.** (Robotic Operating Buddy Born Yours) is a voice-controlled desktop robot companion, inspired by the NES R.O.B. peripheral, built for my daughter. The project is structured in three versions, each adding a layer of sophistication — physical build, then AI conversation, then a custom-trained model.

## V1 — Physical Build (Current)
Goal: a R.O.B.B.Y. that physically moves in response to voice commands.

- **Reference model**: Scaled/modified version of RabbitEngineering's 13-part miniature R.O.B. design (Thingiverse thing:1494964), scaled to ~266% (~240mm total height)
- **CAD**: Designed from scratch in Autodesk Fusion, using the original STL as a mesh reference for tracing geometry (no editable source file was available)
- **Electronics layout**: Split across two housings to solve a space-constrained base —
  - Base bottom: Raspberry Pi Zero 2W (flat, ~9–12mm cavity)
  - Base top: micro servos, mounted using the model's existing pillar structure
- **Core components**: Raspberry Pi Zero 2W, MG90S/MG92B micro servos, ReSpeaker mic array, small powered speaker
- **Status**: Base bottom footprint modeled and extruded; base top geometry in progress (tracing from imported STL reference)

## V2 — Conversational AI Layer
Goal: natural language conversation via an AI/API layer.

- Multi-layer safety architecture required before deployment to a child:
  - System prompt constraints
  - Input filtering
  - Output filtering
  - Logging
  - Model selection
- Scope and safety framework to be finalized and approved jointly before build begins — this isn't a solo decision given it's for a child.

## V3 — Custom Fine-Tuned Model
Goal: fine-tune a small open-source model, replacing reliance on third-party APIs.

- Dual purpose:
  1. Personal learning milestone in LLM training/fine-tuning
  2. Foundation for a potential product concept: privacy-first, parent-controlled AI companions for children — local inference, no cloud dependency by design
- Educational foundation: Karpathy's "Let's Build GPT," 3Blue1Brown's neural network series, Sebastian Raschka's LLM course, freeCodeCamp's beginner LLM course

---
*This repo is an active, in-progress build log — not a finished product. Commits reflect real build sequence as components come together.*
