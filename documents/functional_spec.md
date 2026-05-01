# Intra Proj

**Authors:**
- 
- Vents Zemene – 23705099  


## Table of Contents
1. Introduction  
   1.1 Overview  
   1.2 Business Context  
   1.3 Glossary  
2. General Description  
   2.1 System Functions  
   2.2 User Characteristics and Objectives  
   2.3 Operational Scenarios  
   2.4 Constraints  
3. Functional Requirements  
4. System Architecture  
   4.1 Hardware Architecture  
   4.2 Operating System Architecture  
   4.3 Software Architecture  
5. High-Level Design  
   5.1 System Context Model    
7. Appendices
8. References

---

## 1. Introduction

### 1.1 Overview


### 1.2 Business Context


### 1.3 Glossary


---

## 2. General Description

### 2.1 System Functions


### 2.2 User Characteristics and Objectives
- **Target users**: 
- **Knowledge expected**: 
- **Objectives**:  

### 2.3 Operational Scenarios


---

#### Use Case 1 – System Start‑Up
| Field | Description |
|-------|-------------|
| **Use Case ID** | 1 |
| **Title** | Launch Synthesiser |
| **Actors** | User, Raspberry Pi, Audio Output Subsystem (PortAudio), MIDI System (RtMidi), DAC (Scarlett 4i4) |
| **Preconditions** | Raspberry Pi powered, touchscreen fitted, DAC connected and set as default, speakers connected, libraries installed (PortAudio, RtMidi, ImGui). |
| **Flow of Events** | User powers on Pi → OS boots → App launches → Audio Output Subsystem initialised with DAC → SynthEngine initialised with default sine oscillator → RtMidi scans → GUI loads (keyboard hidden if MIDI detected, shown otherwise). |
| **Postconditions** | Synthesiser initialised, GUI shows correct keyboard, audio routed through DAC. |

---




### 2.4 Constraints
- Must run smoothly on Raspberry Pi  
- Real‑time audio latency < 20ms  
- etc.....


---

## 3. Functional Requirements

**Real‑Time Audio Output**  
- **Description**: System must produce sound at stable 48kHz sample rate  
- **Criticality**: Essential  
- **Technical Issues**: Must be low latency, thread‑safe, concurrent  
- **Dependencies**: PortAudio, threading in C++  


---

## 4. System Architecture


### 4.1 Hardware Architecture


### 4.2 Operating System Architecture


### 4.3 Software Architecture

---

## 5. High-Level Design

### 5.1 System Context Model

---

---

### 7. Appendices

#### Library Documentation
- 

### 8. References





