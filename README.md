# LV Switchboard — Approval Package (Mini Project)

This project represents a simplified Low-Voltage (LV) switchboard design and documentation package. It models a **600 V, 3-phase, 4-wire, 60 Hz switchboard** with a **2000 A main breaker** and **three feeder circuits**. The deliverables mirror what would be prepared for an engineering *approval set*.

## 📂 Project Structure

```
LV-Switchboard/
│
├── drawings/                   # Engineering drawings
│   ├── SLD-001.pdf             # Single-Line Diagram
│   ├── ELEV-001.pdf            # Front elevation with device tags
│   └── SCH-101.pdf             # Feeder control schematic
│
├── tables/                     # Auto-generated schedules
│   ├── BOM_v1.xlsx             # Bill of Materials
│   ├── WireList_v1.xlsx        # Wire list
│   ├── TerminalList_v1.xlsx    # Terminal strip schedule
│   └── Nameplates_v1.xlsx      # Equipment nameplate schedule
│
├── export/
│   └── LV_Switchboard_ApprovalSet_v1.pdf # Combined approval package
│
└── README.md
```

## 🎯 Scope Summary

| Parameter          | Value                                                                    |
| ------------------ | ------------------------------------------------------------------------ |
| Voltage            | 600 V AC, 3φ, 4W, 60 Hz                                                  |
| Main Bus Rating    | 2000 A                                                                   |
| Feeders            | 400 A, 225 A, 100 A                                                      |
| Protection Devices | MCCB main w/ electronic trip; MCCB feeders                               |
| Documentation      | SLD, elevation, control schematic, BOM, wire list, terminals, nameplates |

### Functional Intent

* Provide a representative **approval-stage submittal package** for an LV distribution board
* Demonstrate **design clarity, documentation standards, and engineering workflow**
* Include **automated table outputs** typically derived from electrical CAD tools

## ✅ Deliverables

| Category            | File                                       |
| ------------------- | ------------------------------------------ |
| Single-Line Diagram | `drawings/SLD-001.pdf`                     |
| Front Elevation     | `drawings/ELEV-001.pdf`                    |
| Feeder Schematic    | `drawings/SCH-101.pdf`                     |
| BOM                 | `tables/BOM_v1.xlsx`                       |
| Wire List           | `tables/WireList_v1.xlsx`                  |
| Terminal List       | `tables/TerminalList_v1.xlsx`              |
| Nameplates          | `tables/Nameplates_v1.xlsx`                |
| Approval Set        | `export/LV_Switchboard_ApprovalSet_v1.pdf` |

## ⚙️ Design Assumptions

* **Short-circuit rating:** Utility AFC assumed 50 kA @ 600 V
* **Board SCCR Target:** ≥ 65 kA
* **Conductors:** Copper THHN/THWN (initial sizing placeholder)
* **Grounding:** Per CEC Part I
* **Coordination Strategy:**

  * Main breaker with **adjustable electronic trip** element
  * Feeder breakers coordinated via trip curves/settings

## 🔍 Device Selection Rationale

* **2000 A main MCCB** for full bus protection + coordination flexibility
* **Feeder MCCBs** sized to probable load classes
* Emphasis on **selective coordination**, arc-fault containment, and future adjustability

## 📎 Notes

* This is a **concept/demo-level** package — not intended for construction
* Format and structure align with real-world electrical engineering documentation workflows

---