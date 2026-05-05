# Three-Floor Elevator Controller (Verilog FSM)

## Overview
This project implements a **three-floor elevator controller** using a **Finite State Machine (FSM)** in Verilog.  
The design was tested entirely in simulation without hardware, and focuses on practicing **FSM design, state transitions, and verification**.

---

## FSM States
The elevator controller is modeled as a **5-state FSM**:
- `IDLE` – Elevator is stationary at the current floor  
- `MOVING_UP` – Elevator moves towards a higher floor  
- `MOVING_DOWN` – Elevator moves towards a lower floor  
- `DOOR_OPEN` – Doors open for passengers  
- `DOOR_CLOSED` – Doors close before movement or after boarding/alighting  
- `EMERGENCY_STOP` – (planned but not implemented in this version)

---

## Features
- **Floor navigation logic** to move between floors  
- **Door LED indication** for passenger feedback  
- **State debug LED** for simulation visibility  

---

## Testing & Verification
The elevator controller was tested with **Verilog testbenches**:
- **Functional Tests** – Checking normal floor transitions  
- **State Transitions** – Verifying FSM behavior for up/down movement  
- **Edge Cases** – Emergency stop was considered but not fully implemented.

Outputs were verified through simulation logs and waveform viewers such as GTKWave.

---

## Design Challenges
- Mapping real-world elevator behavior into a **limited set of FSM states**  
- Deciding which states/features (e.g., bell ring, emergency) to include in the minimal design  
- Ensuring synchronization with **button press simulation** in the testbench  

---

## Learning Outcomes
- Gained hands-on experience in **FSM design for real-world systems**  
- Learned to implement **state-driven control logic** in Verilog  
- Improved skills in **functional verification using simulation**
