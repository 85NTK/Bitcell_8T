# Bitcell_8T
Analysis And Design Bitcell 8t Using 130nm Technology
## Definition
Bitcell 8T is a basic component of memory circuits used to store one bit or data (0 or 1)
## Structure
Bitcell 8T is a type of data storage circuit (SRAM), consist of 8 transistor with 2 PMOS transistor and 6 NMOS transistor, connected together to store one bit or data
![Bitcell_8T](/FLOWCHART/Bitcell_8T.png)
## Operating
- Write '0': to write '0', BL (Bit line) must provide 0 volts and VDD to BLB (Bit line bar). And WWL (write word line) is confirmed to make both the M3 and M4 transistors ON. Therefore, the value in the bitstream is stored at Q and '0' is stored at Q
- Write '1':when writing '1' BL (Bit line) must provide a VDD value and BLB (Bit line bar) is provided with a value of 0 volts. When WWL (write word line) is enabled for write operations, the values in the bitlines stored at the corresponding nodes at Q will have a logic value of '1' and logic '0' at Qbar
- Read '0': the reading operation is initiated by pre-loading the RBL (Read bit line) into the VDD. RWL (Read word line) controls the M5 transistor ON. If the value stored at Q is '0' then the M6 transistor will be ON and the RBL (Read bit line) is grounded directly through the M5&M6 transistor discharges. This means that the value stored at Q in SRAM is zero
- Read '1': If the value stored at Q is '1', the M6 transistor will be OFF and there is no discharge line for the RBL, and the value in the RBL is VDD indicating that the value stored at Q is '1'
## Calculation Parameters
