# MAKESPEC — Parametric Fabrication Specification Engine

An isolated, client-side application architecture configured to process unstructured natural language design briefs into structural fabrication specifications, material requirements, sequentially indexed assembly procedures, and real-world parametric 3D layout approximations.

---

## Technical Architecture Overview

The system operates entirely within a decentralized client-side runtime, bypassing central intermediate processing layers to optimize operational privacy and data integrity.

### Core Pipelines
* **Generative Telemetry Layer:** Manages context state machines to seamlessly convert arbitrary text strings into rigidly constrained payload schemas targeting the Google Gemini generative inference runtime array.
* **Asynchronous JSON Invariant Constraints:** Enforces strict upstream serialization controls using direct client bindings to eliminate parsing anomalies and sanitize unstructured text nodes at the inference boundary.
* **Local Cryptographic Profile Segregation:** Implements a localized state persistence driver that utilizes isolated browser storage partitions. Users can switch between unique identity context profiles without cross-contaminating validation tokens or access credentials.
* **Parametric Spatial Layout Engine:** Parses derived dimension strings natively to generate relative 3D viewport representations using a Three.js WebGL canvas workspace rendering engine.

---

## Operational Constraints and Safeguards

### System Warnings: What NOT to do
> **CRITICAL VIOLATION:** Do not expose confidential API authentication arrays to third-party script fragments, public diagnostic hooks, or external tracking architectures.
> 
> **EXECUTION INTERRUPT:** Do not clear volatile browser storage arrays or hard-refresh the application scope while an active streaming content-generation pipeline sequence is executing.
> 
> **BUFFER OVERFLOW RISK:** Do not input raw file buffers, image asset matrices, or multi-megabyte string blocks into the primary description fields. The interface is optimized exclusively for semantic structural text parsing.

---

## Implementation and Deployment Deployment Matrix

### Prerequisites
* An active, authorized API key provided by the **Google AI Studio** orchestration console.
* A modern, standards-compliant web browser environment supporting **WebGL rendering contexts** and **LocalStorage allocations**.

### Standard Setup Procedures

1. **Local Initialization**
   Clone the workspace index container and navigate to the root path:
   ```bash
   git clone [https://github.com/](https://github.com/)Ed13s/makespec.git
   cd makespec
   ```

---

## Circuit Diagrams and Code Generation

For projects with electronics, the generated spec now includes:

* **Wiring diagram** (Circuit & pinouts tab): components laid out around the main controller with colour-coded, routed wires, a connection table (hover a row to highlight its wire), and a one-click `.svg` download. Per-part pinouts are listed below it.
* **Code** (Code tab): a complete starter program with pins declared as named constants that match the circuit, plus optional extra files, required libraries and compile/upload steps. Copy or download each file, or grab everything as a `.zip`.

Both come from the same model response, so ask for changes in the Request Changes box (e.g. "use MicroPython instead" or "move the LED to GPIO 5") and the circuit and code update together. The wiring is AI-generated, so check it against the datasheets before powering anything.

---

## 3D Models, Exploded View and Printable Parts

The 3D layout tab was rebuilt for clarity and accuracy:

* **Real shapes, not placeholder blocks.** Each part is built from several solids (box, rounded box, plate with holes, open tray, cylinder, cone, tube, sphere, hemisphere, torus), so a dev board shows its PCB, shield can, USB port and headers, and an enclosure shows its walls and screw holes. The prompt also gives the model a table of real-world sizes for common parts.
* **Clear rendering.** Edge outlines, soft shadows, a light studio background and a grid whose squares are labelled in millimetres. Hover for dimensions, click a part (or its label or card) to isolate it.
* **Proper exploded view.** Parts are spaced out along the axis they install on, with dashed guide lines and leader-line labels, like a technical exploded diagram. Use the Assembled/Exploded buttons or the Spacing slider. Older specs without explode data get an automatic spread along the assembly's longest axis.
* **Printable vs visual-only.** Below the model, parts to print are listed separately from visual-only components (bought, owned or cut from stock). Each has a thumbnail and size. Only printable parts get STL downloads, exported Z-up and flat on the print bed, as single files, as one printable assembly, or as a zip.
* **Better controls.** Orbit, pan (right-drag or Shift-drag), zoom, touch gestures, and Iso/Front/Side/Top view buttons.

Saved specs from earlier versions still load.

---

## Send circuits to WireFrame

The Circuit & pinouts tab has buttons for [Ed13S/WireFrame](https://github.com/Ed13S/WireFrame), a schematic editor:

* **Open in WireFrame** opens WireFrame in a new tab and imports the circuit as a new project (real parts, pins matched by name or number, unused pins marked no-connect, checks run).
* **Copy for WireFrame** copies the circuit as JSON, to paste into WireFrame's AI Assistant (Make a circuit, reply box).
* **WireFrame address** changes where "Open" points (default `https://ed13s.github.io/WireFrame/`).

The importer lives in WireFrame (`makespec.js`), so that needs to be deployed too.
