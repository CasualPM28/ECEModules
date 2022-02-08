README for Linear Voltage Regulator
@Vincent Agostino Del Tufo, 916328545

Linear Voltage Regulator:

The design taken for the adjustable linear voltage regulator is that of taking in an unregulated voltage via the input, making sure it is smooth and free of noise (as much as possible)
with bypass capacitors, feeding it into the LM317H 3.3V voltage regulator, and then taking the output regulated voltage, smoothing it out again, and outputting it into the main circuit.
However, unlike the linear voltage regulator, this system is adjustable. The implementation of an adjustable voltage was done through a 10k Ohm potentionmeter and a 240 Ohm resistor.
Using the voltage division rule, Vout = Vin (R2/(R2+R1)), one can find their desired voltage output according to the output. The tolerance levels of the potentiometer should align with
how much the potentiometer is turned. For example, at 50% tolerance, the output voltage of 3.3V should be 1.65V. The design was done so in a way that allowed it to be compact and easy
to look at. From an electronics standpoint, the circuit makes use of few parts to accomplish the goal of adjustable voltage regulation, making it part-efficient and cost effective.

Dataset Used, LM317H:
https://www.ti.com/lit/ds/symlink/lm317a.pdf?HQS=dis-mous-null-mousermode-dsf-pf-null-wwe&ts=1644210301708&ref_url=https%253A%252F%252Fwww.mouser.com%252F

Parts Used:
1uF Capacitor             - x1
0.1uF Capacitor           - x1
LM317H Voltage Regulator  - x1
10k Ohm Potentiometer     - x1
240 Ohm Resistor          - x1

How to import design into new DipTrace schematic:

1.) Open the schematic in DipTrace alongside the new circuit.
2.) Copy the entire design with Ctrl+A and Ctrl+C.
3.) Paste the design into the project on a new sheet.
4.) Rename sheet to "Adjustable 3.3v Voltage Regulator" and turn the sheet into a hierarchical block under "Edit" -> "Sheet Type" -> "Hierarchy Block".