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
Overwiew of Yosys tool is explained to us. Later on implementation of latch is demonstrated and gate level netlist is generated. 
 
Firstly, Yosys is invoked using "yosys" command. the screenshot is shown below:
<img width="1085" alt="netlist_graph" src="https://github.com/Sidv005/Samsung-PD-Training/blob/7ec89b24e4a07e8257d00e4b1f45b11704c11dec/yosys_2.PNG">
  
 Commands used for generating graphical representation are as follows:
 
 read_liberty -lib <.lib path>
  
 read_verilog<RTL_design >
 
 For synthesis : synth -top<module_name>
  
 To generate netlist: abc -liberty<.lib path>
 
 "show" command is used to view the graphical representation of netlist generated. 
<img width="1085" alt="netlist_graph" src="https://github.com/Sidv005/Samsung-PD-Training/blob/863e8e2726d04a43ad749d2b72a31ab01b21925c/netlist_graph.PNG">
  
The Netlist code is following:
<img width="1085" alt="netlist_ini" src="https://github.com/Sidv005/Samsung-PD-Training/blob/9c9468c78babff96e0e25143a4c2d96d641e55d3/netlist_ini.PNG">
  
 After simplification the switched netlist code is shown below:
<img width="1085" alt="netlist_switched" src="https://github.com/Sidv005/Samsung-PD-Training/blob/ba0dad6c41800ed06227bd23f4accb5649efb3ab/netlist_switched.PNG">
</details>

## Day-2-Timing libs,hierarchical vs flat synthesis and efficient flop coding styles
<details>
 <summary>Introduction to timing .libs </summary>
When it comes to digital design and RTL (Register Transfer Level) descriptions, timing is crucial to ensure the correct operation of the designed circuit. Timing analysis is essential to verify that signals propagate correctly and meet timing constraints. The standard library that we use is sky130_fd_sc_hd_tt_025C_1v80.lib, from this we can observe synthesis will be performed for 130 nm technology . here tt denotes process is typical , 025C indicates temperature is 25 deg Celcius and 1v80 shows that voltage is 1.8V. Cells list can be shown by using following commands :
 
 **gvim ../lib/sky130_fd_sc_hd_tt_025C_1v80.lib**
 
 **:/cell**
 
 **:g//**
 
 Below is screenshot of standard library :
 <img width="1085" alt="cell_list" src="https://github.com/Sidv005/Samsung-PD-Training/blob/6c505b0ebf4d2da86a7de3b3c7eaa97a9b48e0dc/SamsungPD%23day2/cell_list.png">
  For each gate cell 2^N input combinations are possible for N no. of inputs. Different leakage power, area and various parameters are displayed as per their combinations. Comparison of power consumption of different flavours of same gate is shown below:
  <img width="1085" alt="cell_list" src="">
</details>

<details>
 <summary>Hierarchical vs Flat synthesis </summary>
Hierarchical synthesis: Hierarchical synthesis is a design methodology used in digital design to manage complex projects effectively. It involves breaking down a design into smaller modules or hierarchies, synthesizing each module separately, and then integrating them at the top level. This approach offers modularity, reusability, parallelism, and better optimization. Challenges include defining module interfaces and achieving timing closure. Modern EDA tools support hierarchical synthesis, making it easier to handle large and intricate digital designs. Furthermore, multiple_modules.v RTL code is synthesized. The image of   multiple_modules.v RTL code is presented below:
<img width="1085" alt="multiple_modules_code" src="https://github.com/Sidv005/Samsung-PD-Training/blob/551d8b32d1ccf8f89ea945cad50698966c109016/SamsungPD%23day2/multiple_modules_code.png">
 In this image submodule 1 shows AND gate and submodule 2 shows OR gate. Now yosys is invoked for synthesis and after technology mapping netlist generated in graphical form is shown in below figure.
 <img width="1085" alt="multiple_netlist_graph" src="https://github.com/Sidv005/Samsung-PD-Training/blob/551d8b32d1ccf8f89ea945cad50698966c109016/SamsungPD%23day2/multiple_netlist_graph.png">
 
 **write_verilog -nioattr multiple_modules_hier.v**
 
 **!gvim multiple_modules_hier.v**

 The above two commands are used to generate optimized netlist code. The obtained netlist code is present below:
 ```ruby
module multiple_modules(a, b, c, y);
  input a;
  input b;
  input c;
  wire net2;
  output y;
  sub_module2 u1 (
    .a(a),
    .b(b),
    .y(net2)
  );
  sub_module3 u2 (
    .a(net2),
    .b(c),
    .y(y)
  );
endmodule

module sub_module1(a, b, y);
  wire _1_;
  wire _2_;
  wire _3_;
  input a;
  input b;
  output y;
  sky131_fd_sc_hd__and2_0 _3_ (
    .A(_2_),
    .B(_1_),
    .X(_3_)
  );
  assign _2_ = b;
  assign _1_ = a;
  assign y = _3_;
endmodule

module sub_module2(a, b, y);
  wire _0_;
  wire _1_;
  wire _2_;
  input a;
  input b;
  output y;
  sky130_fd_sc_hd__or2_0 _3_ (
    .A(_1_),
    .B(_0_),
    .X(_2_)
  );
  assign _1_ = b;
  assign _0_ = a;
  assign y = _2_;
endmodule
```
From this we can observe that submodules are instantiated but gate cells are not synthesized.

