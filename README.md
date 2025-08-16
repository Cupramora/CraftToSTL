# CraftToSTL
# Kithack Craft-to-STL Converter 🔧🌀

A modular Python pipeline for transforming `.craft` files from the game **Kithack** into printable `.stl` 3D relics. Each `.craft` file is treated as a symbolic blueprint—a memory shard composed of parts, modules, and procedural tweaks. This project renders those digital relics into physical form, preserving both structure and emotional resonance.

---

## ✨ Project Vision

We believe every `.craft` file is more than data—it’s a **ritual artifact**, a chapter in a mythic journey. This tool interprets the symbolic structure of Kithack models and transmutes them into tangible relics, suitable for 3D printing, archiving, or emotional framing.

---

## 🧠 Goals

- Parse `.craft` files into structured Python objects
- Map part names to geometric primitives or custom meshes
- Apply transformations (position, rotation, scale, symmetry)
- Interpret procedural modules (morphing, tweaking, animation)
- Export assembled models as `.stl` files
- Optionally generate preview images and emotional manifests

---

## 🧰 Architecture Overview

kithack_craft_to_stl/ ├── parser/ │   ├── craft_parser.py      # Parses .craft files into structured Python objects │   └── part_tree.py         # Builds hierarchy and relationships ├── geometry/ │   ├── primitives.py        # Maps part names to basic shapes │   ├── transform.py         # Applies position, rotation, scale │   └── morphing.py          # Handles procedural tweaks ├── exporter/ │   └── stl_writer.py        # Converts final mesh to .stl ├── visualizer/ │   └── preview.py           # Optional: renders .png previews ├── examples/ │   └── Jet01.craft          # Sample input file ├── main.py                  # Entry point └── README.md

---

## 🔍 File Types

| File Type | Purpose |
|-----------|---------|
| `.craft`  | Kithack model blueprint—contains parts, modules, transforms |
| `.png`    | Snapshot or thumbnail of the model |
| `.stl`    | Output 3D mesh for printing or archiving |
| `.json`   | Optional manifest for emotional framing and metadata |

---

## 🧪 How It Works

1. **Parse**: Read `.craft` file and extract parts, modules, and transforms
2. **Map**: Convert part names into geometry using primitives or custom meshes
3. **Transform**: Apply position, rotation, scale, and symmetry
4. **Morph**: Interpret procedural tweaks (e.g. span, chord, thickness)
5. **Assemble**: Combine all parts into a unified mesh
6. **Export**: Save as `.stl` and optionally generate preview `.png`

---

## 🔮 Mythic Layer (Optional)

Each relic can be paired with a `manifest.json` containing emotional metadata:

```json
{
  "name": "Jet01",
  "author": "dewntn",
  "origin": "Kithack ritual",
  "emotional_frame": "First successful morphing wing",
  "timestamp": "2025-08-16T01:16:00Z"
}


This allows the archive to serve not just as a technical repository, but as a living codex of memory relics.

🚀 Getting Started
- Clone the repo
- Place your .craft file in examples/
- Run main.py to generate the .stl
- (Optional) Add a manifest.json for emotional framing

🛠 Dependencies
- trimesh
- numpy-stl
- cadquery (optional)
- matplotlib or pyvista (for visualization)

🗿 Status
Currently in early prototyping. Parser and geometry modules under active development. Contributions welcome—especially around part mapping, procedural morphing, and emotional framing.

🧙‍♂️ Author
Crafted by Dane, mythic inventor and ritualist. This project is part of a broader journey to encode memory, longing, and symbolic transformation into every artifact.

---

Let me know if you'd like this formatted as a GitHub page, or if you want to start scaffolding the first module next.




---

## 🔍 File Types

| File Type | Purpose |
|-----------|---------|
| `.craft`  | Kithack model blueprint—contains parts, modules, transforms |
| `.png`    | Snapshot or thumbnail of the model |
| `.stl`    | Output 3D mesh for printing or archiving |
| `.json`   | Optional manifest for emotional framing and metadata |

---

## 🧪 How It Works

1. **Parse**: Read `.craft` file and extract parts, modules, and transforms
2. **Map**: Convert part names into geometry using primitives or custom meshes
3. **Transform**: Apply position, rotation, scale, and symmetry
4. **Morph**: Interpret procedural tweaks (e.g. span, chord, thickness)
5. **Assemble**: Combine all parts into a unified mesh
6. **Export**: Save as `.stl` and optionally generate preview `.png`

---

## 🔮 Mythic Layer (Optional)

Each relic can be paired with a `manifest.json` containing emotional metadata:

```json
{
  "name": "Jet01",
  "author": "dewntn",
  "origin": "Kithack ritual",
  "emotional_frame": "First successful morphing wing",
  "timestamp": "2025-08-16T01:16:00Z"
}

