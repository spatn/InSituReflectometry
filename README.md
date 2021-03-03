# InSituReflectometry
Code for Arduino in-situ laser reflectometer utilizing stroboscopic effect

This code is for Arduino driven refelctometer that utilizes stroboscopic effect.
The setup consists of a laser diode, a photodiode or light-dependent resistor, and an Arduino board.

It allows to measure evaporation of a solvent in-situ during spin-coating. The laser diode flashes like a strobe. The flash frequency can be adjusted to match the spin-coater speed. Thanks to the programmed flashing, the laser light always shines on the same spot on the rotating disc. 

Adjustment of the stroboscope frequency: F(t-t0)/k + F0
F(t-t0) := phase_conv((tk + time_shift)
F0 := phase_shift
k is period multiplier, allows to make measurment every T/k, T - period of one disc rotation

Condition to flash the light is phase_conv((tk + time_shift) / k) + phase_shift <= RPM_phase(RPM)

https://doi.org/10.26434/chemrxiv.14054033 - supporting data

