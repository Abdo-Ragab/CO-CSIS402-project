# CO-CSIS402-project
Logisim implementation of Mano’s Basic Computer with a custom control unit and MUL instruction, designed to execute a loop-based arithmetic program for Computer Organization coursework.

# Modified Mano Basic Computer in Logisim

This project implements a modified version of Mano's Basic Computer using Logisim as part of the Computer Organization and Systems Programming course at the German University in Cairo.

The processor was redesigned with a custom control unit to execute a specific assembly program involving arithmetic, logical operations, looping, and memory manipulation.

## Features

- Custom control unit implementation:
  - Instruction decoder
  - Sequence counter
  - Timing and control logic
- Supported instructions:
  - LDA
  - AND
  - ADD
  - STA
  - ISZ
  - BUN
  - MUL (custom instruction)
- Program-specific execution cycle optimization
- Bus control and datapath integration
- Memory preloaded with machine code

## Program Executed

```c
int A, B, C, i;

for (i = 0; i < 3; i++) {
    C += A & B;
    A += A * B;
}
