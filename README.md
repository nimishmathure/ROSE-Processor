# ROSE RISC-V Out-Of-Order Superscalar Execution Processor
(Source code will be uploaded soon)

ROSE is a 32-bit RISC-V out-of-order superscalar processor core. The key features are as follows:

- ISA
  - Supports RV32I Base Instruction Set.
  - Partial support for RV32M Standard Extension.

- Microarchitecture
  - 2-fetch front-end and 3-issue execution
  - Up to 32 instructions can be in-flight.
  - A speculative instruction scheduler.
  - Speculative OoO load/store execution.
  - Non-blocking L1 data cache.

- Implementation
  - Written in Verilog.
  - Can be simulated with Modelsim.
  - Can be synthesized.
![alt text](https://github.com/nimishmathure/ROSE-Processor/blob/main/Images/ROSE%20Processor%20Diag%202.jpg)

## ReOrder Buffer
- Each line can hold upto 2 instructions
- Tries to commit as many instructions as possible from a line in each clock cycle (Max 2 commits per cc)
![alt text](https://github.com/nimishmathure/ROSE-Processor/blob/main/Images/ROSE%20ROB.jpg)

## Register File
- 32 Bits registers
- Dual write ports
  - If matching addresses then Write B has higher priority. 
- Quad read ports
![alt text](https://github.com/nimishmathure/ROSE-Processor/blob/main/Images/ROSE%20Register%20File.jpg)
