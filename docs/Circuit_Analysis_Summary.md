## Energy Absorption & Supply in Circuit Elements

Whether a circuit element **absorbs** or **supplies** energy depends on the **reference direction of voltage** with respect to the direction of current.

<img src="../images/Energyflow.jpg" alt="Energy Flow" width="400"/>

## Voltage Sign in Resistors

The voltage across a resistor depends on the reference direction of voltage and the direction of current.

<img src="../images/RVDresistor.jpg" alt="RVDresistor" width="400"/>

Combining the energy absorption in circuit elements and voltage sign in resistors, we can conclude:

> 💡 **A resistor with positive resistance always absorbs energy, regardless of the reference directions of voltage and current.**

## Equivalent Circuit

If replacing a part of the circuit (B) with another circuit (C) does **not change** the voltage or current of any element in the remaining circuit (A),  
then **C is said to be the equivalent circuit of B**, and vice versa.

<img src="../images/equivalent_circuit.jpg" alt="Equivalent Circuit Concept" width="500"/>


## Design Using Op-Amp

To design with operational amplifiers, it is helpful to **memorize common configurations** that relate input(s) to output based on the desired signal behavior.

<img src="../images/commonopamp1.jpg" alt="Op-Amp Classic Configurations" width="1500"/>

<img src="../images/commonopamp2.jpg" alt="Op-Amp Design Examples" width="1500"/>

## Practical Op-Amp

In real life, an op-amp is not ideal. Several **non-ideal models** can be considered depending on the required accuracy.

<img src="../images/practical_opamp_model.jpg" alt="Practical Op-Amp Model" width="1500"/>

> 💡 Bias current, input offset voltage, voltage gain and internal resistances for a practical op-amp vary by model and can be referenced from standard datasheets or textbooks.