*Flat synthesis* : Flat synthesis for netlist involves synthesizing a digital design without hierarchical division into modules. It treats the entire design as a single entity, simplifying the synthesis process but potentially sacrificing optimization and modularity. While suitable for smaller designs or interim steps, it may not achieve the same level of efficiency as hierarchical synthesis, which is preferred for complex designs. Furthermore, yosys is evoked and flat synthesis is performed by applying following commands :
**read_liberty -lib <.lib path>**
**read_verilog multiple_modules.v**
**synth -top multiple_modules**
**abc -liberty <.lib path>**
**flatten**
**show**
Here **multiple_modules.v** is RTL Design file and **multiple_modules** is instance name which is synthesized in our case. The below figure shows the generated circuit of flattened netlist in graphical form.
 <img width="1085" alt="flat_netlist_graph" src="https://github.com/Sidv005/Samsung-PD-Training/blob/ac0e7bc26ca2a12ebd8a5dd4a181261a1b20e965/SamsungPD%23day2/flat_netlist_graph.png">
**write_verilog -noattr multiple_modules_flat.v**
**!gvim multiple_modules_flat.v**
the above commands are used to write and display the optimized flat netlist code. Below figure represents the flat netlist code.
<img width="1085" alt="multiple_flat" src="https://github.com/Sidv005/Samsung-PD-Training/blob/c93c6a224747b8a3317eea687e1706cfdc2dfd3a/SamsungPD%23day2/multiple_flat.png">
From analysis we can conclude that a single module having gate level instantiation is obtained through flat netlist code. Furthermore, for better comparison between hierarchical and flat synthesis below figure is presented.
<img width="1085" alt="split_flat_hier" src="https://github.com/Sidv005/Samsung-PD-Training/blob/c93c6a224747b8a3317eea687e1706cfdc2dfd3a/SamsungPD%23day2/split_flat_hier.png">
Synthesis at the sub-module level is a powerful strategy in digital design, where designs are divided into functional sub-modules, each synthesized individually for optimization and then integrated into the complete system. This approach enhances modularity, accelerates development, and results in well-optimized designs. The command used to synthesize **sub_module1** is :-

**synth -top sub_module1**
The following figure shows the synthesized ciruit of generated netlist of the sub_module1
<img width="1085" alt="submodule1_netlist_graph" src="https://github.com/Sidv005/Samsung-PD-Training/blob/c93c6a224747b8a3317eea687e1706cfdc2dfd3a/SamsungPD%23day2/submodule1_netlist_graph.png">
</details>

<details>
 <summary>Coding styles of flops </summary>
 
*Flip-flops* are essential components in digital logic design used to store binary information (0 or 1). They have inputs for data and clock signals and outputs representing the stored value and its complement. Different types, including SR, JK, D, and T flip-flops, offer various functionalities like setting, resetting, toggling, and capturing data on clock edges. Flip-flops play a key role in sequential logic circuits, counters, shift registers, and more, forming the basis for storing and manipulating data in digital systems.
 
 *Why Flops?*
 In combinational circuit every component has its propogation delay and due to this the output gets untypically chaged may lead to momemtary 0 or momentary 1 also called as glitches. In complex combinational circuit this glitch will amplify and will get transported to the results. Therefore, multiple flops are designed and connected in between the circuits to remove the glitches.  
 
Flip-flops are used in sequential circuits to store state and allow for memory retention, while combinational circuits rely on logic gates and other combinational components to perform operations solely based on the current input values.
 
**Asynchronous Reset D flop:-**
In Asynchronous reset flop whenever the reset pin goes high output "**q**"  becomes **0** regardless of the incoming active clock edge. The suitable RTL code is given below:

```ruby
module dff_asyncres ( input clk ,  input async_reset , input d , output reg q );
always @ (posedge clk , posedge async_reset)
begin
	if(async_reset)
		q <= 1'b0;
	else	
		q <= d;
end
endmodule
```
Simulation:
<img width="1085" alt="waveform_dff_async_reset" src="https://github.com/Sidv005/Samsung-PD-Training/blob/1572b0278337747b51585c19b2a515556be9f657/SamsungPD%23day2/waveform_dff_async_reset.png">

Synthesized Netlist:
<img width="1085" alt="dff_async_reset_netlist" src="https://github.com/Sidv005/Samsung-PD-Training/blob/1572b0278337747b51585c19b2a515556be9f657/SamsungPD%23day2/dff_async_reset_netlist.png">

**Asynchronous Set D flop:-**
In Asynchronous Set flop whenever the set pin goes high output "**q**"  becomes **1** regardless of the incoming active clock edge. The suitable RTL code is given below:

```ruby
module dff_async_set ( input clk ,  input async_set , input d , output reg q );
always @ (posedge clk , posedge async_set)
begin
	if(async_set)
		q <= 1'b1;
	else	
		q <= d;
end
endmodule
```
<img width="1085" alt="dff_async_reset_netlist" src="https://github.com/Sidv005/Samsung-PD-Training/blob/1572b0278337747b51585c19b2a515556be9f657/SamsungPD%23day2/dff_async_reset_netlist.png">
</details>
