# Samsung-PD-Training
## Day-0-Installation

<details>
 <summary>icc2_shell </summary>
"ICC2" stands for "Integrated Circuit Compiler 2," which is a place-and-route tool developed by Synopsys. The ICC2_shell is likely the command-line interface or graphical user interface (GUI) through which engineers and designers interact with the ICC2 tool.
I invoked icc2_shell using the following command: icc2_shell
Below is the screenshot showing sucessful launch:
<img width="1085" alt="icc2_shell" src="https://github.com/Sidv005/Samsung-PD-Training/blob/9132f919f1b97fafb5a77a49d680d8d767232e17/SamsungPD%23Day0/icc2_shell.png">
</details>

<details>
 <summary>dc_shell </summary>
The "dc_shell" tool provides a command-line interface for performing logic synthesis. Designers use this tool to read in the HDL description of their design, specify optimization constraints, and generate the gate-level netlist.
I invoked dc_shell using the following commands: dc_shell
Below is the screenshot showing sucessful launch:
<img width="1085" alt="dc_shell" src="https://github.com/Sidv005/Samsung-PD-Training/blob/32946b9e5b01c48e7e3ea5e00f246180e8ce5419/SamsungPD%23Day0/dc_shell.png">
</details>

<details>
 <summary>lc_shell </summary>
The Synopsys Library Compiler tool is designed to capture ASIC (Application-Specific Integrated Circuit) libraries and convert them into Synopsys' internal database format, suitable for physical synthesis, or into VHDL format, which is compatible with simulation processes.
I invoked lc_shell using the following commands: lc_shell
Below is the screenshot showing sucessful launch:
<img width="1085" alt="lc_shell" src="https://github.com/Sidv005/Samsung-PD-Training/blob/70cb8795964d3ef80b73d1e016eaf5bf6b8315b8/SamsungPD%23Day0/lc_shell.png">
</details>

<details>
 <summary>pt_shell </summary>
PrimeTime is an essential Electronic Design Automation (EDA) tool developed by Synopsys. It's used for analyzing and optimizing the timing performance of digital integrated circuits. By evaluating signal propagation delays, setup times, and other factors, PrimeTime helps designers ensure that circuits operate reliably and meet performance targets.
I invoked pt_shell using the following commands: pt_shell
Below is the screenshot showing sucessful launch:
<img width="1085" alt="pt_shell" src="https://github.com/Sidv005/Samsung-PD-Training/blob/70cb8795964d3ef80b73d1e016eaf5bf6b8315b8/SamsungPD%23Day0/pt_shell.png">
</details>

<details>
 <summary>iverilog </summary>
Iverilog is an open-source tool used in digital circuit design. It enables simulation and testing of designs written in HDLs like Verilog and SystemVerilog. 
I invoked iverilog using the following commands: iverilog
Below is the screenshot showing sucessful launch:
<img width="1085" alt="iverilog" src="https://github.com/Sidv005/Samsung-PD-Training/blob/6a01e81a5310edd8e0ee2e8719fc0d3b0204f026/SamsungPD%23Day0/iverilog.PNG">
</details>

<details>
 <summary>gtkwave </summary>
GTKWave is an open-source waveform viewer used in digital circuit design. It helps users visualize and analyze simulation results by displaying signal values over time. It's valuable for debugging, signal analysis, and signal comparison.
I invoked gtkwave using the following commands: gtkwave
Below is the screenshot showing sucessful launch:
<img width="1085" alt="gtkwave" src="https://github.com/Sidv005/Samsung-PD-Training/blob/6a01e81a5310edd8e0ee2e8719fc0d3b0204f026/SamsungPD%23Day0/gtkwave.PNG">
</details>

<details>
 <summary>yosys </summary>
Yosys is an open-source tool suite used for Verilog RTL synthesis and formal verification in digital circuit design. It converts high-level Verilog descriptions into optimized gate-level netlists, offers optimization and technology mapping, supports formal verification, and provides scripting capabilities. 
I invoked yosys using the following commands: yosys
Below is the screenshot showing sucessful launch:
<img width="1085" alt="yosys" src="https://github.com/Sidv005/Samsung-PD-Training/blob/6a01e81a5310edd8e0ee2e8719fc0d3b0204f026/SamsungPD%23Day0/yosys.PNG">
</details>

