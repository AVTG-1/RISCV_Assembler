# RISC-V Assembler  

RISC-V Assembler is a lightweight assembler that translates 32-bit RISC-V assembly instructions into machine code. It reads an input assembly file (`.asm` format) and generates a corresponding machine code output (`.mc` format), supporting core RISC-V instruction formats (R, I, S, SB, U, UJ) and basic assembler directives.  

## Features  
- **Instruction Translation**: Converts 31 essential RISC-V instructions into their binary equivalents.  
- **Address Calculation**: Automatically assigns memory addresses for instructions and data.  
- **Data Segment Handling**: Supports `.text`, `.data`, `.byte`, `.half`, `.word`, `.dword`, and `.asciz` directives for data storage.  
- **Label Resolution**: Parses labels in the assembly code and replaces them with appropriate memory addresses.  

## Project Structure  
- **`main.cpp`** - Entry point of the assembler, manages file I/O and overall processing.  
- **`InstructionSet.cpp/.h`** - Defines the supported RISC-V instructions and their encoding formats.  
- **`call_IS.cpp`** - Handles instruction parsing and calls the appropriate encoding functions.  
- **`DataSegment.cpp`** - Manages data segment allocation and processing.  
- **`inputDataSeg.asm`** - Sample input assembly file for testing data segment functionality.  
- **`outputDataSeg.txt`** - Generated machine code output from the assembler.  
- **`LICENSE`** - License file for the repository.  
- **`a.out`** - Compiled output binary (for reference).
