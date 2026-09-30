# iKwath Pod

A pod-based smart Kwatha (Kadha) maker that prepares a fresh decoction from coarse powder (yavakuta churna) on demand, in the shortest practical time without changing the quality or yield of the decoction.

Smart India Hackathon 2026, Problem Statement 26048 (Ministry of AYUSH).

This repository contains the CAD model of the first-iteration prototype, designed in SolidWorks 2026.

## Concept
The machine works like a coffee machine. The user inserts a pod of premixed herbal powder, the NFC sensor identifies the formulation, and the machine runs the cycle set for that Kadha.

## Main Components
- **Water storage container:** holds the water supply.
- **Boiling container (stainless steel):** where the decoction is prepared.
- **Pumps:** move water from the storage container to the boiling container, and the finished liquid to the dispenser.
- **Induction heating:** a coil and an AC driver produce a magnetic field that heats the boiling container by eddy currents.
- **Ultrasonic transducers (40 kHz piezoelectric):** break open plant cell membranes to speed up extraction and reduce preparation time.
- **NFC sensor:** reads the pod and starts the process for that specific Kadha.
- **Touchscreen display:** start and stop control for the user.
- **Exhaust fan:** clears vapor from the boiling chamber during the process.
- **Drainer in the boiling container:** keeps powder out of the outlet pipe.
- **Filter paper at the dispenser:** catches any particles that pass through.
- **Electronic box:** houses the electronics. The controller will be an ESP32 or a Raspberry Pi, chosen after prototyping.

## Planned Improvements
- Self pod-opening mechanism (under development)
- Automatic lid lock while the process runs
- Flow sensor to measure liquid transferred to the boiling chamber, validated with a load cell
- Alternatives to the induction coil, such as microwave-induced heating

## Status
First-iteration design. The layout shows the overall setup, and details will change as prototyping continues.

## Repository Structure
- `cad/`: native SolidWorks parts and assembly (Pack and Go)
- `drawings/`: 2D drawings in PDF
- `images/`: isometric, top and front views

## How to Open
- With SolidWorks: open the `.SLDASM` file in `cad/`. Keep all files in the same folder so references do not break.

## Team
Ohm_Lawmen, DJSCE Mumbai
