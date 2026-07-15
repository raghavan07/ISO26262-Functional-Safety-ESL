# ISO 26262 Functional Safety Analysis – Electronic Steering Lock (ESL)

## Project Overview

This project demonstrates the application of the ISO 26262 concept-phase functional safety workflow to an Electronic Steering Lock (ESL) system.

The project focuses on identifying potential hazards associated with steering lock malfunctions, evaluating hazardous events using Hazard Analysis and Risk Assessment (HARA), deriving Safety Goals, and developing Functional Safety Requirements (FSRs).

System architecture and requirement traceability are modelled using SysML in Visual Paradigm.

---

## Project Objective

The objective of this project is to perform a concept-level functional safety analysis of an Electronic Steering Lock and develop safety requirements to prevent hazardous steering lock behaviour.

A primary safety concern considered in this project is unintended steering lock activation while the vehicle is moving.

---

## Electronic Steering Lock – Item Functions

The ESL performs the following item functions:

- Lock Steering
- Unlock Steering
- Detect Lock Position
- Receive Lock/Unlock Commands via CAN
- Transmit Lock Status via CAN
- Perform Diagnostics

---

## ESL System Architecture

The ESL item architecture includes:

- ESL ECU
- CAN Transceiver
- Motor Driver
- Reversible DC Motor
- Gear Train
- Lock Bolt / Locking Mechanism
- Lock Position Sensor

The ESL interfaces with the BCM/EIS through the vehicle CAN network and mechanically interfaces with the steering column.

SysML Block Definition Diagram (BDD) and Internal Block Diagram (IBD) were developed to represent the system structure and internal interactions.

---

## Functional Safety Workflow

The following workflow was applied:

1. Item Definition
2. Item Function Identification
3. System Boundary Definition
4. SysML BDD and IBD Development
5. HAZOP Analysis
6. Operational Situation Identification
7. Hazard Analysis and Risk Assessment (HARA)
8. Severity, Exposure and Controllability Evaluation
9. ASIL Classification
10. Safety Goal Derivation
11. Functional Safety Concept Development
12. Functional Safety Requirement Derivation

---

## Hazard Analysis and Risk Assessment

Potential ESL malfunctions were analysed together with relevant operational situations to identify hazardous events.

Each hazardous event was evaluated based on:

- Severity (S)
- Exposure (E)
- Controllability (C)

The corresponding Automotive Safety Integrity Level (ASIL) was determined using the ISO 26262 risk classification approach.

The analysis includes hazardous scenarios such as unintended steering lock activation during vehicle movement, incorrect lock position detection, communication faults, and undetected safety-related faults.

---

## Safety Goals

Safety Goals were derived from the identified hazardous events.

An example ASIL D Safety Goal developed in this project is:

> **SG-001: Prevent unintended steering lock activation while the vehicle is moving.**

The Safety Goals provide the top-level safety objectives for the ESL system.

---

## Functional Safety Concept

A Functional Safety Concept was developed for SG-001.

Functional Safety Requirements were derived to:

- Prevent steering lock actuation while the vehicle is moving
- Determine the vehicle movement state before permitting lock actuation
- Validate vehicle movement information
- Inhibit lock actuation when movement information is invalid or unavailable
- Detect faults that could result in unintended steering lock actuation
- Maintain the unlocked safe state under safety-related fault conditions
- Communicate safety-related fault status to the vehicle-level controller

Requirement traceability between the Safety Goal and Functional Safety Requirements was modelled using SysML requirement diagrams.

---

## Tools Used

- Visual Paradigm – SysML modelling and requirement traceability
- Ms.Excel – HAZOP, HARA and Safety Goal analysis
- Microsoft PowerPoint – Project documentation and presentation

---

## Repository Contents

- `Fusa_ESL.pptx` – Functional Safety project presentation
- `HARA.ods` – HAZOP, HARA and Safety Goal analysis
- `README.md` – Project documentation

---

## Project Scope

This is a self-developed concept-level functional safety project created for learning and demonstrating the ISO 26262 concept-phase workflow.

The ESL architecture, assumptions, hazardous scenarios and safety requirements are developed for educational and portfolio purposes and do not represent confidential OEM or supplier production data.

---

## Author

**Venkatraghavan Rajagopal**

MSc Autonomous Vehicle Engineering

does not represent confidential OEM or supplier production data
