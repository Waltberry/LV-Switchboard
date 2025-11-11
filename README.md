# LV Switchboard Mini-Package (Portfolio)

**Scope:** 600 V, 3φ, 4W, 60 Hz switchboard (2000 A bus) with main breaker and three feeders (400 A, 225 A, 100 A).  
**Intent:** Produce an "approval set" with SLD, front elevation, a feeder control schematic, and auto-generated tables (BOM, wire list, terminals, nameplates).

> This repo contains *reference PDFs* you can mirror in **AutoCAD Electrical** (preferred for report generation) or **QElectroTech + LibreCAD**. See `HowTo_AutoCAD_Electrical.md` and `HowTo_QElectroTech_LibreCAD.md`.

## Deliverables
- `drawings/SLD-001.pdf` — Single-Line Diagram
- `drawings/ELEV-001.pdf` — Front Elevation with device labels
- `drawings/SCH-101.pdf` — Feeder control schematic
- `tables/BOM_v1.xlsx`, `tables/WireList_v1.xlsx`, `tables/TerminalList_v1.xlsx`, `tables/Nameplates_v1.xlsx`
- `export/LV_Switchboard_ApprovalSet_v1.pdf` — Combined set

## Assumptions
- Service AFC: 50 kA @ 600 V (utility TBD). Switchboard SCCR target: 65 kA.
- Conductors: Cu THHN/THWN (placeholder sizes).
- Grounding per CEC Part I; coordination: main (electronic trip) > feeder MCCBs.

## Device selection rationale (high level)
- Main CB sized for bus (2000 A) with AIC ≥ utility AFC; electronic trip for adjustability and coordination.
- Feeders sized to loads with selective coordination targeted via trip curves/settings.

## Proof of *AutoCAD Electrical* use (what to show in repo)
Include (after you recreate drawings in AE):
- Screenshots of **Project Manager** and **Reports → BOM/Wire/Terminals**.
- Exported **.xls/.csv** reports (replace the placeholders in `tables/`).

## Notes
Portfolio exercise — not an engineered/stamped design.
