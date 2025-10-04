# 4-bit-Adder
4-bit Adder using ICs
🔢 4-Bit Adder Using Logic ICs
This 4-bit binary adder is a modular digital circuit designed to perform addition of two 4-bit binary numbers. Built entirely from fundamental logic gates, it showcases the core principles of combinational logic and arithmetic processing.

🔧 Key Components:

XOR Gates: Used to compute the sum bits by performing bitwise exclusive OR between input bits and carry-in.

AND Gates: Generate carry outputs by detecting when both input bits are high.

OR Gates: Combine multiple carry signals to propagate the final carry-out across bit stages.

🧠 Architecture Overview:

The adder consists of four full-adder modules, each handling one bit of the input.

Each full-adder is constructed using XOR, AND, and OR ICs, such as:

74LS86 for XOR logic

74LS08 for AND logic

74LS32 for OR logic

Inputs: Two 4-bit binary numbers (A₃A₂A₁A₀ and B₃B₂B₁B₀) and an initial carry-in (C₀).

Outputs: A 4-bit sum (S₃S₂S₁S₀) and a final carry-out (C₄).

📐 Functionality:

Each bit stage computes:

Sum = A ⊕ B ⊕ Carry-in

Carry-out = (A AND B) OR (Carry-in AND (A ⊕ B))

This design is ideal for demonstrating low-level digital logic, and can be extended to larger bit-widths or integrated into ALU modules for embedded systems or FPGA projects.
