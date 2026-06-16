![top-level schematic](pic/tt_um_cw_testbuffer.png)


## How it works

A testbuffer that will buffer a voltage signal and drive a off-chip probe.

## How to test

- Bias the amplifier with a 5uA current from pin ua[1].
- Apply test signal to input pin ua[0] 
- Measure buffered signal at the output pin ua[2].

## External hardware

- Oscilloscope and function generator or voltage source and multimeter


## Specifications

| Parameter                        | Symbol.  | Min.      | Typ.     | Max.      | Unit.       | Condition                        |
| :------------------------------- | :------- | :-------: | :------: | :-------: | :---------: | :------------------------------- |
| Supply voltage                   | Vdd      | 3.0       | 3.3      | 5.0       | V           |                                  |
| Temperature range                | T        | 0         |          | 75        | °C          |                                  |
| Area                             | A        |           |          | 90x82     | µm²         |                                  |
| Load capacitance                 | Cl       |           | 10       | 50        | pF          |                                  |
| Load resistance                  | Rl       |           | 1        |           | MΩ          |                                  |
| Bias current                     | Ib       |           | 5        |           | µA          |                                  |
| Supply current                   | Idd      | 46.6      | 49.1     | 56.2      | µA          | Ib = 5µA, All PVT, Rl = 1MΩ      |
| Power consumption                | Pd       | 139       | 162      | 280       | µW          | Ib = 5µA, All PVT, Rl = 1MΩ      |
| Input offset voltage             | Vos      |           | 9.54     |           | mV          | +-3σ, Vdd = 3.3V, T = 27°C       |
| Integrated noise                 | eni      | 30.9      | 36.3     | 42.3      | µVrms       | f = 0.1Hz to 1MHz                |
| Input referred noise             | en       | 9.39      |          | 11.45     | µV/sqrt(Hz) | f = 0.1Hz, All PVT               |
|                                  |          | 0.926     |          | 1.129     | µV/sqrt(Hz) | f = 10Hz,  All PVT               |
|                                  |          | 95.6      |          | 116.3     | nV/sqrt(Hz) | f = 1kHz,  All PVT               |
| Open loop gain                   | Avol     | 83.5      | 85.1     | 88.2      | dB          | All PVT, Rl=1MΩ                  |
| Unity gain bandwidth             | UGBW     | 2.32      | 2.97     | 4.49      | MHz         | All PVT, Cl=10pF                 |
| Phase margin                     | φm       | 65.7      | 75.1     | 84.16     | °           | All PVT, Cl=10pF, Rl=1MΩ         |
| Slew rate                        | SR       | 1.2       | 1.72     |           | MV/s        | All PVT, Cl=10pF                 |
| Input Capacitance                | Cin      | 61.7      | 67.2     | 70.4      | fF          | All PVT                          |
| Power supply rejection ratio pos | PSRR+    | 104       | 123      | 129       | dB          | f = 1Hz,   All PVT               |
|                                  |          | 88        | 89       | 91        | dB          | f = 100Hz, All PVT               |
|                                  |          | 68        | 69       | 71        | dB          | f = 1kHz,  All PVT               |
| Power supply rejection ratio neg | PSRR-    | 101       | 115      | 159       | dB          | f = 1Hz,   All PVT               |
|                                  |          | 78        | 79       | 81        | dB          | f = 10kHz, All PVT               |
| Input common mode range max      | ICMR+    | vdd-0.086 | vdd-0.03 | vdd-0.016 | V           | All PVT, condition: Avol <= 60dB |
| Input common mode range min      | ICMR-    | 0.34      | 0.58     | 0.71      | V           | All PVT, condition: Avol <= 60dB |
| Common common rejection ratio    | CMRR     | 86        | 89       | 109       | dB          | All PVT                          |

