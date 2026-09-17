# Design Log: SDMTS Trolley Tracker Board  

The SDMTS Trolley Tracker Board is an in-progress PCB design that tracks the status of each station on a given line in the MTS trolley lines. Each station will have a dedicated LED that illuminates when a train has arrived at that station. The board will operate using live data from the OneBusAway RESTful API that the MTS uses to provide real time locations. 

## Quick Overview

* **Author:** A. Borja
* **Start Date:** September 15, 2026
* **Software:** Altium Designer, VS Code, GitHub
* **Languages:** TBD

### Objective

The objective is to create a PCB board that connects to the OneBusAway RESTful API, runs computations to determine the proximity of each trolley to nearby stations, and illuminates a station's LED (located on the board) once a trolley is within a 100m radius of the station.

## Phase 1: Ideation

For a complete map of San Diego's trolley system, there is a total of **62 stations**.  
*UC San Diego Blue Line:* 32 stations (22 unique, 10 shared)  
*East County Connector Copper Line*: 4 stations (3 unique, 1 shared)  
*Green Line*: 24 stations (15 unique, 9 shared)  
*Orange Line*: 17 stations (9 unique, 8 shared)  

