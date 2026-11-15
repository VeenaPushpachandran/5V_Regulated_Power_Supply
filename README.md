# 5V Regulated Power Supply – KiCad PCB Design

## Project Overview

This project involves the design and PCB layout of a 5V regulated DC power supply using the LM7805 linear voltage regulator. The circuit accepts a nominal 9V DC input and provides a regulated 5V DC output for low-power electronic applications.

The project was developed using KiCad, covering schematic capture, component selection, PCB layout, copper zone configuration, design rule checking (DRC), and manufacturing file preparation.

## Project Specifications

| Parameter | Specification |
|---|---|
| Input Voltage | 9V DC nominal |
| Output Voltage | 5V DC regulated |
| Voltage Regulator | LM7805 |
| Target Load Current | 100mA |
| PCB Design Software | KiCad |
| PCB Dimensions | Approximately 50mm × 35mm |
| PCB Layers | 2-layer design |

## Circuit Description

The circuit uses an LM7805 linear voltage regulator to convert the 9V DC input into a regulated 5V DC output.

The circuit includes:

- Input electrolytic capacitor for bulk filtering.
- Input ceramic bypass capacitor for high-frequency noise suppression.
- LM7805 linear voltage regulator for voltage regulation.
- Output ceramic bypass capacitor for stability and transient response.
- Output electrolytic capacitor for additional filtering.
- Two-pin input and output connectors.

## Component Selection

| Reference | Component | Value |
|---|---|---|
| U1 | LM7805 Voltage Regulator | 5V |
| C1 | Electrolytic Capacitor | 10µF |
| C2 | Ceramic Capacitor | 100nF |
| C3 | Ceramic Capacitor | 100nF |
| C4 | Electrolytic Capacitor | 10µF |
| J1 | Input Connector | 2-pin |
| J2 | Output Connector | 2-pin |

## PCB Design and Layout

The PCB was designed in KiCad using a two-layer layout.

Design activities included:

- Schematic capture and electrical net assignment.
- Component footprint assignment.
- PCB component placement and routing.
- Power and ground routing.
- Bottom-layer GND copper zone configuration.
- Board outline definition.
- Design Rule Check (DRC).

## Design Calculations

At a nominal 9V input and 5V output:

**Voltage drop across regulator:**

Vdrop = 9V − 5V = 4V

**Estimated regulator power dissipation at 100mA:**

P = (Vin − Vout) × I

P = (9V − 5V) × 0.1A = 0.4W

**Equivalent load resistance at 100mA:**

R = V / I = 5V / 0.1A = 50Ω

Thermal performance and component ratings must be verified before operation at the target load.

## Design Rule Check (DRC)

The KiCad Design Rule Check was completed with the following reported results:

- DRC violations: 0
- Unconnected pads: 0
- Footprint errors: 0

Some optional DRC checks were configured as ignored and require separate review.

## Project Documentation

The repository includes supporting engineering documentation:

- Project Overview
- Bill of Materials (BOM)
- Design Calculations
- Component Selection Justification
- DRC Report
- PCB design screenshots

## Manufacturing Files

Gerber and drill files are prepared for PCB fabrication. These files should be independently checked in a Gerber viewer before manufacturing.

## Project Status

**PCB design and initial DRC completed. Physical prototype testing is pending.**

The design has not yet been validated through physical measurements. Output voltage regulation, load performance, ripple, and thermal behaviour remain to be tested on a fabricated prototype.

## Software and Tools

- KiCad – Schematic capture and PCB design
- Gerber Viewer – Manufacturing output inspection
- GitHub – Project version control and documentation

## Skills Demonstrated

- Electronic circuit design
- Linear voltage regulation
- Electronic component selection
- Schematic capture
- PCB layout and routing
- Through-hole component footprints
- Ground copper zone configuration
- Design Rule Checking
- Gerber and drill file generation
- Engineering documentation

---

**Author:** Veena Pushpachandran, Engineer-in-Training (EIT) – Engineers Nova Scotia

**Project:** 5V Regulated Power Supply PCB Design
