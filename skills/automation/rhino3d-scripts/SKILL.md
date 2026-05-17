---
name: 'rhino3d-scripts'
description: 'Authoring and debugging scripts for Rhinoceros 3D (Rhino 8 and later). Use when asked to write RhinoScript (VBScript / .rvb / .vbs), RhinoPython, or RhinoCommon-based scripts; automate Rhino modeling'
version: 1.0.0
source: awesome-copilot
tier: 2
adopted: 2026-05-16
---

# rhino3d-scripts

'Authoring and debugging scripts for Rhinoceros 3D (Rhino 8 and later). Use when asked to write RhinoScript (VBScript / .rvb / .vbs), RhinoPython, or RhinoCommon-based scripts; automate Rhino modeling

## When to Use

- Use this skill when working on tasks related to rhino3d scripts
- Trigger when you need expertise in this domain
- Apply best practices from awesome-copilot

## Workflow

name: rhino3d-scripts
description: 'Authoring and debugging scripts for Rhinoceros 3D (Rhino 8 and later). Use when asked to write RhinoScript (VBScript / .rvb / .vbs), RhinoPython, or RhinoCommon-based scripts; automate Rhino modeling tasks; build command macros; manipulate Rhino geometry, layers, blocks, or document objects; pick objects from the viewport; control redraw and undo; or load and run scripts from the Rhino Script Editor. Covers `rhinoscriptsyntax`, `scriptcontext`, the `Rhino.*` RhinoCommon namespaces (`Rhino.Geometry`, `Rhino.DocObjects`, `Rhino.Input`, `Rhino.UI`, `Rhino.Display`, `Rhino.FileIO`), and the Rhino 8 unified Script Editor.'
# Rhino 3D Scripting Skill
Write production-quality scripts for Rhinoceros 3D. Covers the three scripting surfaces (RhinoScript/VBScript, RhinoPython, direct RhinoCommon .NET) and the Rhino 8+ Script Editor.
## When to Use This Skill
- User asks to write, edit, or debug a `.rvb`, `.vbs`, or `.py` Rhino script
- User wants a Rhino **command macro** or wants to automate a sequence of Rhino commands
- User wants to manipulate geometry, layers, blocks, materials, viewports, or annotations from code
- User mentions `rhinoscriptsyntax`, `scriptcontext`, `RhinoCommon`, `Rhino.Geometry`, `RhinoDoc`, or the Script Editor
- User wants to pick objects, prompt for input, or build a small UI inside Rhino
- User asks how to load, run, or distribute a script (startup scripts, aliases, toolbar buttons)
## Choosing a Scripting Surface
Pick the surface based on the task, not preference. Recommend Python by default for new work.
| Surface | When to choose | File ext |
|---|---|---|
| **RhinoPython** (`rhinoscriptsyntax` + RhinoCommon) | Default for new scripts. Best ecosystem, readable, full RhinoCommon access. | `.py` |
| **RhinoScript** (VBScript) | Maintaining legacy `.rvb`/`.vbs` files; integrating with VBA/COM. | `.rvb`, `.vbs` |
| **RhinoCommon (C#/.NET) via Script Editor** | Performance-critical loops, complex geometry, leveraging .NET libraries. | `.cs` |
| **Command macro** | Pure sequence of existing Rhino commands; no logic. | toolbar/alias |
A macro is **not** a script — it is a string of command-line input (e.g. `! _-Line 0,0,0 10,0,0 _Enter`). Use a script the moment you need a variable, loop, or conditional.

## Source

This skill was adopted from open-source repository: awesome-copilot
Original path: rhino3d-scripts
