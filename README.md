![Microchip logo](images/microchip.png)

# Current to Voltage converter circuit using OPA of PIC16F17146 Mindi Simulation

**Note : Currently, this repository contains Mindi model of PIC18-Q41 family's OPAMP module. Mindi model of PIC16F17146 family's OPAMP module will be available soon.**

In this example, the OPA module of PIC16F17146 is used to convert force sensing resistor output to voltage using non-inverting amplification configuration. This circuit can be described as a current to voltage converter. This Mindi simulation simulates the circuit described in the  [Force Sensing Resistor interface using PIC16F17146 Code Examples](https://github.com/microchip-pic-avr-examples/pic16f17146-force-sensing-resistor-interface-mplab-mcc). The simulation consists of a model of the PIC16F17146 OPA module and generic components representing the rest of the functionality of the circuit. For more information about getting started with and using the MPLAB Mindi Analog Simulator please refer to the following resources:
- [Using the MPLAB Mindi Analog Simulator with the 8-Bit Operational Amplifier Module Technical Brief](https://www.microchip.com/DS90003293)
- [Microchip Developer - Introduction to MPLAB Mindi Analog Simulator](https://www.microchipdeveloper.com/mindi:mindi-analog-simulator-introduction)
- [Getting Started with the MPLAB Mindi Analog Simulator Document](https://www.microchip.com/DS50002564)

![Circuit](images/ExampleCircuit.svg)

## Related Documentation

* [PIC16F17146 Product Page](https://www.microchip.com/PIC16F17146)
* [PIC16F17146 Data Sheet](https://www.microchip.com/DS40002343)
* [PIC16F17146 Curiosity Nano User Guide](https://www.microchip.com/)

## Related Software
* [Force Sensing Resistor interface using PIC16F17146 Code Examples](https://github.com/microchip-pic-avr-examples/pic16f17146-force-sensing-resistor-interface-mplab-mcc)

### Mindi Simulation
![Mindi](images/mplab-mindi-analog-simulator.png)

Download and open the **Mindi schematic [here](https://github.com/microchip-pic-avr-examples/pic16f17146-current-to-voltage-conveter-using-OPA-mindi/releases/latest)**

Press the _play_ button to simulate with an example stimulus source.

### Tweaking
User can tweak the value of FSR resistor (which is variable in nature) representing the applied force over the surface area of sensor. The given simulation example is having 10 points.

There is a specific parameters: 
* The overall gain can be controlled by changing the value of feedback resistor R2.
* The offset can be changed by changing the value of VDD/2 supply. 

### Don't have Mindi?
You can download and install the [Mindi simulation tool](https://www.microchip.com/mplab/mplab-mindi), or use another SPICE simulator of your own preference. For use with different simulators, a plain spice model can be found in "Opamp_PIC18_Q41.txt" to replace the mindi-optimized "Opamp_PIC18_Q41.lb " 