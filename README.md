## Experiment No: 6
MONOSTABLE MULTIVIBRATOR USING 555 TIMER 
## Aim
To design and simulate a Monostable Multivibrator using NE555 in Proteus Design Suite and verify the time duration of the output pulse.
## Apparatus Required
•	NE555 Timer IC
•	Resistor R = 100 kΩ
•	Capacitor C = 10 µF
•	Push Button (Trigger)
•	DC Power Supply (5V or 9V)
•	CRO / Oscilloscope
•	Connecting wires
## Circuit Diagram
Pin Connections:
•	Pin 1 → Ground
•	Pin 2 → Trigger (Connected to push button)
•	Pin 3 → Output
•	Pin 4 → Reset (Connected to Vcc)
•	Pin 5 → Control Voltage (Optional 0.01 µF capacitor to ground)
•	Pin 6 → Threshold
•	Pin 7 → Discharge
•	Pin 8 → Vcc
## Circuit Connections:
<img width="1031" height="542" alt="Screenshot 2026-03-09 081620" src="https://github.com/user-attachments/assets/6683e26f-19ab-4aff-95d5-8a2a700a8bb9" />

•	Resistor R → Between Vcc and Pin 7
•	Capacitor C → Between Pins 6 & 7 and Ground
•	Trigger → Pin 2
•	Output → Pin 3
## Theory
A Monostable Multivibrator has only one stable state and one quasi-stable state. It produces a single output pulse when triggered externally.
In monostable mode:
•	The circuit remains in stable LOW state.
•	When a negative trigger pulse is applied at Pin 2 (below 1/3 Vcc), the output becomes HIGH.
•	The capacitor starts charging through resistor R.
•	When capacitor voltage reaches 2/3 Vcc, the output returns to LOW state automatically.
Thus, a single pulse is generated for a fixed time duration.
The NE555 operating in monostable mode acts as a one-shot pulse generator. It has one stable state and one quasi-stable state. Normally, the output remains LOW. When a negative trigger pulse is applied to the trigger pin (Pin 2) below 1/3 Vcc, the output becomes HIGH and remains HIGH for a fixed time interval. During this period, the capacitor connected in the circuit charges through the resistor. When the capacitor voltage reaches 2/3 Vcc, the output automatically returns to LOW state. The pulse width of the output is determined by the resistor and capacitor values and is given by the expression T=1.1RCT = 1.1 RCT=1.1RC. Thus, the 555 timer in monostable mode produces a single output pulse for each trigger input and is widely used in timer and delay applications.
## Procedure
1.	Open Proteus software.
2.	Select NE555 timer, resistor, capacitor, push button, and CRO.
3.	Connect circuit in monostable configuration.
4.	Apply 5V supply.
5.	Press trigger button.
6.	Observe output pulse on CRO.
7.	Measure pulse width.
## Tabulation
| **S.No** | **R (kΩ)** | **C (µF)** | **Theoretical Pulse Width** | **Practical Pulse Width** |
| -------- | ---------- | ---------- | --------------------------- | ------------------------- |
| 1        | 100        | 10         | 1.1 sec                     | 1.07 sec                  |
| 2        | 100        | 22         | 2.43 sec                    | 2.40 sec                  |
| 3        | 150        | 10         | 1.65 sec                    | 1.61 sec                  |

## Waveform
<img width="1037" height="640" alt="Screenshot 2026-03-09 081643" src="https://github.com/user-attachments/assets/f4510fb8-595e-47c0-9af9-7a39d1b4b171" />

•	Trigger → Short negative pulse
•	Output → Single positive pulse
•	Capacitor voltage → Exponential charging waveform
## Result
The Monostable Multivibrator using NE555 Timer IC was successfully designed and simulated in Proteus.
A single output pulse of duration approximately 1.1 seconds was obtained.
The practical value closely matches the theoretical value.
## Conclusion
•	The circuit produces one output pulse for each trigger.
•	Pulse width depends on R and C values.
•	Increasing R or C increases pulse duration.
•	Used in timers, delay circuits, and pulse generation applications.
## Viva Questions
1. What is a monostable multivibrator? A monostable multivibrator is a circuit that has one stable state and one quasi-stable state. When a trigger pulse is applied, the circuit switches to the quasi-stable state for a fixed time and then automatically returns to its stable state.
2. Write the pulse width formula. The pulse width of a monostable multivibrator using a 555 timer is given by T = 1.1 RC where R is the resistance and C is the capacitance connected to the circuit.
3. What is the stable state of monostable? In a monostable circuit, the stable state is the condition in which the output remains LOW until a trigger pulse is applied.
4. Why is it called “one-shot”? It is called a one-shot because the circuit produces only one output pulse for each triggering input signal.
5. What happens if capacitor value increases? If the capacitance value increases, the pulse width increases because the capacitor takes more time to charge, resulting in a longer output pulse.

