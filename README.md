MemoryForge is an AI‑assisted layout engine that turns a list of concepts into a **spatial design** for a VR memory palace. Instead of hard‑coding rooms and objects inside a game engine, you describe your topics in a CSV, and MemoryForge suggests where each idea should live in 3D space.

## What it does

- Groups related topics into **virtual rooms**.
- Assigns each concept a **3D coordinate**:
  - Room index → which room.
  - Left/right offset → lateral position.
  - Height → difficulty level.
- Produces:
  - A top‑down **floor‑plan plot**.
  - A **3D scatter plot** you can treat as a VR “blueprint”.
  - Text descriptions of where to place each concept on walls in VR.

## Input format

Upload or place a CSV named `memoryforge_topics.csv` with columns:

- `topic` – concept name.  
- `group` – logical group or chapter (used as room).  
- `importance` – 1–5 scale (higher = more central).  
- `difficulty` – 1–5 scale (higher = placed higher in space).

An example file is included in this repo.

