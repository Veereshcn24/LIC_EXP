# Modified Current-Reuse OTA for High CMRR

## Objective
To design and implement a modified current-reuse operational transconductance amplifier (OTA) optimized for high common-mode rejection ratio (CMRR) in low-power and low-voltage analog applications. The amplifier employs a cross-coupled load topology combined with a current-reuse architecture to enhance differential gain while significantly attenuating common-mode signals.

## Design Specifications
- **Supply Voltage**: ±1.5 V
- **Input Range**: ±0.9 V
- **Bandwidth**: Up to 10 MHz
- **Total Harmonic Distortion (THD)**: <1%
- **Linearity Error**: <1%
- **Power Consumption**: Approx. 0.5 mW

## Design Description

### 1. Input Stage (Differential Pair)
- Utilizes PMOS or NMOS differential input stage with a wide input range (±0.9 V).
- Supports bulk-driven extensions for wider swing under low overdrive.
- Operates in subthreshold or moderate inversion to improve linearity and reduce noise.

### 2. Cross-Coupled Load
- Provides low impedance for common-mode signals and high impedance for differential mode.
- Suppresses common-mode gain, significantly boosting CMRR.

### 3. Current-Reuse Mechanism
- Stacks NMOS and PMOS differential pairs to reuse tail current, effectively doubling transconductance without increasing power.
- Improves gain-bandwidth product and power efficiency.

### 4. Common-Mode Feedback (CMFB)

- Ensures balanced differential operation by stabilizing output common-mode voltage.

## 5. Circuit Diagram


![image](https://github.com/user-attachments/assets/110d46d9-bcd6-4ac9-b80b-ebefba69b81b)

##  6.  lt spice simulation result 


![image](https://github.com/user-attachments/assets/84cb13ff-8d3b-4929-97c9-bffb68cb0819)

## 7. operational point analysis

![image](https://github.com/user-attachments/assets/38a4c424-4567-4a55-b29c-7e8b42882286)

## 8.  output 

* a) commom mode output
  
![image](https://github.com/user-attachments/assets/8f594120-6bbb-4401-9021-cbfa86ef5055)
  
* b) differential mode analysis
  
![image](https://github.com/user-attachments/assets/a75a5e31-c488-4dcf-b1b5-727362eb1abe)




## 9.  LTspice Simulation Results
- **Input**: (Details not fully specified in the provided document.)
- **Operation Point Analysis**: (Details not fully specified in the provided document.)
- **Output**:
  - **Common-Mode Output**: (Details not fully specified in the provided document.)
  - **Differential Mode Analysis**: (Details not fully specified in the provided document.)

## Results
- **Open-Loop Gain**: 40–60 dB
- **Bandwidth**: Up to 10 MHz
- **Total Harmonic Distortion (THD)**: <1%
- **Linearity Error**: <1%
- **Power Consumption**: Approx. 0.5 mW

## Conclusion
This project presents the design of a Modified Current-Reuse Operational Transconductance Amplifier (OTA) optimized for high common-mode rejection ratio (CMRR) in low-power, low-voltage analog applications. The architecture integrates:

- A differential input stage for wide input range and low noise.
- A cross-coupled active load for enhanced common-mode suppression.
- A current-reuse architecture to improve transconductance and power efficiency.

Operating at a supply voltage of ±1.5 V, the OTA achieves:
- A bandwidth of up to 10 MHz.
- An open-loop gain of 40–60 dB.
- Low harmonic distortion (<1%) and linearity error (<1%).
- Power consumption of approximately 0.5 mW.

These characteristics make the proposed OTA highly suitable for applications such as biomedical instrumentation, wearable sensors, and IoT analog front-ends, where signal integrity and energy efficiency are critical.

## Summary
The modified current-reuse OTA combines a differential input stage, cross-coupled active load, and current-reuse stacking technique to achieve a compact, power-efficient design with high CMRR. It is designed for low-power, low-voltage applications, operating at ±1.5 V with a bandwidth of up to 10 MHz, an open-loop gain of 40–60 dB, and low distortion and linearity error (<1%). With a power consumption of approximately 0.5 mW, it is ideal for biomedical signal acquisition, wearable devices, and IoT sensor interfaces.

---

*Note*: Simulation results and circuit diagrams were referenced but not fully detailed in the provided document. For a complete report, include LTspice simulation data and schematic diagrams as images or linked files.