## Day-1-Introduction to Verilog RTL Design and Synthesis
<details>
 <summary>Introduction to RTL_Design, Testbench and Simulator </summary>
Register Transfer Level (RTL): In digital design and computer engineering, RTL refers to a high-level abstraction that describes the flow of data between registers in a digital circuit or microprocessor. It's an important step in the design process before actual circuitry is created.


TestBench: A testbench is a virtual environment where digital designs are thoroughly tested and validated through simulation. It's an essential part of the design process, helping to catch bugs and design flaws before the hardware is physically fabricated.

Simulator: A simulator for RTL (Register Transfer Level) design is a software tool used to simulate and verify the behavior of digital circuits and systems described at the RTL abstraction level. RTL simulators play a crucial role in verifying the correctness and functionality of digital designs before they are implemented in actual hardware.
</details>

<details>
 <summary>dc_shell </summary>
The "dc_shell" tool provides a command-line interface for performing logic synthesis. Designers use this tool to read in the HDL description of their design, specify optimization constraints, and generate the gate-level netlist.
I invoked dc_shell using the following commands: dc_shell
Below is the screenshot showing sucessful launch:
<img width="1085" alt="dc_shell" src="https://github.com/Sidv005/Samsung-PD-Training/blob/32946b9e5b01c48e7e3ea5e00f246180e8ce5419/SamsungPD%23Day0/dc_shell.png">
</details>

<details>
 <summary>lc_shell </summary>
The Synopsys Library Compiler tool is designed to capture ASIC (Application-Specific Integrated Circuit) libraries and convert them into Synopsys' internal database format, suitable for physical synthesis, or into VHDL format, which is compatible with simulation processes.
I invoked lc_shell using the following commands: lc_shell
Below is the screenshot showing sucessful launch:
<img width="1085" alt="lc_shell" src="https://github.com/Sidv005/Samsung-PD-Training/blob/70cb8795964d3ef80b73d1e016eaf5bf6b8315b8/SamsungPD%23Day0/lc_shell.png">
</details>

<details>
 <summary>pt_shell </summary>
PrimeTime is an essential Electronic Design Automation (EDA) tool developed by Synopsys. It's used for analyzing and optimizing the timing performance of digital integrated circuits. By evaluating signal propagation delays, setup times, and other factors, PrimeTime helps designers ensure that circuits operate reliably and meet performance targets.
I invoked pt_shell using the following commands: pt_shell
Below is the screenshot showing sucessful launch:
<img width="1085" alt="pt_shell" src="https://github.com/Sidv005/Samsung-PD-Training/blob/70cb8795964d3ef80b73d1e016eaf5bf6b8315b8/SamsungPD%23Day0/pt_shell.png">
</details>

<details>
 <summary>iverilog </summary>
Iverilog is an open-source tool used in digital circuit design. It enables simulation and testing of designs written in HDLs like Verilog and SystemVerilog. 
I invoked iverilog using the following commands: iverilog
Below is the screenshot showing sucessful launch:
<img width="1085" alt="iverilog" src="https://github.com/Sidv005/Samsung-PD-Training/blob/6a01e81a5310edd8e0ee2e8719fc0d3b0204f026/SamsungPD%23Day0/iverilog.PNG">
</details>

<details>
 <summary>gtkwave </summary>
GTKWave is an open-source waveform viewer used in digital circuit design. It helps users visualize and analyze simulation results by displaying signal values over time. It's valuable for debugging, signal analysis, and signal comparison.
I invoked gtkwave using the following commands: gtkwave
Below is the screenshot showing sucessful launch:
<img width="1085" alt="gtkwave" src="https://github.com/Sidv005/Samsung-PD-Training/blob/6a01e81a5310edd8e0ee2e8719fc0d3b0204f026/SamsungPD%23Day0/gtkwave.PNG">
</details>

<details>
 <summary>yosys </summary>
Yosys is an open-source tool suite used for Verilog RTL synthesis and formal verification in digital circuit design. It converts high-level Verilog descriptions into optimized gate-level netlists, offers optimization and technology mapping, supports formal verification, and provides scripting capabilities. 
I invoked yosys using the following commands: yosys
Below is the screenshot showing sucessful launch:
<img width="1085" alt="yosys" src="https://github.com/Sidv005/Samsung-PD-Training/blob/6a01e81a5310edd8e0ee2e8719fc0d3b0204f026/SamsungPD%23Day0/yosys.PNG">
</details>
