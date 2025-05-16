#  IEEE 39-Bus System Analysis with Industrial Load and PV Integration

## Table of Contents
- [Introduction](#introduction)
- [System Description](#system-description)
- [Tasks](#tasks)
- [Modifications](#modifications)
- [Simulation Results](#simulation-results)
- [Conclusion](#conclusion)


---

## Introduction
This project focuses on analyzing the IEEE 39-bus power system network. The main objective was to observe the impact of integrating photovoltaic (PV) generators and large industrial loads into the system. We used load flow and fault analysis to study how these additions affect system performance.

---

## System Description
The IEEE 39-bus system, also known as the New England power system, contains 39 buses, 10 generators, and multiple loads and transformers. The nominal frequency is 50 Hz. This system is often used for stability and fault analysis in power systems.

---

## Tasks

**Task 1 & 2:**  
Performed load flow analysis on the base IEEE 39-bus system without any modifications. The load flow successfully converged, meaning the input data was correct.

**Task 3:**  
We modified the generators connected at buses 32, 33, 34, and 36 to work as PV generators. The fault current for PVs was assumed to be equal to their rated current. We then did fault analysis at those buses.

**Task 4 & 5:**  
We added an industrial plant (modeled as an induction motor) at Bus 23. After adding it, we performed load flow again to see how the system changed. The motor had a rating of 100 MVA with 0.8 power factor and 90% efficiency.

---

## Modifications

- **PV Generator Assumptions:**  
  - Power factor: 0.9  
  - Qmax = 0.2 × MVA  
  - Qmin = –0.2 × MVA  

- **Industrial Load (Induction Motor):**  
  - Bus: 23  
  - Voltage: 345 kV  
  - Efficiency: 90%  
  - MVA rating: 100 MVA  
  - Power factor: 0.8  
  - KW rating: 72,000 kW  
  - R = 0.00556, X = 0.3  

---

## Simulation Results

- The base case load flow converged, confirming correct data entry.
- After converting selected generators to PV, the system behaved differently, especially in fault responses.
- Adding the induction motor increased the loading at Bus 23. Voltage slightly dropped and nearby buses also showed changes in power flow.
- Compared to the base case, the modified system had noticeable changes in voltage profiles and line loadings.

<p align="center">
<img src="https://github.com/user-attachments/assets/59d272b5-5c53-43a1-87e8-cd5cf16f0c11" width="400">
</p>
---

## Conclusion

We successfully analyzed the IEEE 39-bus system under different scenarios. Adding PV generators and a large industrial load had a clear effect on system performance. This project helped us understand the behavior of power systems under real-world conditions like renewable integration and large-scale industrial consumption.

---
