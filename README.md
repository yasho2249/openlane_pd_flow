This repo is an attempt at and a tutorial for the OpenLane Physical Design Flow

# Table of Contents

* RTL2GDS flow
* Introduction to OpenLANE
* Synthesis
* Floorplan
* Placement
* Standard cell design and characterization
* Timing Analysis
* Clock Tree Synthesis
* Routing
* DRC

# RTL2GDS flow
![](Snapshots/rtl2gds.png)

# Introdction to OpenLANE
![](Snapshots/openlane_flowchart.png)

## Invoking OpenLANE: 
![](Snapshots/openlane_invoke.png)

Preparation for Synthesis:
![](Snapshots/prep_for_synth.png)

# Synthesis
![](Snapshots/synthesis.png)

Synthesis Statistics:
![](Snapshots/synthesis_statistics.png)

Snapshot of the Netlist:
![](Snapshots/netlist.png)

# Floorplan
![](Snapshots/floorplan.png)

Floorplanning logs and edits:
![](Snapshots/floorplan_log_edits.png)

SkyLake130 config.tcl (highest priority):
![](Snapshots/sky_tcl.png)

Floorplan Custom config.tcl:
![](Snapshots/floorplan_custom_config.png)

Floorplan Default config.tcl (lowest priority):
![](Snapshots/default_config.png)

Environment Variables:
![](Snapshots/echo_set.png)

Floorplan def file:
![](Snapshots/floorplan_def.png)

## Invoking Magic
![](Snapshots/invoke_magic1.png)

![](Snapshots/invoke_magic.png)

Floorplan Analysis on Magic:
![](Snapshots/fr_magic_analysis.png)

# Placement
![](Snapshots/placement.png)

Placement on Magic:
![](Snapshots/placement_magic.png)

# Standard cell design and characterization
Cloning the required custom cell files:
![](Snapshots/custom_cell_gitclone.png)

Custom Inverter Cell on Magic:
![](Snapshots/custom_inv_magic.png)

Export to Ngspice for analysis:
![](Snapshots/custom_inv_spice.png)

Spice file:
![](Snapshots/custom_inv_spice_file.png)

## Invoke ngspice
![](Snapshots/invoke_ngspice.png)

Transient Analysis of Custom Inverter Cell:
![](Snapshots/inv_transient.png)

Lef file of Custom Inverter Cell:
![](Snapshots/inv_lef.png)

Lib file for inclusion of custom cell:
![](Snapshots/scr_custom_inv.png)

Custom config for inclusion of custom cell:
![](Snapshots/inv_config.png)

Synthesis prep witj custom inverter cell:
![](Snapshots/inv_synthesis.png)

Synthesis:
![](Snapshots/inv_synthesis.png)

# Timing Analysis
Synthesis with better slack: 
![](Snapshots/inv_synth2.png)

Floorplan with custom Inverter cell:
![](Snapshots/inv_floorplan.png)

Placement with Custom Inverter celll:
![](Snapshots/inv_placement.png)

Placement of custom inverter cell on Magic:
![](Snapshots/inv_placement_magic.png)

# Clock Tree Synthesis
Command for CTS. Ran with the default config. 
```
run_cts
```
The output of CTS stage will provide a new netlist in ~/results/synthesis/ folder name picorv32a.synthesis_cts.v

# Routing

# DRC
