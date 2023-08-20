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
 <summary>Labs on examples of iverilog and gtkwave </summary>
Iverilog is an open-source tool used in digital circuit design. It enables simulation and testing of designs written in HDLs like Verilog and SystemVerilog.
GTKWave is an open-source waveform viewer used in digital circuit design. It helps users visualize and analyze simulation results by displaying signal values over time. It's valuable for debugging, signal analysis, and signal comparison.

We created a directory named as siddhant.v and the cloned vsdflow repostry as well as we cloned sky130RTLDesignAndSynthesisWorkshop repostry. These repostitories contains  the necessary .lib files and verilog design files and testbeches for practice.
The screenshots of RTL Design code, Testbench and gtkwave viewer are shown as follows:

RTL Design code :-
<img width="1085" alt="good_latch" src="https://github.com/Sidv005/Samsung-PD-Training/blob/44f51a59e7ccacf4af7dfd90e3d56e24c0f36174/good_latch.PNG">

Testbench :-

<img width="1085" alt="good_latch" src="https://github.com/Sidv005/Samsung-PD-Training/blob/274dd505c6fc92029359f0d6e71789f4fae34644/tb_good_latch.PNG">

Output Waveform :-

<img width="1085" alt="good_latch" src="https://github.com/Sidv005/Samsung-PD-Training/blob/d232cb70dbc4dccb461917b6a79e4d62559db1fc/gtk_good_latch.PNG">
</details>

<details>
 <summary>Fundamentals of Yosys </summary>
Synthesis: In Very Large Scale Integration (VLSI) design, synthesis is a crucial step that transforms a high-level hardware description (RTL) into an optimized gate-level netlist. This process involves logic optimization, technology mapping, and creating a gate-level representation using a target technology library. Timing constraints are applied to meet performance requirements, and clock tree synthesis ensures proper clock distribution. Verification ensures correctness, and the output is a gate-level netlist that serves as the foundation for physical design. Synthesis plays a vital role in bridging the gap between functional design and physical implementation, impacting factors like performance, power efficiency, and manufacturability.

Yosys is an open-source tool suite used for Verilog RTL synthesis and formal verification in digital circuit design. It converts high-level Verilog descriptions into optimized gate-level netlists, offers optimization and technology mapping, supports formal verification, and provides scripting capabilities. 

Faster cells vs Slower cells:- Faster cells are requried to take care of setup violaton and improves performance but comes up with a drawback of larger area and high power consumption whereas slower cells takes control of hold violations and has benefits of less area and low power consumption but lags in performance.
</details>

<details>
 <summary>Labs on Yosys </summary>
Overwiew of Yosys tool is explained to us. Later on implementation of latch is demonstrated and gate level netlist is genrated. Command used for generating graphical representation are as follows:
 read_liberty -lib <.lib path>
  
 read_verilog<RTL_design >
 
 For synthesis : synth -top<module_name>
  
 To generate netlist: abc -liberty<.lib path>
 
 "show" command is used to view the graphical representation of netlist generated. 
<img width="1085" alt="netlist_graph" src="https://github.com/Sidv005/Samsung-PD-Training/blob/863e8e2726d04a43ad749d2b72a31ab01b21925c/netlist_graph.PNG">
  
The Netlist code is following:
<img width="1085" alt="netlist_ini" src="https://github.com/Sidv005/Samsung-PD-Training/blob/9c9468c78babff96e0e25143a4c2d96d641e55d3/netlist_ini.PNG">
  
 After simplification the switched netlist code is shown below:
<img width="1085" alt="netlist_switched" src="https://github.com/Sidv005/Samsung-PD-Training/blob/6e71349c6cea71f31b30a9feb915b27596a2d638/netlist_switched.PNG">
</details>

