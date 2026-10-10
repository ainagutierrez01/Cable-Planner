# Cable Planner

**A browser-based tool for planning audiovisual (AV) cabling, placing equipment on floor plans, and calculating cable requirements.**

Cable Planner lets you design AV installations visually, connect equipment ports, estimate cable lengths using a calibrated floor plan, and export the resulting plan and cable summary to PDF.

Built with **HTML, CSS, and vanilla JavaScript**, it runs directly in your browser without a build step, backend, or additional dependencies.

## Features

### 📐 Floor Plan & Scaling
- **Import floor plans:** Upload PNG, JPEG, or WebP images as your installation layout.
- **Calibrate real-world scale:** Mark two reference points (A and B), enter the known distance in metres, and use it to calculate cable lengths.
- **Manual scale adjustment:** Set the scale in metres per grid square or reset it when needed.
- **Resizable workspace:** Drag the canvas resize handle to expand the planning area. Use the arrow keys for fine adjustments, or double-click the handle or press `Home` to reset it.

### 🔌 Equipment & Connector Catalogue
- **Search the Harman catalogue:** Find equipment by model, brand, or part number, such as `SRX910LA` or `M4250`.
- **Add compatible equipment:** Place catalogue models with known connector configurations directly onto the floor plan.
- **Create custom equipment:** Define your own devices by name, connector type, and number of ports (1–16).
- **Configure multiple connector types:** Assign additional connector types to individual devices.

Supported connector types include:

| Category | Connectors |
| --- | --- |
| Audio | XLR (male/female/combo), Speakon NL2/NL4/NL8, 1/4" TRS, RCA, 3.5 mm, Euroblock, Phoenix 3.5/5.08 mm, speaker terminals, binding post |
| Network | EtherCON, Ethernet RJ45, SFP/SFP+, QSFP28 |
| Video & other | BNC, USB-A, USB-C |
| Power & control | PowerCON, DMX 3-pin and 5-pin (male/female) |

### 🔗 Connections & Cable Lengths
- **Port-to-port connections:** Connect equipment by selecting ports directly on the canvas.
- **Automatic length calculation:** Calculate required cable lengths from the calibrated floor plan scale.
- **Live cable summary:** View the cables required by the current design as connections are added or modified.

### 🗄️ Rack Management
- Group equipment into racks to organise your installation.
- Rename racks to match your project requirements.
- Reorder devices within a rack using move-up and move-down actions.
- Remove individual devices or ungroup a rack using the canvas context menu.

### 📥 Design Import
Import an existing equipment list from an Excel (`.xlsx`) or CSV file.

Before importing, review a preview table showing:
- Equipment models and quantities.
- Detected connector configurations.
- Catalogue match status.

This lets you inspect equipment matches before placing devices on the plan.

### 📄 PDF Export
Export your design as a PDF containing the floor plan and cable summary, with the project name used to identify the document.

