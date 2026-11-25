# FMCW Radar with ADALM-Pluto SDR and MATLAB

**5G Testbed Laboratory | Indian Institute of Science (IISc), Bengaluru | July 2022**  
**Project report prepared by:** Dhavala Bhat  
**Supervision:** Prof. Chandra R. Murthy, Department of Electrical Communication Engineering, IISc

## Project overview

This project investigated an **FMCW (frequency-modulated continuous-wave) radar** architecture using **ADALM-Pluto software-defined radio (SDR)** and **MATLAB**. The documented work covers chirp generation, radio-frequency up- and down-conversion, receive-signal processing, and experimental system-delay calibration.

The project was part of work at the 5G Testbed Laboratory at IISc. This repository is a portfolio summary of the engineering work described in the final project closure report.

## System workflow

1. Generate an FMCW chirp at baseband in MATLAB.
2. Transmit the signal using ADALM-Pluto SDR and an RF up-converter toward the **24 GHz** band.
3. Receive the returned signal using the down-converter and Pluto SDR.
4. Mix the transmit and receive baseband chirps in MATLAB.
5. Estimate the beat frequency using frequency-domain analysis and study its relationship to target range.

## Engineering work documented

- Modeled the radar signal chain in MATLAB, including chirp generation, conversion stages, channel/target representation, and baseband mixing.
- Investigated SDR platform choices and the integration of Pluto SDR with MATLAB.
- Documented characterization of RF components and synthesizer-related circuitry for a 2×2 MIMO system.
- Implemented and measured the radar signal chain in a **6 m RF-cable loopback configuration** to assess and calibrate system delay.

## Validation status

The original report documents **loopback testing through an RF cable**, including transmitted/received spectra and beat-frequency analysis. It identifies over-the-air testing with antennas and a physical target as **future work**. Accordingly, this repository does **not** claim that physical-target range detection was experimentally validated.

## Tools and technical areas

MATLAB · ADALM-Pluto SDR · FMCW chirps · SDR integration · RF up/down-conversion · Spectrum/FFT analysis · RF component characterization · Radar signal processing

## Project report

The complete 66-page [Final Project Closure Report](docs/Final_Project_Closure_Report_IISc_2022.pdf) covers the system design, MATLAB modeling, RF characterization, experimental setup, results, and future work.

Original standalone MATLAB scripts and hardware-design files were not supplied for this portfolio package. The README is a technical summary, not a runnable reproduction.
