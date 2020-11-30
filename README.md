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
