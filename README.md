# Tldr;

DBR = Distributed Bragg Reflector.

Web-based DBR mirror simulator built using vanilla JS.
Implements TMM (Transfer Matrix Method).
We compute reflectance spectra R(λ) and spatial E-field standing wave |E(x)|² from first principles.
Semiconductor types are GaAs/AlAs, SiO₂/TiO₂, and Si/SiO₂ multilayer stacks.

[https://profound-sundae-8e7853.netlify.app/](https://profound-sundae-8e7853.netlify.app/)

<img width="674" height="460" alt="image" src="https://github.com/user-attachments/assets/7fbe9b7d-af20-4710-8060-c0bb975bafc1" />

# Physics background

A DBR mirror is made of alternating high- and low-refractive-index layers, 
each exactly a quarter-wavelength thick (d = λ₀/4n). 
At this condition, partial reflections from every interface arrive b
ack in phase — constructive interference builds reflectance toward 100%.
The DBR mirror is the passive reflector in a DBR laser. 
Two DBR stacks form  optical cavity around a quantum well active region.
Understanding how to design these mirrors 
(peak R, stopband width, field distribution) is foundational for 
VCSEL and superconducting qubit readout resonator design
<img width="474" height="257" alt="image" src="https://github.com/user-attachments/assets/160e3ddd-a0f8-4de9-bb6b-853bd0db68f6" />


# Tech stack
Vanilla HTML / CSS / JavaScript — no build tools, no framework
Chart.js for the reflectance spectrum and E-field bar chart
All TMM physics computed in real time


Context: built for fun while i was taking a photonics module in uni.
