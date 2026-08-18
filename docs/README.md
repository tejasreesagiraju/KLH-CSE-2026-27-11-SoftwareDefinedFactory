# Software-Defined Factory Controller using Distributed RT Linux

## Team Members

| S. No. | Roll Number | Name           |
| :----: | :---------: | -------------- |
|    1   |  2420030313 | P Maha Lakshmi |
|    2   |  2420030441 | S Tejasree     |
|    3   |  2420030578 | B Sruthi       |
|    4   |  2420090132 | K Amulya       |

## Supervisor

**C.H. Srikanth**

---

## Abstract

This project develops a **Software-Defined Factory Controller using Distributed Real-Time Linux (RT Linux)** for an automated conveyor-based sorting process.

The system is implemented as a **software-based simulation**, eliminating the need for physical hardware. The factory process is divided into multiple software modules running as separate RT Linux nodes. These nodes perform conveyor control, object detection, sorting decisions, and inter-node communication.

The distributed architecture enables real-time processing, modular control, and reliable communication between different factory operations. The project demonstrates how software-defined and distributed real-time control can be used to simulate an automated industrial sorting system.

---

## Project Objectives

* Develop a software-defined controller for an automated factory sorting process.
* Implement distributed control using separate RT Linux nodes.
* Simulate conveyor control, object detection, and sorting operations.
* Enable real-time communication between the distributed nodes.
* Implement automated sorting decisions based on detected object properties.
* Provide a modular and flexible software architecture.
* Monitor the status and results of the simulated factory process.

---

## System Architecture

The system consists of multiple software-based RT Linux nodes:

```text
                ┌─────────────────────────┐
                │     Controller Node     │
                │  Overall Coordination   │
                └────────────┬────────────┘
                             │
              ┌──────────────┼──────────────┐
              │              │              │
              ▼              ▼              ▼
      ┌─────────────┐ ┌─────────────┐ ┌─────────────┐
      │  Conveyor   │ │  Detection  │ │   Sorting   │
      │    Node     │ │    Node     │ │    Node     │
      └─────────────┘ └─────────────┘ └─────────────┘
              │              │              │
              └──────────────┼──────────────┘
                             ▼
                   ┌──────────────────┐
                   │ Communication /  │
                   │ Monitoring Module │
                   └──────────────────┘
```

### Main Modules

| Module               | Function                                           |
| -------------------- | -------------------------------------------------- |
| Conveyor Node        | Simulates conveyor movement and control            |
| Detection Node       | Detects and classifies simulated objects           |
| Sorting Node         | Makes sorting decisions based on detection results |
| Controller Node      | Coordinates the complete factory process           |
| Communication Module | Enables communication between distributed nodes    |
| Monitoring Module    | Displays system status and sorting results         |

---

## Repository Structure

The repository follows the GitHub submission norms:

```text
Software-Defined-Factory-Controller/
│
├── src/
│   ├── controller/
│   ├── conveyor/
│   ├── detection/
│   ├── sorting/
│   └── communication/
│
├── docs/
│   └── project-documentation/
│
├── data/
│   └── README.md
│
├── results/
│   └── README.md
│
├── reports/
│   └── README.md
│
└── README.md
```

### Folder Description

* **`src/`** – Contains the main project source code.
* **`docs/`** – Contains project documentation and supporting documents.
* **`data/`** – Contains project data or a documented reference to the data source.
* **`results/`** – Contains simulation outputs, logs, and result files.
* **`reports/`** – Contains project reports and review-related documents.
* **`README.md`** – Contains the complete project information and instructions.

---

## Setup Instructions

### Prerequisites

Install the required software and dependencies before running the project.

The project requires:

* Linux / RT Linux environment
* Git
* Required programming language/runtime dependencies
* Required libraries for the simulation
* Networking/communication tools required by the distributed nodes

### Clone the Repository

```bash
git clone <repository-url>
```

Navigate to the project directory:

```bash
cd <repository-name>
```

Install the required dependencies according to the project implementation.

---

## Execution Instructions

1. Start the required RT Linux environment.
2. Start the **Controller Node**.
3. Start the **Conveyor Node**.
4. Start the **Detection Node**.
5. Start the **Sorting Node**.
6. Establish communication between the nodes.
7. Run the simulated conveyor-based sorting process.
8. Monitor the communication, object detection, and sorting results.
9. Check the generated outputs in the `results/` directory.

---

## Current Project Status

**Phase:** Review 1

**Status:** Project architecture and initial software structure are being developed.

### Current Progress

* Project architecture defined.
* Distributed RT Linux node structure planned.
* Conveyor control module planned.
* Object detection module planned.
* Sorting module planned.
* Inter-node communication architecture planned.
* GitHub repository structure established.

---

## Future Work

* Implement the distributed RT Linux nodes.
* Implement inter-node communication.
* Develop the conveyor simulation.
* Implement object detection and classification.
* Implement automated sorting logic.
* Integrate all software modules.
* Test real-time communication and system performance.
* Generate and analyze simulation results.
* Complete Review 2 and final project deliverables.

---

## Project Team

**P Maha Lakshmi** – 2420030313
**S Tejasree** – 2420030441
**B Sruthi** – 2420030578
**K Amulya** – 2420090132

**Supervisor:** C.H. Srikanth
