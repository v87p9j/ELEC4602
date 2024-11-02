java c
ELEC4602
Microelectronics
Design and Technology
Design Project: level translating buffer — term 3, 2024
Problem
The aim of this project is, for teams of two students, to design a level translating buffer in the usual FreePDK 45 nm CMOS process used in the course. Parameters for hand calculations, simulation parameters, and layout design rules can be found on the course website.
Design requirements
The purpose of the level translating buffer is to take an analogue input signal with a voltage swing exceeding the chip supply voltages (VIn ∈ [−5V; 5V]) and linearly scale and shift this to a signal with a voltage range comfortably between the chip power supply voltages (VOut ∈ [0.5V; 1.5V]) – i.e. a signal reference shift from 0V to VGG = 1V and a gain of G = dVOut/dVIn = 0.1 (or −0.1). Further, a logic gain control signal (VG) must set the gain to G = 0.2 (or −0.2) if High (mapping VIn ∈ [−2.5V; 2.5V] to VOut ∈ [0.5V; 1.5V]). The circuit must be able to process DC signals. The input signal source resistance is unknown but in the range RS ∈ [10 kΩ; 100 kΩ]. Finally, the circuit must use a single-ended supply of VDD = 3.3V and must drive a grounded load resistance of RL = 10 kΩ. A reference voltage VRef and a reference current IRef are available if desired, as is a logic power supply VLL = 0.9V. The design requirements to the circuit are summarised in figure 1.

Figure 1: Design requirements summary.
The circuit performance is to be evaluated using the test-setup in figure 2; the circuit itself must contain only NMOS and PMOS transistors (of any variation available in the process), capacitors (MIMC) and resistors (POLYR). MI1 (P THKOX) and MI2 (N THKOX) shown in the test-setup are ESD protection devices and have dimensions WI1 = WI2 = 500µm and LI1 = LI2 = 0.25µm. (Other than these, package and I/O parasitics are ignored in this design project). A POLYR resistor RIn of any desired value may be placed between the source resistance RS and the level shifting buffer; this resistor is considered part of the design.
Other than the above, there are no design constraints: you are free to choose circuit architecture, circuit bandwidth, design methodology, etc; you may代 写ELEC4602 Microelectronics Design and Technology 2024
代做程序编程语言 also make use of circuits – or variations of circuits – designed in the labs (e.g. op-amp structure or logic gates). However, the cir-cuit must be evaluated according to the following performance measure, quoted in the unit of MHz/(mW·mV· µm2), which should be as large as possible:

where f0 is the 3 dB bandwidth at maximum, undistorted output voltage, PSup =VDDIDD+VLLILL (average) is the circuit power consumption, VOS is the worst-case output referred offset volt-age (VOS = max|VOut −1V| when VIn = 0V), αG is the worst-case gain error (defined as αG = max|1−|Gactual/Gideal||), and ALO is an estimate of the required layout area, calculated thus:

where WiLiis the gate area of transistor i, Cjis the capacitance of capacitor j, and Rk is the resistance of resistor k.

Figure 2: Performance test-bench.
Note that the design requirements are very open; there are many solutions to the problem (which makes this a good engineering exercise), some good, some not so good. The same can be said about the requirements to the report. It is left for the students to judge what makes up a good design, good supporting simulations and a convincing report, keeping the following in mind: the report must answer all questions asked and implied in the project description, it must document the work done, and it must show that the authors understand the material. Also note that any illegible material will be considered incorrect.
Work
The following work is expected to be carried out:
• choice of circuit topology,
• design of analogue and digital circuit components (including simple hand calculations on critical functions),
• circuit simulations that verifies circuit operation/requirements and that allows the perfor-mance measure to be calculated,
• a written report documenting the work done.
Report
Requirements to the report include:
• one report per group,
• inclusion of complete schematic with transistor sizes,
• inclusion of relevant simulation plots,
• reasoning for design choices,
• reasoning for transistor sizes,
• calculation of performance measure, and
• submission in .pdf format.





         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
