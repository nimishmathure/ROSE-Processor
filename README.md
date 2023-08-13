# ROSE RISC-V Out-Of-Order Superscalar Execution Processor
ROSE is a 32-bit RISC-V out-of-order superscalar processor core. The key features are as follows:

-ISA
  -Support RV32IMF

-Microarchitecture
  -2-fetch front-end and 3-issue execution
  -Up to 32 instructions are in-flight.
  -A speculative instruction scheduler.
  -Speculative OoO load/store execution.
  -Non-blocking L1 data cache.

-Implementation
  -Written in SystemVerilog
  -Can be simulated with Modelsim
  -Can be synthesized
![alt text](https://github.com/nimishmathure/ROSE-Processor/blob/main/Images/ROSE%20Processor%20Diag%201.jpg)
