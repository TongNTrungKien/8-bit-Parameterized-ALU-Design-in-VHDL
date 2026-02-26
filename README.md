8-bit-Parameterized-ALU-Design-in-VHDL

An 8-bit parametric Arithmetic Logic Unit (ALU) was developed using VHDL in a digital system environment for an FPGA based application.

The ALU supports a total of 16 possible functions and uses a 4-bit control signal to choose from the 16 function available to the ALU, which include, but are not limited to, arithmetic, logic, shifting/rotating and comparing. The design of this project is compliant with IEEE by utilizing the numeric_std library found within VHDL to assure proper and portable arithmetic calculations among various EDA tools.

The most significant feature of this design is the use of a generic parameter to configure the shifting and rotating functions which allows for reuse and scalability of these functions without modifying internal logic. Carry and borrow functions are designed through the use of extended 9-bit reasoning to establish if an overflow has occurred.

The ALU is purely combinational and was verified with a self-checking testbench (that uses assert-based verification techniques) written in VHDL. The design also successfully synthesizes to a clean RTL schematic (in Xilinx Vivado) that contained no timing or synthesis errors.

This project has given me a great deal of experience related to datapath design, implementing combinational logic, and creating VHDL for verification purposes.
