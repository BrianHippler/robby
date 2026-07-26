# R.O.B.B.Y. — Bill of Materials

| Component | Purpose | Why chosen |
|---|---|---|
| Raspberry Pi Zero 2W | Core compute / SBC | Small form factor fits base-bottom cavity; enough headroom for V1 voice/servo logic and future V2 API calls |
| MG90S / MG92B micro servos | Physical movement (per original R.O.B. joint layout) | Small size fits scaled model; sufficient torque for lightweight 3D-printed parts |
| ReSpeaker microphone array | Voice command input | Multi-mic array handles noisy real-world environments (household use) far better than a single mic |
| Small powered speaker | Audio output / responses | Compact, low-power, fits alongside base electronics |
| RabbitEngineering R.O.B. STL (thing:1494964), scaled ~266% | Structural reference / mechanical housing | Closest available reference to the original NES R.O.B. form factor; base redesigned from scratch since source SCAD wasn't available |

*Status: sourcing/salvage in progress — some components being pulled from a prior canned project. List will expand as CAD and wiring are finalized.*
