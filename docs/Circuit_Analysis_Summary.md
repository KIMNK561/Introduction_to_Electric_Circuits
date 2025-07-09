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

### 💡 Mapping Equivalent Resistance: Simplifying a Complex Resistor Network

1. **Mark all nodes** as distinct dots or circles  
2. **Draw resistors as lines** connecting these nodes

<img src="../images/MappingResistor.jpg" alt="Resistor map" width="700"/>
  
## Design Using Op-Amp

To design with operational amplifiers, it is helpful to **memorize common configurations** that relate input(s) to output based on the desired signal behavior.

<img src="../images/commonopamp1.jpg" alt="Op-Amp Classic Configurations" width="1000"/>

<img src="../images/commonopamp2.jpg" alt="Op-Amp Design Examples" width="1000"/>

## Practical Op-Amp

In real life, an op-amp is not ideal. Several **non-ideal models** can be considered depending on the required accuracy.

<img src="../images/practical_opamp_model.jpg" alt="Practical Op-Amp Model" width="1000"/>

> 💡 Bias current, input offset voltage, voltage gain and internal resistances for a practical op-amp vary by model and can be referenced from standard datasheets or textbooks.

## Frequency Response

### Gain

The **gain** of a system refers to the **ratio of output to input amplitudes**:

- **Linear scale**:  
  \[
  \text{Gain} = \frac{\text{Output}}{\text{Input}}
  \]

- **Decibels (dB)**:  
  Use 10log when dealing with **power**, and 20log when dealing with **voltage or current**, assuming the load impedance is constant.

### Bode Plot

A **Bode plot** displays the **gain (in dB)** and **phase (in degrees)** of a **network function** versus the **logarithm of frequency**.

The **exact magnitude Bode plot** is a smooth curve that accurately represents the frequency response (**drawn as a solid blue line**).  
The **asymptotic magnitude Bode plot** is a piecewise linear approximation (**drawn as a black dashed line**).

<img src="../images/bode_vs_asymptotic.jpg" alt="Bode vs Asymptotic Plot" width="1000"/>

> 💡 **Definition-wise, the Bode plot is the exact magnitude and phase plot. But in most practical contexts, "sketching" the Bode plot refers to drawing the asymptotic approximation.**

### Corner Frequency vs. Break Frequency

- **Corner frequency**:  
  The frequency at which the gain drops to  
  \[
  \frac{1}{\sqrt{2}} \times \text{maximum gain}
  \]  
  It often occurs when \( \omega \to 0 \) or \( \omega \to \infty \) gives the maximum gain.

- **Break frequency**:  
  The frequency at which the **asymptotic magnitude Bode plot** changes slope.

> 💡 In simple systems, these frequencies are often the same, but they are conceptually different.
