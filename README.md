# **VLSI Project**
## NMOS
### Voltage Transfer Characteristics/ DC transfer characteristics (VTC Curve)
-  Schematic
![id-vgs-schematic](https://github.com/DevinduDh/VLSI/assets/76746921/67988b57-a323-40dd-b8ec-27f88d5e847d)

- Graphs
  #### I_D vs V_DS graph
![id-vgs](https://github.com/DevinduDh/VLSI/assets/76746921/ba4c9f6f-701f-43fd-955c-28a10901f055)

  #### I_D vs V_GS graph
  ![id-vgs1](https://github.com/DevinduDh/VLSI/assets/76746921/3d05363e-fa08-4a6a-aa7e-a0ff4bd61212)
# CMOS INVERTER

-  Schematic
![cmos-schematic](https://github.com/DevinduDh/VLSI/assets/76746921/b789add5-c4e5-4842-99f8-b3794c2b66a5)


-   Graphs


-   Layout

Tools used:- CADENCE Virtuoso <br>
PDK used:- gpdk 45

Firstly, NMOS and PMOS lengths are kept at 50nm and widths are varied using parametric analysis to make rise and fall transition equal.

<br>

# CMOS Latch comparison

| Latch          | Functionality                                    | Good                                                                                   | Bad                                                                                                                     |
|----------------|--------------------------------------------------|----------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------|
| (a) [Latch Image](url_to_image_a)           | Transparent latch                                | Compact, fast operation                                                                | Limited output swing (not rail-to-rail), dynamic output (floats when opaque), exposed state node, potential noise issues  |
| (b) [Latch Image](url_to_image_b)           | Improved with CMOS transmission gate            | Rail-to-rail output swings, requires complementary clock                                 | Requires additional clock signal (K), increased complexity                                                            |
| (c) [Latch Image](url_to_image_c)           | Inverting latch with output inverter            | Isolates state node from output noise                                                    | Inverts output, requires additional inverter, potential delay increase                                                  |
| (d) [Latch Image](url_to_image_d)           | Inverting latch with buffered input              | Fast operation, simplified structure                                                     | Inverts output, potential delay increase, unbuffered output                                                             |
| (e) [Latch Image](url_to_image_e)           | Staticized latch with feedback                   | Prevents output from floating, adds stability                                           | Output noise sensitivity, potential state corruption                                                                   |
| (f) [Latch Image](url_to_image_f)           | Staticized latch with input inverter             | Fast and compact inverting latch                                                        | Output noise sensitivity, potential state corruption                                                                   |
| (g) [Latch Image](url_to_image_g)           | Robust static latch                               | Static operation, rail-to-rail swings, isolates state noise from output noise              | More complex design, potentially larger area footprint                                                                 |
| (h) [Latch Image](url_to_image_h)           | Inverting latch for semicustom datapath          | Faster and more compact design for controlled noise environments                         | Inverts output, potential delay increase, may not be suitable for all applications                                       |
| (i) [Latch Image](url_to_image_i)           | Jamb latch with weak feedback inverter           | Reduces clock load, saves transistors, improved design for specific applications           | Requires careful design for feedback inverter strength, potential noise issues                                            |
| (j) [Latch Image](url_to_image_j)           | Jamb latch for register files and FPGAs          | Suitable for specific applications like register files and FPGAs                           | Requires careful control of Dout signal, potential noise issues                                                         |
| (k) [Latch Image](url_to_image_k)           | Latch used in Itanium 2 processor               | Static feedback, optimized for specific processor requirements                            | Requires strong gate driving input, potentially complex design                                                          |
|                |                                                  |                                                                                         |                                                                                                                         |





