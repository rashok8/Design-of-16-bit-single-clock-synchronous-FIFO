# Design-of-16-bit-single-clock-synchronous-FIFO
Designed single clock (n+1) and n bit FIFO with 4bit Write and Read pointer. Accounted for RACE condition in the design. 
 FIFO Memory Verilog Implementation 

 Description: 
This repository contains Verilog code for implementing a First In, First Out (FIFO) memory structure. The FIFO memory is a crucial component in digital systems for managing data flow in a sequential manner. This Verilog implementation provides a modular design for easy integration into FPGA projects.

 Files: 
1. `fifo_mem.v`: Top-level Verilog module defining the FIFO memory interface and instantiating submodules for write pointer, read pointer, memory array, and status signals.
2. `memory_array.v`: Verilog submodule for storing and retrieving data based on pointers.
3. `read_pointer.v`: Verilog submodule for managing the read pointer and controlling read operations.
4. `status_signal.v`: Verilog submodule for calculating status signals such as FIFO full, empty, overflow, and underflow.
5. `write_pointer.v`: Verilog submodule for managing the write pointer and controlling write operations.

 Usage: 
To integrate this FIFO memory module into your Verilog project, follow these steps:
1. Include the necessary Verilog files (`fifo_mem.v`, `memory_array.v`, `read_pointer.v`, `status_signal.v`, and `write_pointer.v`) in your project directory.
2. Instantiate the `fifo_mem` module in your top-level design, connecting the appropriate input and output ports.
3. Ensure that the clock (`clk`), reset (`rst_n`), write enable (`wr`), read enable (`rd`), data input (`data_in`), and data output (`data_out`) signals are connected correctly.
4. Simulate and verify the functionality of the FIFO memory module using a Verilog simulation tool such as ModelSim or Vivado Simulator.
5. Synthesize the design and implement it on your target FPGA platform.

 Contributing: 
Contributions to this Verilog implementation are welcome. If you find any bugs, issues, or have suggestions for improvements, please open an issue or pull request on GitHub.

 License: 
This Verilog code is provided under the [MIT License](LICENSE), allowing for both personal and commercial use with proper attribution.

 Author: 
This FIFO memory Verilog implementation was developed by Ritwik Ashok

