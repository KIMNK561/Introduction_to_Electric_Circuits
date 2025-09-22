# Op-amp Notes

Today’s topic can be summarized in one sentence: “We can make a circuit act like a signal operator using an operational amplifier.”

A signal is a voltage or current that represents a quantity such as temperature, pressure, or sound. An operator is a symbol indicating a specific calculation, such as +, −, d/dt, or ∫. With different circuit designs, we can add, subtract, differentiate, and integrate signals.

For example, suppose we want

$$ v_o = 4v_x + v_y + \tfrac{1}{2}v_z + 4 $$

It is not obvious how many operations are required just by looking at the equation, so we use a block diagram to show the signal flow. The operators here are multiplication by 4, multiplication by 1, multiplication by 1/2, and summation (Σ). If you memorize the corresponding circuits for these operators, you can design a circuit to produce the desired output from the inputs.

However, an op-amp does not work properly unless certain conditions are satisfied:

$$ |v_o| < V_{sat}, \quad |i_o| < I_{sat}, \quad \left|\frac{d v_o}{dt}\right| < SR $$

The corresponding circuits are usually derived under the assumption of an ideal op-amp. In reality, op-amps have finite gain, input and output resistance, offset voltage, bias current, limited CMRR, and finite bandwidth. Considering these makes the model more accurate but also slows down calculation, so we choose the level of detail depending on the purpose.

When applying KCL to a circuit with an op-amp, we need to be careful at the output node. The out
