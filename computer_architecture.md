# Computer architecture

## Universal machine model
Contains:
- a memory: contains instructions and data
- an arithmetic and logical unit (ALU): performs the calculations
- an input/output unit: information exchange (I/O) with devices
- a control unit: control (UC)

## The Control Unit:
1. extracts an instruction from the memory,
2. analyzes the instruction,
3. searches the memory for the relevant data,
4. triggers the appropriate operation on the ALU or I/O,
5. stores the result in memory.

## Signal and chronogram
- A signal is a discrete quantity belonging to [0,1].
- A chronogram is the graphical representation of a signal evolving over time.

## Registers
- Fast memory elements internal to the CPU.
- A signal commands storage: ▪ level loading,
- front loading.

## Bus
▪ Set of electrical wires on which the signals pass through.
▪Connects the units to each other.
▪Bus width:
▪ number of wires constituting the path,
▪ number of signals that can be sent at the same time.

## Memory
▪Vector in which each component is accessible through an address.
▪Permitted transactions: ▪ Read,
▪ Write.
▪ Word = unit of information accessible in a single reading operation.

## How it works
1. The CPU writes the address of a cell in an address register (AR).
2. The CU is requesting an operation.
3. Exchanges are made via a word register (WR).
**Write**      
Read AR ← address       
WR ← value       
memory[AR]← WR      
**Read**      
AR ← address       
WR ← memory[AR]     


## ALU

▪3-parameter function: ▪ 1 operation
▪ 2 arguments ▪ 1 result
▪Requires a or some storage registers: ▪ inputs, outputs,
▪ intermediate results.
        