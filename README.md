# Solar Array Based Single Input Multi Output Converter

## Project Overview

This project presents the design and simulation of a solar array based single input multi output converter. The proposed system uses a photovoltaic array as the input source and generates multiple isolated DC bus voltages using a multi-winding transformer based converter structure.

Averaged converter models are used for the simulation in order to reduce computational time and improve simulation stability. Although high-fidelity switching models provide more accurate device-level behavior, they require significantly higher simulation time, especially when multiple converter stages and transformer windings are involved.

The system is designed using a photovoltaic source, MPPT-controlled boost converter, single-phase inverter, multi-winding transformer, rectification stages, buck converters, and an inverter with an LCL output filter.

---

## System Block Diagram

![System Block Diagram](images/simulation_diagram.png)

The overall power flow of the system is:

```text
PV Array → Boost Converter → Single-Phase Inverter → Multi-Winding Transformer
         → Rectifier Stages → Buck Converters → DC Output Buses
