# sme-pcb-energysolution-s01

## Project description

This repository contains the energy PCB design for the SME project. The project was created in Altium Designer and is organized around a main schematic sheet with subcircuits for power management, conversion, protection, and output regulation.

This board is intended to work with a single-cell 3.7 V lithium battery, charge it from a 5 V supply, and provide regulated 5 V and 3.3 V outputs up to 3 A.

![PCB 3D preview](Project%20Ouputs/PCB%203D%20Print/PCB_s01.png)

## What this repository is useful for

This repository is useful for:

- Reviewing and understanding the power architecture of the SME solution.
- Opening the complete Altium project and modifying the schematic or PCB layout.
- Generating and checking manufacturing outputs such as BOMs, Gerbers, drill files, and pick-and-place data.
- Tracking design changes through ECO logs.
- Accessing the technical datasheets referenced by the design.

## Integrated circuits used

The design includes the following integrated circuits and power-management devices:

- **MIC841**: protection and supervision block.
- **TPS63021**: buck-boost converter used for voltage conversion and power support.
- **MP2759GQ**: charging and power-path control device.
- **TPS61022**: boost converter used to raise voltage when required.
- **S8261**: additional regulator for the system output stage.

## Project structure

### Main files

- `sme-pcb-energysolution-s01.PrjPcb`: Altium project.
- `PCB_s01.PcbDoc`: main PCB board file.
- `SME_Main.SchDoc`: main schematic sheet.
- `SME_mic841.SchDoc`: MIC841 circuit block.
- `SME_tps63021.SchDoc`: TPS63021 converter block.
- `SME_mp2759gq.SchDoc`: MP2759GQ controller block.
- `SME_MP2759GQ_PowerPath.SchDoc`: power-path section associated with MP2759GQ.
- `SME_tps61022.SchDoc`: TPS61022 converter block.
- `SME_S8261.SchDoc`: S8261 regulator block.

### Important folders

- `Datasheet/`: component datasheets used by the design.
- `Project Logs for sme-pcb-energysolution-s01/`: ECO and change history for the schematic and PCB.
- `Project Ouputs/`: manufacturing, review, and analysis outputs.
- `__Previews/`: preview images of the schematic sheets.
- `History/`: version history for the project.

## Technical documentation

### Available datasheets

- `20005758A.pdf`
- `DATASHEET_BWVS00505020_SERIES.pdf`
- `tps61022.pdf`
- `tps63021.pdf`

These references should be reviewed before changing values, tolerances, or power-routing decisions.

## Project outputs

### BOM and verification

- `Project Ouputs/BOM/Bill of Materials-sme-pcb-energysolution-s01.xlsx`
- `Project Ouputs/BOM/BOM Checks Report-sme-pcb-energysolution-s01.html`
- `Project Ouputs/BOM/PCBWay - BOM-sme-pcb-energysolution-s01.csv`

### Manufacturing and packaging

- `Project Ouputs/PCBWay/Assembly Fabrication/`
- `Project Ouputs/PCBWay/Board Fabrication/`
- `Project Ouputs/PCBWay/Status Report.Txt`
- `Project Ouputs/Pick Place/Pick Place for PCB_s01.csv`
- `Project Ouputs/Pick Place/Pick Place for PCB_s01.txt`

### Quality reports

- `Project Ouputs/DRC/PCB_s01.html`
- `Project Ouputs/ERC/sme-pcb-energysolution-s01.html`
- `Project Ouputs/ECCC/sme-pcb-energysolution-s01.html`
- `Project Ouputs/ComponentState/sme-pcb-energysolution-s01.html`

### Manufacturing files

- `Project Ouputs/GerberX2/PCB_s01_Copper_Signal_Bot.gbr`
- `Project Ouputs/GerberX2/PCB_s01_Copper_Signal_Top.gbr`
- `Project Ouputs/GerberX2/PCB_s01_Legend_Bot.gbr`
- `Project Ouputs/GerberX2/PCB_s01_Legend_Top.gbr`
- `Project Ouputs/GerberX2/PCB_s01_NPTH_Drill.gbr`
- `Project Ouputs/GerberX2/PCB_s01_Paste_Bot.gbr`
- `Project Ouputs/GerberX2/PCB_s01_Paste_Top.gbr`
- `Project Ouputs/GerberX2/PCB_s01_Profile.gbr`
- `Project Ouputs/GerberX2/PCB_s01_PTH_Drill.gbr`
- `Project Ouputs/GerberX2/PCB_s01_Soldermask_Bot.gbr`
- `Project Ouputs/GerberX2/PCB_s01_Soldermask_Top.gbr`
- `Project Ouputs/NC Drill/PCB_s01.DRR`
- `Project Ouputs/NC Drill/PCB_s01.LDP`
- `Project Ouputs/NC Drill/PCB_s01.TXT`

## How to open and work on the project

1. Open `sme-pcb-energysolution-s01.PrjPcb` in Altium Designer.
2. Verify that the schematic and PCB files are synchronized.
3. Review the ECO logs in `Project Logs for sme-pcb-energysolution-s01/` before generating outputs.
4. Regenerate the BOM, Gerbers, DRC, and pick-and-place files if the design changes.