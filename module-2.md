# Diode Circuits and Power supplies

## Circuit modelling of PN Junction Diodes

- Mathematical modelling
  - [Shockley Diode Equation](https://en.wikipedia.org/wiki/Shockley_diode_equation)
  - $I_D = I_0\left[e^{\frac{V_D}{\eta V_T} - 1}\right]$
  - $I_D$ terminal current
  - $V_D$ terminal voltage
  - $V_T$ = $\frac{kT}{q}$
    - $k$ = boltzmann constant
    - $q$ = magnitude charge of electron
    - $T$ = temperature
  - $I_0$ = reverse saturation current
    - Heavy temperature dependence
      - For Si, doubles every 10 degree kelvin
  - $\eta$ = Process Ideality Factor (aka ideality factor)
    - For Ge $\approx$ 1
    - For Si $\approx$ 2
    - For other practical diodes in between 1 and 2
    - Caculated based on curve fitting data
- In Forward Bias: Closed Switch
- In Reverse Bias: Open Switch
- DC Resistance (aka static resistance) = $R_{DC} = \frac{V_D}{I_D}$
- AC Resistance (aka dynamic resistance) = $R_{AC} = \frac{dV}{dI} \approx \frac{\eta V_T}{I_D}$
- $R_{avg} = \frac{\Delta V_D}{\Delta I_D}$ 
- 1% approximation

Avalanche breakdown (at higher voltages like 30V)
in zener diodes (high doping): still avalanche breakdown at lower voltages (like 5V)

<!-- 23/01/2025 -->
Examples:

Q1
- compute the current through the diode assuming R_avg of diode is much smaller compared to given resistance (assuming 1% approximation)

Q2
- the forward bias voltage needed to turn on the white led shown for the given circuit is 4 V
- the breakdown voltage of these zener diodes z1 and z2 are 6v and 3.3 v resp.
- calculate for this circuit
  - the current flowing thorough all the diodes by neglecting the diode resistances and their operations
    - I = 20 mA
  - ratio of references voltages v01 and v02
  -  ratio of power dissipated in white led to that zener diode z1
  - power delieverd by the dc supply present in the circuit

## Application of Diodes

- Power Supplies
  - e.g Regulated Power Supply
    - step down
    - AC -> DC (Rectification)
    - Unregulated DC -> DC Regulated DC
    - e.g. Chargers for Laptop and Mobile Phones

- Voltage regulation
  - e.g.
    For the circuit given in the diagram assume that 
    Rs = 10kohm
    Rl = 5kohm
    Vz = 6V
    PZmax = 7.2mW
    Vsmin = 18V
    Vsmax = 30V
    find the range of values for the input voltage Vn, where the circuit generates a constant regulated DC voltage
  - e.g.
    Design a zener  regulator circuit to obtain a regulated voltage of 3.3 V across load resistance, for a given input voltage of Vin fo 5V
    for the design, assume that you have been provided with a zener diode with a breakdown voltage of 3.3 V, and a maximum power dissipation limit of 100 mW.
    Design the circuit subject to the following design constraints:
      - current flowing through the load resistance is 1 mA
      - power dissipated in zener diodes is 25% of max power dissipation limit of the device
      - give your final design in terms of a circuit diagram with all the values mentioned in it


