# Operational Amplifier

Today’s topic can be summarized in one sentence: **“We can make a circuit act like a signal operator using an operational amplifier.”**
A signal is a voltage or current that represents a quantity such as temperature, pressure, or sound. An operator is a symbol indicating a specific calculation, such as $$+$$, $$−$$, $$\tfrac{d}{dt}$$, or $$\int$$. With different circuit designs, we can add, subtract, differentiate, and integrate signals.
For example, suppose we want
$$ v_o = 4v_x + v_y + \tfrac{1}{2}v_z + 4 $$
It is not obvious how many operations are required just by looking at the equation, so we use a **block diagram** to show the signal flow. The operators here are multiplication by 4, multiplication by 1, multiplication by 1/2, and summation (Σ). If you memorize the **corresponding circuits** for these operators, you can design a circuit to produce the desired output from the inputs.
<img src="../images/commonopamp1.jpg" alt="Op-Amp Classic Configurations" width="800"/>
<img src="../images/commonopamp2.jpg" alt="Op-Amp Design Examples" width="800"/>
The corresponding circuits are usually derived under the assumption of an **ideal op-amp**  . In reality, op-amps have finite gain, input and output resistance, offset voltage, bias current, limited CMRR, and finite bandwidth. Considering these makes the model more accurate but also slows down calculation, so we choose the level of detail depending on the purpose.
<img src="../images/practical_opamp_model.jpg" alt="Practical Op-Amp Model" width="800"/>
An op-amp does not work properly unless certain conditions are satisfied:

$$ |v_o| < V_{sat}, \quad |i_o| < I_{sat}, \quad \left|\frac{d v_o}{dt}\right| < SR $$

When applying **KCL** to a circuit with an op-amp, we need to be careful at the output node. The output current $$i_{o}$$ is supplied internally by the op-amp’s voltage source, and if we do not know its value, the equation only adds an unknown variable instead of helping with analysis.
