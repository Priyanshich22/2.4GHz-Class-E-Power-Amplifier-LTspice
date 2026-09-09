# 2.4 GHz CMOS Class-E Power Amplifier for IEEE 802.15.1 (Bluetooth/WPAN) Applications

## Project Overview

This project focuses on the design and LTspice-based simulation of a
2.4 GHz CMOS Class-E Power Amplifier in 180 nm CMOS technology.

Three power amplifier configurations were designed and analyzed:

- Conventional Class-E
- Self-Biased Class-E
- Bootstrapped Cascode Class-E

The designs were evaluated through circuit-level simulations to study
transient behavior and efficiency under different operating conditions.

## Design Specifications

| Parameter | Specification |
|---|---|
| CMOS Technology | 180 nm |
| Supply Voltage | 1.8 V |
| Operating Frequency | 2.4 GHz |
| Target Output Power | 15 dBm |
| Design Methodology | gm/ID |
| Simulation Tool | LTspice |

## Application

The 2.4 GHz operating frequency places the design within the 2.4 GHz
ISM band used by several short-range wireless technologies, including
Bluetooth/WPAN applications.

The project focuses on the RF power-amplifier stage and does not
implement the complete Bluetooth protocol stack or claim IEEE
802.15.1 compliance.

## Circuit Topologies

### 1. Conventional Class-E

The conventional Class-E power amplifier is used as the baseline
configuration for analyzing Class-E operation and RF performance.

### 2. Self-Biased Class-E

A self-biased Class-E configuration was designed and simulated to
investigate the effect of self-biasing on amplifier performance.

The design includes analysis of efficiency variation with self-bias
resistance.

### 3. Bootstrapped Cascode Class-E

A bootstrapped cascode Class-E configuration was designed and simulated
for the 2.4 GHz operating condition.

The configuration was analyzed through transient simulation and drain
efficiency variation.

## Design Methodology

The transistor sizing and design process was based on the gm/ID
methodology.

The power amplifier designs were developed for the following target
conditions:

- Supply voltage: 1.8 V
- Operating frequency: 2.4 GHz
- Target output power: 15 dBm
- CMOS technology: 180 nm

Component values for the RF design were determined using Class-E power
amplifier design relationships based on the target operating
specifications.

## Simulation

LTspice was used to verify the designed circuits.

The simulation analysis includes:

- Transient response
- RF output behavior
- Drain efficiency
- Efficiency variation with self-bias resistance
- Efficiency variation with source degeneration
- Analysis of different Class-E configurations

## Simulation Results

### Transient Response

Transient simulations were performed for:

- Conventional Class-E
- Self-Biased Class-E
- Bootstrapped Cascode Class-E

The corresponding simulation plots are included in the repository.

### Efficiency Analysis

The project also investigates efficiency variation under different
design conditions, including:

- Bootstrapped configuration
- Self-bias resistance
- Source degeneration

The simulation plots are provided in the repository for comparison and
analysis.

## Repository Structure

```text
2.4GHz-Class-E-Power-Amplifier-LTspice/
│
├── BOOTSTRAPED.asc
├── Bootstrapedfinal.asc
├── Conventional classe.asc
├── SELFBIASED PA.asc
├── Self biased.asc
│
├── Transient response of the bootstrapped cascode...
├── Transient response of the conventional cascode...
├── Transient response of the self-biased cascode...
├── Variation of simulated drain efficiency with bootstrapped...
├── Variation of simulated efficiency with self-bias resistance...
└── Variation of simulated efficiency with source-degeneration...
