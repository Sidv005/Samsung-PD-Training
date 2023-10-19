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
When it comes to digital design and RTL (Register Transfer Level) descriptions, timing is crucial to ensure the correct operation of the designed circuit. Timing analysis is essential to verify that signals propagate correctly and meet timing constraints. The standard library that we use is **sky130_fd_sc_hd_tt_025C_1v80.lib**, from this we can observe synthesis will be performed for 130 nm technology . here tt denotes process is typical , 025C indicates temperature is 25 deg Celcius and 1v80 shows that voltage is 1.8V. Cells list can be shown by using following commands :
 
 **gvim ../lib/sky130_fd_sc_hd_tt_025C_1v80.lib**
 
 **:/cell**
 
 **:g//**
 
 Below is screenshot of standard library :
 <img width="1085" alt="cell_list" src="https://github.com/Sidv005/Samsung-PD-Training/blob/6c505b0ebf4d2da86a7de3b3c7eaa97a9b48e0dc/SamsungPD%23day2/cell_list.png">
For each gate cell 2^N input combinations are possible for N no. of inputs. Different leakage power, area and various parameters are displayed as per their combinations.
</details>

<details>
 <summary>Hierarchical vs Flat synthesis </summary>
	
*Hierarchical synthesis*: Hierarchical synthesis is a design methodology used in digital design to manage complex projects effectively. It involves breaking down a design into smaller modules or hierarchies, synthesizing each module separately, and then integrating them at the top level. This approach offers modularity, reusability, parallelism, and better optimization. Challenges include defining module interfaces and achieving timing closure. Modern EDA tools support hierarchical synthesis, making it easier to handle large and intricate digital designs. Furthermore, multiple_modules.v RTL code is synthesized. The image of   multiple_modules.v RTL code is presented below:
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
Simulation:
<img width="1085" alt="waveform_async_set" src="https://github.com/Sidv005/Samsung-PD-Training/blob/c96e3f23d1c872c0baa6f4e48b51d022285bdb18/SamsungPD%23day2/waveform_async_set.png">

Synthesized Netlist:
<img width="1085" alt="dff_async_set_netlist" src="https://github.com/Sidv005/Samsung-PD-Training/blob/c96e3f23d1c872c0baa6f4e48b51d022285bdb18/SamsungPD%23day2/dff_async_set_netlist.png">

**Synchronous Reset D flop:-**
In Synchronous reset flop a 2:1 mux is implemented before flop. In this flop when the active clock edge arrives condition is checked if **sync_reset** pin is high the output "**q**"  becomes **0** otherwise it follows the behavior of input **d** . The suitable RTL code is given below:

```ruby
module dff_syncres ( input clk , input async_reset , input sync_reset , input d , output reg q );
always @ (posedge clk )
begin
	if (sync_reset)
		q <= 1'b0;
	else	
		q <= d;
end
endmodule
```
Simulation:
<img width="1085" alt="waveform_async_set" src="https://github.com/Sidv005/Samsung-PD-Training/blob/c96e3f23d1c872c0baa6f4e48b51d022285bdb18/SamsungPD%23day2/waveform_dff_sync_reset.png">

Synthesized Netlist:
<img width="1085" alt="dff_async_set_netlist" src="https://github.com/Sidv005/Samsung-PD-Training/blob/c96e3f23d1c872c0baa6f4e48b51d022285bdb18/SamsungPD%23day2/dff_sync_reset_netlist.png">
</details>

<details>
 <summary>Interesting Optimization Techniques </summary>
Here we will discuss about special cases where additional hardwares are not required to implement the circuit. For instance consider a design where 3bit number is multipied by 2. Here we need connecting bits to the output and LSB is needed to be grounded. RTL code of multipying by 2 is shown below:
	
```ruby
module mul2 (input [2:0] a, output [3:0] y);
	assign y = a * 2;
endmodule
```
For multipying any no. by 2 shifting the bits to left and appending extra bit as 0 is needed to be done. Same is described through synthesized netlist circuit as seen below:

<img width="1085" alt="mult2_netlist" src="https://github.com/Sidv005/Samsung-PD-Training/blob/6e28ddc230185ce2d77a588dbb28051e9717a353/SamsungPD%23day2/mult2_netlist.png">

Generated netlist code is presented in the following figure:
<img width="1085" alt="mult2_netlist_code" src="https://github.com/Sidv005/Samsung-PD-Training/blob/6e28ddc230185ce2d77a588dbb28051e9717a353/SamsungPD%23day2/mult2_netlist_code.png">
Consider another special case where any no. is multipied by 9. The RTL Design code is given below:

```ruby
module mult8 (input [2:0] a , output [5:0] y);
	assign y = a * 9;
endmodule
```
The synthesized netlist circuit is shown in the following figure:
<img width="1085" alt="mult8_netlist" src="https://github.com/Sidv005/Samsung-PD-Training/blob/6e28ddc230185ce2d77a588dbb28051e9717a353/SamsungPD%23day2/mult8_netlist.png">
The generated netlist code is represented by the below image.
<img width="1085" alt="mult8_netlist_code" src="https://github.com/Sidv005/Samsung-PD-Training/blob/6e28ddc230185ce2d77a588dbb28051e9717a353/SamsungPD%23day2/mult8_netlist_code.png">
</details>

## Day-3-Intoduction to Optimizations

<details>
 <summary>Combinational Logic Optimization with examples </summary>
	
**Combinational Logic Optimization** This term refers to squeezing of logic to get best possible optimized designin terms of area and power saving. This divided in two categories as follows:-
*constant propogation* also called Direct Propogation example - Consider output Y=(A+B)' if implemented using CMOS technology it will have 6 MOS transistors but it can also be simplified if an input A=0 then only 2 MOS  transistors are used for implementation.
*Boolean Logic Optimization* which are analysed using K-Map and Quine McKluskey. For instance consider a statement y=a?(b?c:(c?a:0)):!c this will contain 3 2x1 mux but after simplification y=a xnor c i.e. 1 xnor gate is sufficient to implement the logic.

**opt_clean -purge** : this command is used to optimize circuit in yosys.

**Example 1**: For opt_check1.v file
```ruby
module opt_check (input a, input b,output y);
  assign y= a?b:0;
endmodule
```
<img width="1085" alt="opt_check_circuit" src="https://github.com/Sidv005/Samsung-PD-Training/blob/c9bc447d8675e0b8f10f8a4fea6b5d3070e11ad1/SamsungPD/%23day3/opt_check_circuit.png">

The generated netlist code is mentioned in the following image. The command used is **write_verilog opt_check_netlist.v**
<img width="1085" alt="opt_check_netlist_code" src="https://github.com/Sidv005/Samsung-PD-Training/blob/1046d1469b68aab2d132e038bafb6b03d7e0019d/SamsungPD/%23day3/opt_check_netlist_code.png">

**Example 2**: For opt_check2.v file
```ruby
module opt_check (input a , input b , output y);
   assign y = a?1:b;
endmodule
```
Synthesized circuit is shown in below figure.
<img width="1085" alt="opt_check1_circuit" src="https://github.com/Sidv005/Samsung-PD-Training/blob/5557de567020067bae2496c8ff77c3cf54e8152a/SamsungPD/%23day3/opt_check1_circuit.png">

The generated netlist code is mentioned in the following image. The command used is **write_verilog opt_check2_netlist.v**
<img width="1085" alt="opt_check2_netlist_code" src="https://github.com/Sidv005/Samsung-PD-Training/blob/1046d1469b68aab2d132e038bafb6b03d7e0019d/SamsungPD/%23day3/opt_check2_netlist_code.png">

**Example 3** For opt_check3.v file
```ruby
module opt_check3 (input a , input b, input c , output y);
   assign y = a?(c?b:0):0;
endmodule
```
Synthesized circuit is shown in below figure.
<img width="1085" alt="opt_check3_circuit" src="https://github.com/Sidv005/Samsung-PD-Training/blob/1046d1469b68aab2d132e038bafb6b03d7e0019d/SamsungPD/%23day3/opt_check3_circuit.PNG">

The generated netlist code is mentioned in the following image. The command used is **write_verilog opt_check3_netlist.v**
<img width="1085" alt="opt_check3_netlist_code" src="https://github.com/Sidv005/Samsung-PD-Training/blob/1046d1469b68aab2d132e038bafb6b03d7e0019d/SamsungPD/%23day3/opt%E2%80%AD_check3_netlsit_code.png">

**Example 4** For opt_check3.v file
```ruby
module opt_check4 (input a , input b , input c , output y);
   assign y = a?(b?(a & c ):c):(!c);
endmodule
```
Synthesized circuit is shown in below figure.
<img width="1085" alt="opt_check_circuit" src="https://github.com/Sidv005/Samsung-PD-Training/blob/1046d1469b68aab2d132e038bafb6b03d7e0019d/SamsungPD/%23day3/opt_check4_circuit.png">

The generated netlist code is mentioned in the following image. The command used is **write_verilog opt_check4_netlist.v**
<img width="1085" alt="opt_check4=_netlist_code" src="https://github.com/Sidv005/Samsung-PD-Training/blob/1046d1469b68aab2d132e038bafb6b03d7e0019d/SamsungPD/%23day3/opt_check4_netlist_code.png">

**Example 5** Optimize multimodule (RTL file name- multiple_module_opt.v). 
The following commands are used for generating the netlist in possible optimized form  :

**read_liberty -lib <library_path>**

**read_verilog <verilog_file>**

**synth -top <module_name>**

**flatten**

**opt_clean -purge**

**abc -liberty <library_path>**

```ruby
module sub_module1(input a , input b , output y);
	 assign y = a & b;
	endmodule

	module sub_module2(input a , input b , output y);
	 assign y = a^b;
	endmodule

	module multiple_module_opt(input a , input b , input c , input d , output y);
	wire n1,n2,n3;
	sub_module1 U1 (.a(a) , .b(1'b1) , .y(n1));
	sub_module2 U2 (.a(n1), .b(1'b0) , .y(n2));
	sub_module2 U3 (.a(b), .b(d) , .y(n3));

	assign y = c | (b & n1); 
	endmodule
```
Before flatten
<img width="1085" alt="before_flat_multiple_module__circuit" src="https://github.com/Sidv005/Samsung-PD-Training/blob/0b83c1033ea83fb3523aa6e996bb86fadeb6c9b7/SamsungPD/%23day3/before_flat_multiple_module__circuit.PNG">
After flatten
<img width="1085" alt="before_flat_multiple_module__circuit" src="https://github.com/Sidv005/Samsung-PD-Training/blob/0b83c1033ea83fb3523aa6e996bb86fadeb6c9b7/SamsungPD/%23day3/after_flat_multiple_module_circuit.PNG">

**Example 6** Optimize multimodule (RTL file name- multiple_module_opt2.v). 
```ruby
module sub_module(input a , input b , output y);
	assign y = a & b;
endmodule

module multiple_module_opt2(input a , input b , input c , input d , output y);
	wire n1,n2,n3;
	sub_module U1 (.a(a) , .b(1'b0) , .y(n1));
	sub_module U2 (.a(b), .b(c) , .y(n2));
	sub_module U3 (.a(n2), .b(d) , .y(n3));
	sub_module U4 (.a(n3), .b(n1) , .y(y));
endmodule
```
Before flatten
<img width="1085" alt="before_flat_multiple_module_opt2_circuit" src="https://github.com/Sidv005/Samsung-PD-Training/blob/0b83c1033ea83fb3523aa6e996bb86fadeb6c9b7/SamsungPD/%23day3/before_flat_multiple_module_opt2_circuit.PNG">

After flatten
<img width="1085" alt="after_flat_multiple_module_opt2_circuit" src="https://github.com/Sidv005/Samsung-PD-Training/blob/0b83c1033ea83fb3523aa6e996bb86fadeb6c9b7/SamsungPD/%23day3/after_flat_multiple_module_opt2_circuit.PNG">
</details>

<details>
 <summary>Sequential Logic optimization </summary>
 There are few techniques for Sequential Logic Optimization which are as follows:
 BASIC (Sequential Constant Propogation)
 ADVANCED (State Optimization, Retiming, Sequential Logic cloning)

 *Sequential Constant Propogation*
 Considering a asynchronous reset D Flip-flop is fed with D = 0 (i.e Ground). Here output y is always 1 so no need of gates.
<img width="1085" alt="hand_write_dff_const" src="https://github.com/Sidv005/Samsung-PD-Training/blob/8a0fc3e0728ce7bb23438d3d1a5703ca9b4ce921/SamsungPD/%23day3/hand_write_dff_const1.jpeg">

*State Optimisation*: This refers to optimization of unused states. This develops best possible optimized state machine.

*Cloning*:This optimization method involves replicating a cell to alleviate the burden on a heavily utilized cell. This approach is commonly favored during the execution of a PHYSICAL AWARE SYNTHESIS. Let's take into account a flip-flop denoted as A, which establishes connections with both flip-flops B and C through a combination of logic operations. In cases where B and C are positioned a considerable distance away from A in the floorplan, there arises a delay in the routing path. To mitigate this issue, we duplicate A and connect it to two intermediary flip-flops. Subsequently, the outputs from these intermediary flip-flops are directed towards B and C, effectively reducing the delay. This procedure is referred to as "cloning," as it involves generating two novel flip-flops that replicate the functionality of A.

*Retiming* : Retime optimization is a strategy employed to enhance sequential circuits. Its impact is limited to the arrangement of registers within the circuit, leaving the combinational segment untouched. This robust technique for sequential optimization facilitates the shifting of registers throughout the combinational logic or the enhancement of register count, thereby enhancing performance by striking a balance between power consumption and delay. Importantly, these improvements are achieved without altering the overall input-output behavior of the circuit.

**Example 1** Here D flip flop is the result in synthesized circuit
```ruby
module dff_const1(input clk, input reset, output reg q);
	always @(posedge clk, posedge reset)
	begin
		if(reset)
			q <= 1'b0;
		else
			q <= 1'b1;
	end
endmodule
```
Simulation
<img width="1085" alt="wave_dff_const1" src="https://github.com/Sidv005/Samsung-PD-Training/blob/8a0fc3e0728ce7bb23438d3d1a5703ca9b4ce921/SamsungPD/%23day3/wave_dff_const1.png">

Synthesized circuit is shown below 
<img width="1085" alt="dff_const1_circuit" src="https://github.com/Sidv005/Samsung-PD-Training/blob/8a0fc3e0728ce7bb23438d3d1a5703ca9b4ce921/SamsungPD/%23day3/dff_const1_circuit.png">

**Example 2** Here D flip flop is not yielded in synthesized circuit
```ruby
module dff_const2(input clk, input reset, output reg q);
	always @(posedge clk, posedge reset)
	begin
		if(reset)
			q <= 1'b1;
		else
			q <= 1'b1;
	end
endmodule
```
Simulation
<img width="1085" alt="wave_dff_const2" src="https://github.com/Sidv005/Samsung-PD-Training/blob/8a0fc3e0728ce7bb23438d3d1a5703ca9b4ce921/SamsungPD/%23day3/wave_dff_const2.png">

Synthesized circuit is shown below 
<img width="1085" alt="dff_const2_circuit" src="https://github.com/Sidv005/Samsung-PD-Training/blob/8a0fc3e0728ce7bb23438d3d1a5703ca9b4ce921/SamsungPD/%23day3/dff_const2_circuit.png">

**Example 3**
```ruby
module dff_const3(input clk, input reset, output reg q);
	reg q1;

	always @(posedge clk, posedge reset)
	begin
		if(reset)
		begin
			q <= 1'b1;
			q1 <= 1'b0;
		end
		else
		begin
			q1 <= 1'b1;
			q <= q1;
		end
	end
	endmodule
```
Simulation
<img width="1085" alt="waveform_dff_const3" src="https://github.com/Sidv005/Samsung-PD-Training/blob/8a0fc3e0728ce7bb23438d3d1a5703ca9b4ce921/SamsungPD/%23day3/waveform_dff_const3.png">

Synthesized circuit is shown below 
<img width="1085" alt="dff_const3_circuit" src="https://github.com/Sidv005/Samsung-PD-Training/blob/8a0fc3e0728ce7bb23438d3d1a5703ca9b4ce921/SamsungPD/%23day3/dff_const3_circuit.png">

Example 4
```ruby
module dff_const4(input clk, input reset, output reg q);
	reg q1;

	always @(posedge clk, posedge reset)
	begin
		if(reset)
		begin
			q <= 1'b1;
			q1 <= 1'b1;
		end
	else
		begin
			q1 <= 1'b1;
			q <= q1;
		end
	end
	endmodule
```
Simulation
<img width="1085" alt="waveform_dff_const4" src="https://github.com/Sidv005/Samsung-PD-Training/blob/8a0fc3e0728ce7bb23438d3d1a5703ca9b4ce921/SamsungPD/%23day3/waveform_dff_const4.png">

Synthesized circuit is shown below 
<img width="1085" alt="dff_const4_circuit" src="https://github.com/Sidv005/Samsung-PD-Training/blob/8a0fc3e0728ce7bb23438d3d1a5703ca9b4ce921/SamsungPD/%23day3/dff_const4_circuit.png">

Example 5
```ruby
module dff_const5(input clk, input reset, output reg q);
	reg q1;
	always @(posedge clk, posedge reset)
		begin
			if(reset)
			begin
				q <= 1'b0;
				q1 <= 1'b0;
			end
		else
			begin
				q1 <= 1'b1;
				q <= q1;
			end
		end
	endmodule
```
Simulation
<img width="1085" alt="waveform_dff_const5" src="https://github.com/Sidv005/Samsung-PD-Training/blob/8a0fc3e0728ce7bb23438d3d1a5703ca9b4ce921/SamsungPD/%23day3/waveform_dff_const5.png">

Synthesized circuit is shown below 
<img width="1085" alt="dff_const5_circuit" src="hhttps://github.com/Sidv005/Samsung-PD-Training/blob/8a0fc3e0728ce7bb23438d3d1a5703ca9b4ce921/SamsungPD/%23day3/dff_const5_circuit.png">
</details>

<details>
<summary>Sequential optimization of unused outputs </summary>

**Example 1**
```ruby
module counter_opt (input clk , input reset , output q);
   reg [2:0] count;
   assign q = count[0];
   always @(posedge clk ,posedge reset)
   begin
   	if(reset)
   		count <= 3'b000;
   	else
   		count <= count + 1;
   end
   endmodule
```
During synthesis by yosys printing statistics need to be observed which is displayed in below image.
<img width="1085" alt="counter_opt_printing_stat" src="https://github.com/Sidv005/Samsung-PD-Training/blob/8a0fc3e0728ce7bb23438d3d1a5703ca9b4ce921/SamsungPD/%23day3/counter_opt_printing_stat.png">
From this we can notice that only one D Flip Flop is implemented in 3 bit counter instead of 3 Flip Flops. since 2 bits are unused.

Synthesized circuit is shown below.
<img width="1085" alt="counter_opt_circuit" src="https://github.com/Sidv005/Samsung-PD-Training/blob/8a0fc3e0728ce7bb23438d3d1a5703ca9b4ce921/SamsungPD/%23day3/counter_opt_circuit.png">
This is a 3 bit counter with output only LSB.

**Updated Counter**
```ruby
module counter_opt (input clk , input reset , output q);
	reg [2:0] count;
	assign q = {count[2:0]==3'b100};
	always @(posedge clk ,posedge reset)
	begin
	if(reset)
		count <= 3'b000;
	else
		count <= count + 1;
	end
endmodule
```
Here all 3 bits are used so 3 Flops are preserved But in earlier case Oonly LSB was used hence 1 Flop was used. All other blocks are driving adder circuit.
Below image shows the printing statistics during synthesis.
<img width="1085" alt="counter_opt2_printing_stat" src="https://github.com/Sidv005/Samsung-PD-Training/blob/8a0fc3e0728ce7bb23438d3d1a5703ca9b4ce921/SamsungPD/%23day3/counter_opt2_printing_stat.png">

Synthesized circuit is as follows:
<img width="1085" alt="counter_opt2_circuit" src="https://github.com/Sidv005/Samsung-PD-Training/blob/8a0fc3e0728ce7bb23438d3d1a5703ca9b4ce921/SamsungPD/%23day3/counter_opt2_circuit.png">

</details>

## Day-4-Intoduction to GLS, Synthesis-Simulation mismatch and Blocking/Non Blocking Statements
<details>
 <summary>GLS, Synthesis Simulation Mismatch and Blocking vs Non Blocking statements in Verilog </summary>
GLS stands for gate level Synthesis. This is the process in which testbench runs with netlist as DUT. Gate-level synthesis is the process of converting a high-level digital circuit description written in a hardware description language (HDL) into a lower-level representation composed of logic gates and basic digital components. This transformation optimizes the design for factors like speed, area, and power consumption while maintaining the intended functionality. The process involves functional verification, optimization, timing analysis, and layout verification before the circuit is manufactured. It bridges the gap between the abstract design and the physical implementation on a chip.
	
**Why GLS ?**
GLS is used to verify logical correctness of design after synthesis. GLS also assist in ensuring timing of the design is met. For this GLS needs to be run with delay annotations. If Gate level models are delay annotated the GLS can be used for timing validation.

***Synthesis Simulation Mismatch***
Synthesis Simulation Mismatch (SSM) denotes inconsistencies between predicted circuit behavior during simulation and the realized behavior post gate-level synthesis. This divergence can arise from factors like abstraction level disparities, timing effects, optimization discrepancies, and variances in tool behavior. Rectifying SSM entails employing timing-aware simulations, gate-level simulations, static timing analysis, robust verification techniques, and design evaluations to ensure precise circuit performance after synthesis. SSM are caused dur to few factors which are as follows:
- Missing Sensitivity list
- Blocking and Non Blocking Assignments
- Non standard Verilog Code

*Missing Sensitivity List*: A missing sensitivity list refers to an incomplete or incorrect list of input signals in a procedural block within hardware description languages like Verilog or VHDL. This list specifies which signals trigger the execution of the block. Neglecting to include all relevant signals can lead to inaccurate or unintended circuit behavior during simulation and synthesis. Properly defining the sensitivity list is essential for ensuring accurate logic operations and handling asynchronous events correctly in digital circuit design. 
As we know Synthesizer only focuses on statements and assignments in procedural block and not on sensitivity list so it may lead to correct synesized circuit but while functional verification results would have difference between RTL simulation and synthesized netlsit simulation. 

To avoid missing sensitivity lists, designers need to ensure that all the signals that influence the behavior of the logic inside a procedural block are included in the sensitivity list. This helps maintain accurate and predictable circuit behavior during simulation and synthesis. Properly specifying the sensitivity list is important for capturing the intended logic operation, handling asynchronous events correctly, and preventing unexpected issues in the design.

*Blocking and Non Blocking Assignments*:-
Blocking statements: When a blocking statement is encountered in a procedural block, it is executed sequentially, and the next statement in the block will not begin execution until the current statement completes. This can lead to a specific and predictable order of operations, but it also means that the execution of subsequent statements is blocked until the current one finishes. They reflect a clear sequence of operations and are commonly used to model synchronous circuit behavior where order matters.

**Example-1**:-
```ruby
always @(posedge clk) begin
    a = b + c;  // Blocking assignment
    d = a - e;  // Subsequent statement blocked until assignment to 'a' completes
end
```
Non Blocking statements: This executes all RHS when always block is entered and assigns to LHS. Here parallel evaluation is done. When a non-blocking statement is encountered in a procedural block, it is scheduled for execution but does not take immediate effect. Instead, the assignment occurs at the end of the current time step, ensuring that all statements within the block are evaluated independently of the order in which they appear in the code. 

**Example-2**:-
```ruby
always @(posedge clk) begin
    a <= b + c;  // Non-blocking assignment
    d <= a - e;  // No delay, assigned concurrently with previous statement
end
```
Non Blocking statements are best choice for always block execution.
 </details>

<details>
 <summary>LABS on GLS (Simulation Synthesis Mismatch)</summary>
	
**Example-1** RTL Code for ternary_operator.v file 
```ruby
module ternary_operator_mux (input i0 , input i1 , input sel , output y);
assign y = sel?i1:i0;
endmodule
```
Simulated wave form is as follows:
<img width="1085" alt="wave_ternary%20_operartor_mux" src="https://github.com/Sidv005/Samsung-PD-Training/blob/6e8630d4cf3f6450246aedea8d66b62c33953deb/SamsungPD%23day4/wave_ternary%20_operartor_mux.png">
synthesized circuit is shown below:
<img width="1085" alt="ternary_circuit" src="https://github.com/Sidv005/Samsung-PD-Training/blob/6e8630d4cf3f6450246aedea8d66b62c33953deb/SamsungPD%23day4/ternary_circuit.png">
Generated Netlist code is following.
<img width="1085" alt="ternary_netlist_code" src="https://github.com/Sidv005/Samsung-PD-Training/blob/6e8630d4cf3f6450246aedea8d66b62c33953deb/SamsungPD%23day4/ternary_netlist_code.png">
Netlist Simulation:
	<img width="1085" alt="ternary_netlist_gls" src="https://github.com/Sidv005/Samsung-PD-Training/blob/6e8630d4cf3f6450246aedea8d66b62c33953deb/SamsungPD%23day4/ternary_netlist_gls.png">
From the above two waveforms it is observed that when *sel* is 0 output follows i0 and when *sel* is 1 output follows i1. The RTL simulated waveform and Netlist simulated waveform obtained is same. 
There is no synth-sim mismatch.

**Example 2** RTL Cede of bad_mux.v file. Here always block is activated only when *sel* line is changed.
```ruby
module bad_mux (input i0 , input i1 , input sel , output reg y);
always @ (sel)
begin
	if(sel)
		y <= i1;
	else 
		y <= i0;
end
endmodule
```
RTL Simulated waveform is shown below:
<img width="1085" alt="wave_bad_mux" src="https://github.com/Sidv005/Samsung-PD-Training/blob/6e8630d4cf3f6450246aedea8d66b62c33953deb/SamsungPD%23day4/wave_bad_mux.png">

Synthesized circuit
<img width="1085" alt="bad_mux%20_circuit" src="https://github.com/Sidv005/Samsung-PD-Training/blob/6e8630d4cf3f6450246aedea8d66b62c33953deb/SamsungPD%23day4/bad_mux%20_circuit.png">

Generated Netlist code is as follows:

```ruby
/* Generated by Yosys 0.9+4081 (git sha1 862e84eb, gcc 7.5.0-3ubuntu1~18.04 -fPIC -Os) */

module bad_mux(i0, i1, sel, y);
  wire _0_;
  wire _1_;
  wire _2_;
  wire _3_;
  input i0;
  input i1;
  input sel;
  output y;
  sky130_fd_sc_hd__mux2_1 _4_ (
    .A0(_0_),
    .A1(_1_),
    .S(_2_),
    .X(_3_)
  );
  assign _0_ = i0;
  assign _1_ = i1;
  assign _2_ = sel;
  assign y = _3_;
endmodule
```
Netlist simulated waveform :
<img width="1085" alt="wave_bad_mux_gls" src="https://github.com/Sidv005/Samsung-PD-Training/blob/6e8630d4cf3f6450246aedea8d66b62c33953deb/SamsungPD%23day4/wave_bad_mux_gls.png">
The RTL simulated waveform and synthesized netlist simulated waveform are compleletly different. In netlist simulated waveform y follows *i0* and *i1* completely throughout when *sel* is 0 and 1 respectively. In RTL simulation output changes only when *sel* is altering which is incorrect behavior of mux. This is example of synth - sim mismatch due to *Missing Sensitivity List*.
</details>

<details>
 <summary>LABS on Simulation Synthesis Mismatch (Blocking statement)</summary>

**Example-1** RTL code of blocking_caveat.v file
In this design output *d* depends on past avlues of x which means past values of *a* and *b*. This apparently behaves like imaginary flop.
```ruby
module blocking_caveat (input a , input b , input  c, output reg d); 
reg x;
always @ (*)
begin
	d = x & c;
	x = a | b;
end
endmodule
```
Simulation waveform of RTL:-
<img width="1085" alt="wave_blocking_caveat" src="https://github.com/Sidv005/Samsung-PD-Training/blob/42b6ce6beab111a67f38498028f57a28c9323852/SamsungPD%23day4/wave_blocking_caveat.png">
From this image observe thutput is acting like a imaginary flop since it is beholding previous values of *a* and *b*.

Now yosys is invoked for synthesis. The synthesized circuit is shown below.
<img width="1085" alt="blocking_caviat_circuit" src="https://github.com/Sidv005/Samsung-PD-Training/blob/42b6ce6beab111a67f38498028f57a28c9323852/SamsungPD%23day4/blocking_caviat_circuit.png">

The generated netlist code is illustrated below.
<img width="1085" alt="blocking_caveat_netlist_code" src="https://github.com/Sidv005/Samsung-PD-Training/blob/42b6ce6beab111a67f38498028f57a28c9323852/SamsungPD%23day4/blocking_caveat_netlist_code.png">

Simulated waveform for synthesized netlist is in following figure.
<img width="1085" alt="wave_blockin_caveat_GLS" src="https://github.com/Sidv005/Samsung-PD-Training/blob/42b6ce6beab111a67f38498028f57a28c9323852/SamsungPD%23day4/wave_blockin_caveat_GLS.png">

The above .v file describes a combinational circuit having *or and gate*, where output (x) of or is internally connected to and gate giving final output as *d*. In RTL code *or and* operations are operating in reverse order due to bolocking assignments. Hence AND gate is taking input from previous output of OR gate which acts like imaginary flop this leads to wrong output *d* waveform. The netlist simulated waveform shows correct functionality of combinational circuit this can be observed from above figure. This is example of synth-sim mismatch due to *Blocking statements*. This issue can be tackeled by using Non Blocking statements.

</details>

## Day-5-Intoduction to Design for Testability
<details>
<summary>Fundamentals of DFT</summary>
	
***Testability***- This term refers to the degree of easiness towards checking a chip for detecting faults and errors. It is executed during synthesis of RTL Design in ASIC design flow. Testability features involves scan chains, BIST, etc. which improves reliability of the integrated circuits.

***DFT***- Design for Testability is a technique which provides a design to become testable after production. It is the extra logic which need to be inserted during design process which is helpful in post-production testing.

**Why need DFT ?** - There are defects in silicon which leads to errors in the device. The manufacturing process is not 100% error free. For manufacturing millions of chip running full exhaustive tests on the device is not feasible so a design is necessary required to detect the defects and faults which results to correct manufacturing. Thus, DFT technique is used to implement such a design which detects the faults in the physical device.

- DFT assures the detection of all faults in circuit.
  
- DFT reduces cost and time associated with test development.
  
- DFT reduces the execution time of performing test on fabrication chips.

**Levels of testing** : The 3 main levels of testing are are follows:

- a.Chip-level :- stage at which chips are manufactured. Example:*Built-in self-test(BIST)*

- b.Board-level :- stage at which chips are integrated on boards.

- c.System-level:- stage at which various boards are gathered together. Example:*Boundary scan*

**Benefits** of DFT are as follows:

- a. DFT methods contributes to the overall test coverage of circuit.

- b. Assists in localizing faults and makes debugging and fault isolation easier.

- c. Reduces test time by allowing concurrent testing of multiple parts of ICs.

- d. DFT simplifies the testing process and is cost effectiveduring manufacturing.

**Tradeoffs** of DFT are listed below:

- a. Increases design compexity so design time also increases.

- b. Potentially affects performance.

- c. Due to extra circuitry more chip area is consumed.

- d. Additional costs because of extra testing circuitry.

**Basic teminologies**
DFT increases the accessibility of internal nodes 

- **Controllability**: this term refers to tendency to establish specific signal value in any net.i.e ability to drive the node to "1" or"0".

- **Observability**: This term refers to ability to determine internal values by controlling stimulus inputs and observing outputs.i.e. ability to observe the effect of controlling.
The value at the nodes is shifted out through scan patterns and is observed in scan out ports.

**Fault**: It is a defect which might results to system malfunction and errors.

**Error**: Error is consequence of faults which leads to unstable state.

**Failure**: System is said to be failure if it does not perform expected functions.

**Fault coverage**: It can be defined as a percentage ratio representing total no. of faults detected over total no. of possible faults.

**Defect level**: It is the fraction of faulty parts that are shipped to customers
</details>

## Day6 - Introduction To Logic Synthesis 
<details>
<summary>Fundamentals of Digital Logic Design and Synthesis</summary>
Digital Logic, as a switching mechanism, possesses significant capabilities in the realms of automation and decision-making. Many automation tasks heavily rely on decision-making circuits, and these functionalities are typically described using behavioral design specifications written in Hardware Description Languages (HDLs). Notable examples of HDLs include VHDL and Verilog.

- The RTL is the behavioral code. We require the actual gates i.e., gates, flops etc.
- The RTL code is converted into gate level netlist by Synthesis. The synthesis tool takes .lib, verilog file and sdc file (constraint file) as input and generates netlist as output.
- A ".lib" file comprises a variety of logical modules such as AND, OR, NOT, NAND, each with distinct performance characteristics, including Fast, Typical, and Slow variations. Faster cells are essential to satisfy setup time constraints and enhance overall performance, while slower cells are necessary to fulfill hold time requirements.
- The synthesizer is directed to choose the most suitable cell variations for constructing a logic circuit, and this guidance is commonly known as constraints.

**LOGIC SYNTHESIS:**
Logic synthesis aims to create a functional digital circuit that is both logically and electrically accurate while adhering to specified timing requirements. To illustrate this concept, let's delve into an example. Here output *y* is assigned as *ab+bc+ac* the output can be achieved using 3 implementations. Refering to below figure the table shows that implemetation 3 is best option for designing logic circuit. Meanwhile consider a situation where this circuit is present in hold sensitive path then we need to add buffers to increase combinational delay and this may lead to kore area consumption. So synthesizer needs to be guided by *sdc* file as per requirements. 
<img width="1085" alt="illustration" src="https://github.com/Sidv005/Samsung-PD-Training/blob/4e5ba100ac404f70ff959d99e8266aa741ca3b14/SamsungPD%23day6/illustration.PNG">

- Constraints serve as directives for the synthesizer, instructing it to select the most suitable library cells that are ideal for achieving an optimal design.
</details>

<details>
<summary>Introduction to DC Shell</summary>
The Design Compiler, developed by Synopsys, is a synthesis tool designed specifically for the ASIC (Application-Specific Integrated Circuit) design flow. The features are as follows:
	
- Has the ability to perform DFT Scan stitch
- Can handle huge designs with extreme complexity and provide very good QoR.
- Compatibility with different tools made by Synopsys.
- Recognized as a top-quality synthesis tool widely used in the semiconductor industry.
  
***Common Terminology associated with DC:***
*Synopsys Design Constraints(SDC)* : These design constraints are given to DC (Design Compiler) to facilitate the necessary optimizations for achieving the best possible implementation.

- *.lib* : A design library housing standard cells.
- *.db* : Similar to .lib, but in an alternate format that DC (Design Compiler) can comprehend, libraries are provided in .db format.
- *.ddc* : Synopsys uses its own exclusive format called DDC for storing design data, and DC (Design Compiler) has the ability to both produce and interpret this format.
- *Design* : RTL files which has the behavioral model of the design.

**SDC : Synopsys Design Constraints**
The SDC format defines design intentions regarding timing, power, and area constraints, with power described using UPF. SDC commands can extract UPF information. This format is compatible with various EDA tools in the semiconductor industry and is built upon the Tool Command Language (Tcl).

**DC Setup:**
The DC setup process involves taking RTL files, .lib files (similar to Yosys), and SDC files as inputs to produce gate-level netlists, DDC format files, and synthesis reports as outputs.
The ASIC flow is the steps involved in converting RTL to the Graphical Data set(GDS). The Application Specific IC flow is shown in figure below: <br>
<img width="600" alt="ASICflow" src="https://github.com/Sidv005/Samsung-PD-Training/blob/23a9599941c49214a1e3a55031833afe2746c3db/SamsungPD%23day6/ASICflow.jpeg"> <br>
- The DC Synthesis process can be described in the following manner: In this scenario, the "Design.lib" is a specific design library, distinct from the standard .lib or technology library, and it may represent third-party intellectual property (IP) or pre-designed modules. The Design Compiler ensures that the connections of inputs and outputs from this module are correctly integrated into the overall design and optimizes the logic accordingly.

- The Design Compiler reads the Verilog files of the design, along with the standard library files and constraints, and generates reports as it links and synthesizes the design. Eventually, it produces a netlist as its final output. The DC Synthesis flow is given below in the figure.<br>
<img width="600" alt="dc_synth" src="https://github.com/Sidv005/Samsung-PD-Training/blob/7662963a9a31c04b318faed24f35b77eb406fb9e/SamsungPD%23day6/dc_synth.png"><br>

**Invoking dc basic setup**
- We understand that the library name contains crucial information regarding the PVT (Process, Voltage, Temperature) conditions under which a design operates. The performance of any electronic circuit is influenced by factors like voltage, temperature, and manufacturing process. Therefore, a unique .lib file is defined for each PVT corner, with this particular PVT corner representing typical conditions at 25°C temperature and 1.8V voltage.

- Within the .lib file, you can find valuable data such as the units for resistance (R), inductance (L), capacitance (C), time measurements, technology specifications, and the various versions or flavors of each cell.

- To initiate the DC (Design Compiler) shell, the following commands are executed:

```ruby
$ csh
$ dc_shell
dc_shell> 
```
To initiate the process, we must activate the C shell and subsequently launch the DC shell. Within the DC shell, a series of license checks are performed for various compilers, including the VHDL compiler, HDL compiler (used for interpreting Verilog or other Hardware Description Languages), DFT compiler (for enabling scan stitching), Design Vision (the graphical version of DC), and Power Compiler (essential for power-aware synthesis). Below image shows the dc_shell activatation.<br>
<img width="800" alt="dc_shell_invoke" src="https://github.com/Sidv005/Samsung-PD-Training/blob/4ca2a060e41021014edb7705e94c38d2a137ff95/SamsungPD%23day6/dc_shell_labs/dc_shell_invoke.png"><br>

```ruby
dc_shell> echo $target_library
 your_library.db
dc_shell> echo $link_library
 * your_library.db
```
In DC, the technology file is in the form of target library or link library. These both libraries are used by DC shell to pick standard cells. your_library.db is an imaginary non-existent library, just pointed for dummy purpose.

```ruby
dc_shell> read_verilog DC_WORKSHOP/verilog_files/lab1_flop_with_en.v
dc_shell> write -f verilog -out lab1_net.v
dc_shell> sh gvim lab1_net.v &
```
We provide the input Verilog file (which contains the RTL code) to be read and written in the same format as understood by the design. To access the file editor within the shell, we need to utilize the specified command "sh gvim." The behavioral code of the design that is being read is:

```ruby
module lab1_flop_with_en ( input res , input clk , input d , input en , output reg q);
always @ (posedge clk , posedge res)
begin
	if(res)
		q <= 1'b0;
	else if(en)
		q <= d;	
end
endmodule
```
The dc shell reads lib files in .db format.

```ruby
dc_shell> read_db ~/DC_WORKSHOP/lib/sky130_fd_sc_hd_tt_025c_1v80.db
dc_shell> sh gvim lab1_net.v &
```
The resulting netlist appears as follows: <br>
<img width="600" alt="SEQGEN" src="https://github.com/Sidv005/Samsung-PD-Training/blob/4ca2a060e41021014edb7705e94c38d2a137ff95/SamsungPD%23day6/dc_shell_labs/SEQGEN.png"><br>

The cells are within SEQGEN, but they are not in the sky130 cell format. This situation arises because no file has been designated for the target and link library. "gtech" serves as the virtual library within DC's memory, used to interpret the design. A dummy library file is indicated when set library is not assigned. Below image shows the same. <br>
<img width="600" alt="your_lib" src="https://github.com/Sidv005/Samsung-PD-Training/blob/4ca2a060e41021014edb7705e94c38d2a137ff95/SamsungPD%23day6/dc_shell_labs/your_lib.png"><br>
Upon assigning files to the libraries, the design is linked and compiled in the following manner.
```ruby
dc_shell> set target_library /home/usha.m/DC_WORKSHOP/lib/sky130_fd_sc_hd_tt_025c_1v80.db
dc_shell> set link_library {* <path to standardcell library> }
dc_shell> link
dc_shell> compile
dc_shell> write -f verilog -out lab1_net_with_sky130.v
```
Now the library is assigned which is shown in following figure. <br>
<img width="500" alt="synopsys_dc_setup" src="https://github.com/Sidv005/Samsung-PD-Training/blob/4ca2a060e41021014edb7705e94c38d2a137ff95/SamsungPD%23day6/dc_shell_labs/synopsys_dc_setup.png"><br>

 In this process, the link_library is specified to append data to the existing list without replacing it. Consequently, the resulting outnetlist is as follows:<br>
<img width="600" alt="sky130" src="https://github.com/Sidv005/Samsung-PD-Training/blob/678497056bdef97e7199d0db48ade549231d629a/SamsungPD%23day6/dc_shell_labs/sky130.png"><br>

 Below image shows the comparison between the two netlist obtained.<br>
 <img width="600" alt="comparison(SEQ_sky)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/c1daf0e62aa3c9adafef173f74452d66d2b8808b/SamsungPD%23day6/dc_shell_labs/comparison(SEQ_sky).png"><br>

## Lab on ddc gui with design_vision##
For launching the design vision tool, we need to load cshell and design_vision command. GUI version of design vision is evoked. The command to write out a ddc file as output of dc_shell after writing out netlist is:
```ruby
dc_shell> write -f ddc -out lab1_flop.ddc
```
The major benefit of ddc is that all the information loaded in one tool can be saved and used in another tool with one command. Following command is used inside the GUI. 
```ruby
design_vision> read_ddc lab1.ddc
```
The resulted netlist is shown in below image.<br>
<img width="1085" alt="ddc_netlist" src="https://github.com/Sidv005/Samsung-PD-Training/blob/4ca2a060e41021014edb7705e94c38d2a137ff95/SamsungPD%23day6/dc_shell_labs/ddc_netlist.png"><br>

## Lab on .synopsys dc setup ##
Everytime setting link and target library is cumbersum and error prone. Hence, following commands are used in terminal to setup library.
```ruby
gvim .synopsys_dc.setup
```
Below screenshot show the expected result in the terminal.<br>
<img width="600" alt="synopsys_dc_setup" src="https://github.com/Sidv005/Samsung-PD-Training/blob/4ca2a060e41021014edb7705e94c38d2a137ff95/SamsungPD%23day6/dc_shell_labs/synopsys_dc_setup.png"><br>
</details>

<details>
<summary>Labs on Tcl Scripting</summary>
	
The Tool Command Language (Tcl) is employed for crafting SDCs.
	
**Set**
- It is utilized for generating and assigning variables.
- For example, set x 10 => x=10
- set a [expr $x+$y] => x=x+y
- Square brackets serve the purpose of encapsulating commands within TCL for nesting.

**if-else**
```ruby
if {condition} {
statements if true
} else {
statements if false
}
```
In TCL, conditions should consistently be enclosed within curly braces. The dollar sign ($) is employed when referencing the value of a variable, not when initially assigning it using the "set" command.
An example is given below:

```ruby
if {$a < 10} {
echo "$a is less than 10"
}else {
echo "$a is greater than 10"
}
```

**while**
```ruby
 while {condition} {
 statements
 }
```
The "incr" command in TCL performs the same function as setting a variable using the expression "i [expr $i+1]" or "i=i+1."
An example is given below:
```ruby
set i 0
while {$i < 10} {
  echo $i;
 incr i;
}
```

**for**
```ruby
for {looping var} {condition} {looping var modification} {
statements
}
```
An example is given below:
  for {set i 0} {$i < 10} {incr i} {
  echo $i;
  }

Below image show the loop commands like for and while.<br>
<img width="400" alt="for_while" src="https://github.com/Sidv005/Samsung-PD-Training/blob/678497056bdef97e7199d0db48ade549231d629a/SamsungPD%23day6/dc_shell_labs/for_while.png"><br>

**foreach**
```ruby
 foreach var list {
 statements
}
```

```ruby
set my_design_list [list u_top/u_mod1 \
			 u_top/u_mod3 ]
foreach my_module $my_design_list {
set_size_only $my_module;
  }
```
- In this example, "my_design_list" serves as the identifier for the list. Lists in TCL can be likened to arrays in C.
- \ is used as line breaker. 
- set_size_only is a DC specific command.
Below image show the instruction set and obtained result in the terminal.<br>
<img width="600" alt="foreach" src="https://github.com/Sidv005/Samsung-PD-Training/blob/678497056bdef97e7199d0db48ade549231d629a/SamsungPD%23day6/dc_shell_labs/foreach.png"><br>

**foreach_in_collection**
The command "foreach_in_collection" is specific to DC (Design Compiler).
```ruby
foreach_in_collection var collection {
   statements
 }
```
The following figure shows the instruction set for *foreach_in_collection*.<br>
<img width="600" alt="foreach_in_collection" src="https://github.com/Sidv005/Samsung-PD-Training/blob/678497056bdef97e7199d0db48ade549231d629a/SamsungPD%23day6/dc_shell_labs/foreach_in_collection.png"><br>

*dc_shell> sh gvim &* 

The above command is utilized to open gvim window

The following command is used in the gvim window to create a tcl file.
```ruby
source myscript.tcl
```
where *myscript.tcl* is the name of the tcl file.
The following screenshot shows the myscript.tcl that is being used.<br>
<img width="600" alt="foreach_in_collection_tcl" src="https://github.com/Sidv005/Samsung-PD-Training/blob/678497056bdef97e7199d0db48ade549231d629a/SamsungPD%23day6/dc_shell_labs/foreach_in_collection_tcl.png"><br>

The result obtained is printed in the terminal which is shown below.<br>
<img width="600" alt="foreach_in_collection_multipy" src="https://github.com/Sidv005/Samsung-PD-Training/blob/52cdbfaad0368eb4c82aa6bfaeaa27567d3394f0/SamsungPD%23day6/dc_shell_labs/foreach_in_collection_multipy.png"><br>
</details>

## Day-7- Fundamentals of STA

<details>
 <summary>Introduction to STA(Static Timing Analysis) </summary>

***Static Timing Analysis (STA)*** plays a vital role in the validation and assurance of digital integrated circuit designs, verifying that they adhere to timing criteria and function dependably.

STA evaluates the timing behavior of digital circuits without the necessity for real-time simulation. It confirms that signals traverse the circuit while adhering to predetermined timing constraints, thereby ensuring correct operation and the attainment of performance objectives.

***Delay***
Delay is the duration required for a signal to travel from one location within a digital circuit to another. This metric holds immense significance in the design process, as it exerts a direct influence on the integrated circuit's performance, power efficiency, and overall reliability.

A *Maximum Delay* Constraint represents a design parameter or condition that sets an upper threshold on the time it requires for a signal to travel through a specific route or segment within an integrated circuit. As an illustration, think of a situation where two D flip-flops are linked with a combinational logic component in between them.

Tclk >= Tcq + Tcombi + Tsetup

The term *Minimum Delay constraint* denotes a design specification or stipulation that establishes a mandatory lower limit for the delay a signal must experience when traveling through a particular route or component within an integrated circuit. This constraint is implemented to guarantee that specific signals within the circuit do not propagate too swiftly, thereby preventing potential timing conflicts and operational complications.

Thold < Tcq + Tcombi

The concept of delay can be easily grasped by drawing an analogy with a water bucket. The aim is to fill both the buckets. One bucket is having higher inflow while the other one is having lesser inflow of water. So, the one having higher inflow will get fill first. This can be corelated with input transition i.e. we can infer that higher input transition less will be the dealy. 

Considering another example where one bucket is bigger than the other bucket and both have same inflow. In that case the smaller bucket will fill first. This can be corelated with load capacitance i.e lower the load capacitance lesser will be delay. We can conclude that Delay is the function of *input transition and load capacitance*.

***Timing Arc***
iming arcs are essential elements within VLSI (Very Large Scale Integration) design, playing a pivotal role in the process of timing analysis. These arcs outline how a particular logic element, such as a flip-flop or gate, interacts with input and output transitions, elucidating the resultant delay incurred during signal processing. They encapsulate the intricate dynamics of digital components, including considerations like rising and falling signal edges, setup and hold requirements, and the time it takes for signals to propagate through the element.

Combinational Cells Timing arcs : It gathers delay data for each input pin to every output pin that falls within its jurisdiction or control.

Below is the screenshot showing sucessful launch: <br>
<img width="600" alt="mux" src="https://github.com/Sidv005/Samsung-PD-Training/blob/d325849fd723c189376cb0bd1f6cc979bd667e89/day7/mux.png"> <br>
The timing arcs are as follows:

- I0 => Y
- I1 => Y
- S => Y

Y depends on all 3 inputs.

***Constraints***
In VLSI tools are used to synthesize a design so a VLSI designer can understand functionality under boundaries but for tool it is not possible. Hence constraints are required by the tool to synthesize the design. 

*The need of Constraints.*
In VLSI circuits if we consider a case where a launch FF is transporting data to capture FF through any combinational logic then some amount of delay will occur practicaly. Every FF will have their setup and hold timing constraint which are necessary otherwise the data will get corrupted or lost. Critical path is the path which decides the clock frequency. The VLSI circuits must not disobey setup and hold timing constraints. 

***Timing paths***
Timing paths in VLSI design refer to particular signal routes or pathways within a digital circuit, where the timing properties, such as signal propagation delays, setup times, hold times, and clock-to-q delays, are scrutinized to guarantee the circuit's accuracy and dependable functioning. These pathways are of utmost importance for timing analysis and serve as a cornerstone in attaining the desired performance and functionality of the integrated circuit. Typically, a timing path encompasses an initial point (usually a flip-flop or input pin), an array of logic gates and connections, and a concluding point (another flip-flop or output pin).

Start points of timing path

- Input ports
- Clock pins of regs

End point of timing path

- Output ports
- D pin of D flip flop / D Latch

A circuit is shown below. <br>
<img width="600" alt="timingpath" src="https://github.com/Sidv005/Samsung-PD-Training/blob/2b017f268dd36c88423a9575c40362eb362c5c1e/day7/timingpath.png"> <br>

- In this Reg 2 Reg is constrained by clock
- Reg to out is constrained by Output external delay , load and clock .
- In 2 Reg is constrained by input external delay ,clock, input transition.

Here we should consider the rising and falling time of the signal as constraint also then only this circuit is practically feasible.
</details>

<details>
 <summary>LABS </summary>

***Timing (.lib) file***
During the ASIC design flow, designers use this ".lib" file to select appropriate standard cells, estimate the circuit's timing and power characteristics, and perform optimizations to meet the project's requirements and constraints. It serves as a crucial resource for ensuring the successful implementation of the desired ASIC design.

As an illustration, our chosen standard library in this instance is "sky130_fd_sc_hd_tt_025C_1v8." This nomenclature indicates that we are employing a technology based on 130 nanometers, employing a typical manufacturing process, operating at a temperature of 25 degrees Celsius, and utilizing a voltage level of 1.8 volts. This also encompasses various variations or configurations of the same logic gates.

Within the ".lib" file, you'll also find details about each distinct version of gate cells, including information on their leakage power, physical area, and timing characteristics. Below screenshot shows the comparison between and2_0 and and2_2 interms of area and leakage power. <br>
<img width="900" alt="lib_and2gate" src="https://github.com/Sidv005/Samsung-PD-Training/blob/2b017f268dd36c88423a9575c40362eb362c5c1e/day7/lib_and2gate.png"> <br>


A *Look-Up Table (LUT)* in a Liberty file is a data structure that defines the logical functionality of a specific digital logic cell or gate in terms of its input combinations and corresponding output values.
It comprises of two indices where index 1 shows the input transition and  index2 shows output load capacitance. The matrix is selected using interpolation when any information is provided regarding  input transition and output load capacitance. Below image shows the index of and2_0 , and2_2. <br>
<img width="900" alt="lib_and_index" src="https://github.com/Sidv005/Samsung-PD-Training/blob/2b017f268dd36c88423a9575c40362eb362c5c1e/day7/lib_and_index.png"> <br>

*Unateness*
There are two major types of unateness: 

A positive unate function, concerning a specific input variable, behaves in a way that, regardless of how you set the other input variables, the function either stays the same or becomes larger as you change the designated input variable from 0 to 1. Essentially, this function relies solely on the presence of positive (1) values for that particular input variable

A negative unate function, concerning a specific input variable, exhibits a behavior where, regardless of the settings of the other input variables, the function either remains constant or decreases as the designated input variable changes from 0 to 1. In this scenario, the function relies solely on the presence of negative (0) values for that particular input variable. Below screenshot demonstrates the comparison of and2_0 and DFF in terms of timing_sense (unateness) and timing_type. <br>
<img width="900" alt="unateness" src="https://github.com/Sidv005/Samsung-PD-Training/blob/2b017f268dd36c88423a9575c40362eb362c5c1e/day7/unateness.png"> <br>

Below image shows the unateness of the D latch. <br>
<img width="900" alt="unatness_latch" src="https://github.com/Sidv005/Samsung-PD-Training/blob/2b017f268dd36c88423a9575c40362eb362c5c1e/day7/unatness_latch.png"> <br>

Below screenshot shows the comparison between Negedge D FF and Negedge D Latch. <br>
<img width="1000" alt="setup_timing_ff_latch" src="https://github.com/Sidv005/Samsung-PD-Training/blob/2b017f268dd36c88423a9575c40362eb362c5c1e/day7/setup_timing_ff_latch.png"> <br>

***lab on .lib in dc_shell***
1) to display all the sequential gates <br>
<img width="1080" alt="get_lib_cells" src="https://github.com/Sidv005/Samsung-PD-Training/blob/2b017f268dd36c88423a9575c40362eb362c5c1e/day7/get_lib_cells.png"> <br>

2) Display the library linked <br>
<img width="900" alt="list_lib" src="https://github.com/Sidv005/Samsung-PD-Training/blob/2b017f268dd36c88423a9575c40362eb362c5c1e/day7/list_lib.png"> <br>

3) Displays the cells list from the collection <br>
<img width="600" alt="forech_in_collection_get_lib_cells" src="https://github.com/Sidv005/Samsung-PD-Training/blob/2b017f268dd36c88423a9575c40362eb362c5c1e/day7/forech_in_collection_get_lib_cells.png"> <br>

4) Displays the pins of the gate cell and functionality of a particular gate <br>
<img width="900" alt="get_lib_pins" src="https://github.com/Sidv005/Samsung-PD-Training/blob/2b017f268dd36c88423a9575c40362eb362c5c1e/day7/get_lib_pins.png"> <br>

5) Displays the pins along with the direction of nand4bb_2 gate <br>
<img width="900" alt="get_lib_pin_dir" src="https://github.com/Sidv005/Samsung-PD-Training/blob/2b017f268dd36c88423a9575c40362eb362c5c1e/day7/get_lib_pin_dir.png"> <br>

6) Here's a Tcl program that takes a list of cells as input and prints the output pins along with their corresponding functionalities:

```ruby
set mylist [list sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__nand2_1 \
sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__nand2_2 \
sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__nand2_4 \
sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__nand2_8 \
sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__nand2b_1 \
sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__nand2b_2 \
sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__nand2b_4 \
sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__nand3_1 \
sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__nand3_2 \
sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__nand3_4 ];

foreach var $mylist {
  foreach_in_collection var_pins [get_lib_pins ${var}/* ] {
      set pin_name [get_object_name $var_pins];
      set pin_dir [get_lib_attribute $pin_name direction];
      if { $pin_dir == 2 } {


          set pin_func [get_lib_attribute $pin_name function];

          echo $pin_name $pin_dir $pin_func ;
       }
    }
} 
```
<img width="800" alt="critical_prog" src="https://github.com/Sidv005/Samsung-PD-Training/blob/2b017f268dd36c88423a9575c40362eb362c5c1e/day7/critical_prog.png"> <br>

7) Displays the functionality of nand4bb_2 <br>
<img width="600" alt="get_lib_pin_function" src="https://github.com/Sidv005/Samsung-PD-Training/blob/2b017f268dd36c88423a9575c40362eb362c5c1e/day7/get_lib_pin_function.png"><br>

8)  Displays the attributes of the cell/pin<br>
 <img width="1000" alt="attributes" src="https://github.com/Sidv005/Samsung-PD-Training/blob/2b017f268dd36c88423a9575c40362eb362c5c1e/day7/attributes.png"><br>

9)  Displays all the attributes in a list <br>
  <img width="600" alt="list_attributes" src="https://github.com/Sidv005/Samsung-PD-Training/blob/2b017f268dd36c88423a9575c40362eb362c5c1e/day7/list_attributes.png"> <br>
</details>

## Day-8-Advanced Constraints

<details>
 <summary>Clock Terminologies </summary>
We say that clock is constrained by originally its the clock period which gets constrained this leads limitation of combinational delay.

*Tclk >= Tcq + Tcomb + Tst*

*Tcomb <= Tclk - (Tcq + Tst)*

- A ***Clock Generator*** is an electronic oscillator that produces a clock signal for use in synchronizing a circuit's operation. The signal can range from a simple symmetrical square wave to more complex arrangements. The basic parts that all clock generators share are a resonant circuit and an amplifier. Different types are :-
  
1) Oscillators:-They generate continuous periodic signals without an external input. Common types include RC oscillators, LC oscillators, and crystal oscillators.
2) Phase-Locked Loops (PLLs): A phase-locked loop (also phase lock loop or PLL) is a system that generates an output signal whose phase is related to its input. The two signals will have the same frequency and either no phase difference or a constant phase difference between them.
3) Delay-Locked Loops (DLLs): A delay-locked loop (DLL) is a digital circuit that provides high-bandwidth data transmission rates between devices. DLL transmissions have no propagation delay, low clock skew between output clock signals and advanced clock domain control.
4) Ring Oscillators:A time-delay oscillator consists of an inverting amplifier with a delay element between the amplifier output and its input. The amplifier must have a gain greater than 1 at the intended oscillation frequency.
5) Crystal Oscillators: A crystal oscillator is an electric oscillator type circuit that uses a piezoelectric resonator, a crystal, as its frequency-determining element.

- ***Clock Distribution***
- When clock is generarted it needed to be distributed over the entire circuit. Clock trees are utilized in the network to achieve minmized skew and obtain optimized timing paths.

- *Clock skew* The difference in the arrival time of a clock signal at two different registers, which can be caused by path length differences between two clock paths, or by using gated or rippled clocks. Clock skew is the most common cause of internal hold violations.
<img width="600" alt="skew" src="https://github.com/Sidv005/Samsung-PD-Training/blob/0eb811e2240364b5da3bb20230a5bfb5916d2445/SamsungPD%23day8%23lab8/skew.png"><br>
In the above figure clock skew is represented.
  -  *Global Clock Skew*: The clock latency difference between two non related flops or the difference between the longest clock path and the shortest clock path in the design.
  -  *Local Clock Skew* :  The latency difference between two related flops in a design is called as local skew.
  -  *Positive skew* : The capture clock delay is greater than the launch clock latency. is advantageous for setup timing. Due to the inclusion of skew, the capture clock is delayed by a few ns. Therefore the 
     timing path requires one clock period and Skew margin to match the setup requirement.
  -  *Negative Skew*: If the destination register received the edge of the clock after the source register, the clock skew would be lagging. Negative Skew is beneficial for hold time since it delays the fresh 
     launch. Because of the delay in launching the new data, the prior data will be effectively recorded and will not be overwritten.

- *Clock jitter* : is a characteristic of the clock source and the clock signal environment. It can be defined as “deviation of a clock edge from its ideal location.” Clock jitter is typically caused by clock generator circuitry, noise, power supply variations, interference from nearby circuitry etc.

- *Clock latency* is defined as the amount of time taken by the clock signal in traveling from its source to the sinks. Clock latency comprises of two components - clock source latency and clock network latency.
  - Source latency is the time taken by the clock signal in traveling from clock source (may be PLL, oscillator or some other source) to the clock definition point.
  - Network latency is the time taken by the clock signal in traveling from clock definition point to the sinks of the clock.

***Clock Modelling*** - We need to model clock constrains as follows:
1. period
2. Source latency
3. Clock Network latency
4. Clock skew
5. Clock Network
</details>

<details>
 <summary>Constraining Design using DC_compiler </summary>
Now, we will discuss how constraints to be modeled. We are considering a verilog design file which is shown in below image.

```ruby
module lab8_circuit (input rst, input clk , input IN_A , input IN_B , output OUT_Y , output out_clk);
reg REGA , REGB , REGC ; 
always @ (posedge clk , posedge rst)
begin
	if(rst)
	begin
		REGA <= 1'b0;
		REGB <= 1'b0;
		REGC <= 1'b0;
	end
	else
	begin
		REGA <= IN_A | IN_B;
		REGB <= IN_A ^ IN_B;
		REGC <= !(REGA & REGB); 
	end
end
assign OUT_Y = ~REGC;
assign out_clk = clk;
endmodule
```
The circuit to be modeled is below:- <br>
<img width="800" alt="ckt" src="https://github.com/Sidv005/Samsung-PD-Training/blob/071d8ece53c37beb047910f894aa4a573e614377/SamsungPD%23day8%23lab8/ckt.jpeg"> <br>

Below screenshot is a display of linking and compiling via dc_shell.<br>
<img width="900" alt="link_compile" src="https://github.com/Sidv005/Samsung-PD-Training/blob/59c270a1ebf2d2a576c596367f3378daeb1dc07a/SamsungPD%23day8%23lab8/link_compile.png"> <br>

```ruby
get_ports
```
The above command is used to obtain collection of ports. Further scripting is done using foreach-in_collection to display all ports with its corresponding direction. The below image illustrates the same.<br>
<img width="900" alt="ports_dir" src="https://github.com/Sidv005/Samsung-PD-Training/blob/071d8ece53c37beb047910f894aa4a573e614377/SamsungPD%23day8%23lab8/ports_dir.png"> <br>

```ruby
get_cells *
```
The above command helps to display the collection of all cells available in design. Further cells are verifired wheather they are hierarchical or not. *is_hierarchical* is an attribute which is used appropritely and is demonstrated in the below image.<br>
<img width="900" alt="get_cells" src="https://github.com/Sidv005/Samsung-PD-Training/blob/071d8ece53c37beb047910f894aa4a573e614377/SamsungPD%23day8%23lab8/get_cells.png"> <br>

```ruby
get_attribute [get_cells <cell_name>] ref_name
```
The above command helps to print the reference name of the particular cell. Further scripting is done to the collection of cells with their associated reference name. This is illustrated in below image.<br>
<img width="900" alt="ref_name" src="https://github.com/Sidv005/Samsung-PD-Training/blob/071d8ece53c37beb047910f894aa4a573e614377/SamsungPD%23day8%23lab8/ref_name.png"> <br>

Now, after executing *write -f ddc -out lab_circuit.ddc* command in dc_shell *ddc file is read in the gui of design_vision*. The below image shows the schematic view of the circuit.<br>

<img width="900" alt="schematic_lab8" src="https://github.com/Sidv005/Samsung-PD-Training/blob/071d8ece53c37beb047910f894aa4a573e614377/SamsungPD%23day8%23lab8/schematic_lab8.png"> <br>
 Here the xor gate is replaced with and & nor gate by the tool during synthesis for optimization.

```ruby
get_nets *
all _connected <net name>
```
The above commands are used to obtain collection of nets. Same is illustrated in below image.<br>
<img width="600" alt="all_connected_nets" src="https://github.com/Sidv005/Samsung-PD-Training/blob/071d8ece53c37beb047910f894aa4a573e614377/SamsungPD%23day8%23lab8/all_connected_nets.png"> <br>

The below image shows how the scripting is done to display the driver cells and driven cells associated to a net.<br>
<img width="900" alt="ref_name" src="https://github.com/Sidv005/Samsung-PD-Training/blob/071d8ece53c37beb047910f894aa4a573e614377/SamsungPD%23day8%23lab8/net_driver%26driven_cell.png"> <br>

**Creating master Clock**

Here we will discuss how master clock is created in the network. The below screenshot shows how MYCLK (master clock) is created wherre the period is 10.<br>
<img width="600" alt="create_MYCLK" src="https://github.com/Sidv005/Samsung-PD-Training/blob/d214e4a767053dcbad92f3fda2fe3bc47f021f59/SamsungPD%23Day8%23lab10/create_MYCLK.png"> <br>

```ruby
report_clocks
```
The above command is used to give list of all clocks.
The below command is used to match the tow parameters and if yes then it returns 1 else 0.

```ruby
regexp [<parameter_1> <parameter_2>]
```
A tcl script is written and executed to display the pin name and clock name associated with it. The script is mentioned below.<br>
<img width="1090" alt="query_clock_pin_tcl" src="https://github.com/Sidv005/Samsung-PD-Training/blob/d214e4a767053dcbad92f3fda2fe3bc47f021f59/SamsungPD%23Day8%23lab10/query_clock_pin_tcl.png"> <br>

The obtained result is presented below.<br>
<img width="600" alt="clock_tcl_output" src="https://github.com/Sidv005/Samsung-PD-Training/blob/d214e4a767053dcbad92f3fda2fe3bc47f021f59/SamsungPD%23Day8%23lab10/clock_tcl_output.png"> <br>

Now an example of unvalid clock is discussed. Here a BADCLK is created on the nand gate output pin (U14 /Y). Below screenshot represents the same.<br>
<img width="600" alt="BADCLK" src="https://github.com/Sidv005/Samsung-PD-Training/blob/d214e4a767053dcbad92f3fda2fe3bc47f021f59/SamsungPD%23Day8%23lab10/BADCLK.png"> <br>

Below image shows how a 25% duty cycle clock can be created.<br>
<img width="600" alt="25%25_cycle_clock" src="https://github.com/Sidv005/Samsung-PD-Training/blob/d214e4a767053dcbad92f3fda2fe3bc47f021f59/SamsungPD%23Day8%23lab10/25%25_cycle_clock.png"> <br>

**Clock Network Modeling and Uncertainty**

The commands used to set the clock latency source end and clock network latency are as follows:

```ruby
set_clock_latency -source 1 [get_clocks MYCLK]
set_clock_latency 1 [get_clocks MYCLK]
```
The below image shows the setup of setup and hold delay. Later clock is removed to observe that path is unconstrained.<br>
<img width="600" alt="set_clock_latency" src="https://github.com/Sidv005/Samsung-PD-Training/blob/985826bcbf9eeb5a0f3c415d28cae6043de14973/SamsungPD%23day8%23lab11/set_clock_latency.png"> <br>

Now we will add the constraints once again by changing source latency to 2ns. We see that the clock delay is added to the clock period and clock_uncertainity gets subtracted in case of max. From the below image we can observe that slack has gone down.<br>
<img width="600" alt="slack_down" src="https://github.com/Sidv005/Samsung-PD-Training/blob/985826bcbf9eeb5a0f3c415d28cae6043de14973/SamsungPD%23day8%23lab11/slack_down.png"> <br>

In case of hold clock_uncertainity gets added to the clock delay.<br>
<img width="600" alt="slack_down_hold" src="https://github.com/Sidv005/Samsung-PD-Training/blob/985826bcbf9eeb5a0f3c415d28cae6043de14973/SamsungPD%23day8%23lab11/slack_down_hold.png"> <br>

**IO Delays**

Now Path is unconstrained for input and output external port. The below command is used to setup the input delay for max delay.
```ruby
set_input_delay -max 5 -clock [get_clocks MYCLK] [get_ports IN_A]
set_input_delay -max 5 -clock [get_clocks MYCLK] [get_ports IN_B]
```
The below image shows the report for the same.<br>
<img width="600" alt="set_input_delay" src="https://github.com/Sidv005/Samsung-PD-Training/blob/985826bcbf9eeb5a0f3c415d28cae6043de14973/SamsungPD%23day8%23lab12/set_input_delay.png"> <br>
<img width="600" alt="set_input_delay_report" src="https://github.com/Sidv005/Samsung-PD-Training/blob/985826bcbf9eeb5a0f3c415d28cae6043de14973/SamsungPD%23day8%23lab12/set_input_delay_report.png"> <br>

The below command is used to setup the input delay for min delay.
```ruby
set_input_delay -max 5 -clock [get_clocks MYCLK] [get_ports IN_A]
set_input_delay -max 5 -clock [get_clocks MYCLK] [get_ports IN_B]
```

The below image shows the report for the same.<br>
<img width="600" alt="set_input_min_rep" src="https://github.com/Sidv005/Samsung-PD-Training/blob/df06222e0016e18df64560f8483c86817b7f4b35/SamsungPD%23day8%23lab12/set_input_min_rep.png"> <br>

```ruby
set_input_transition -max 0.3 [get_ports IN_A]
set_input_transition -max 0.3 [get_ports IN_B]
set_input_transition -min 0.1 [get_ports IN_A]
set_input_transition -min 0.1 [get_ports IN_B]
```
Screenshot of input transition delay from port IN_A as as follows:<br>
<img width="600" alt="set_input_trans_report" src="https://github.com/Sidv005/Samsung-PD-Training/blob/df06222e0016e18df64560f8483c86817b7f4b35/SamsungPD%23day8%23lab12/set_input_trans_report.png"> <br>

Adding constraints to output

```ruby
set_output_delay -max 5 [get_clocks MYCLK] [get_ports OUT_Y]
set_output_delay -min 1 [get_clocks MYCLK][get_ports OUT_Y]
```
Screenshot of output_delay is given below:<br>
<img width="600" alt="set_output_delay_report" src="https://github.com/Sidv005/Samsung-PD-Training/blob/df06222e0016e18df64560f8483c86817b7f4b35/SamsungPD%23day8%23lab12/set_output_delay_report.png"> <br>

Now we need to add load  constraint
```ruby
set_load -max 0.4 [get_ports OUT_Y]
```
Below is the report for max path type where 0.4 ns is added as load cap.<br>
<img width="600" alt="set_load_report" src="https://github.com/Sidv005/Samsung-PD-Training/blob/df06222e0016e18df64560f8483c86817b7f4b35/SamsungPD%23day8%23lab12/set_load_report.png"> <br>

```ruby
set_load -min 0.1 [get_ports OUT_Y]
```

Below is the report for min path type where 0.1 ns is added as load cap.<br>
<img width="600" alt="set_load(min)_report1" src="https://github.com/Sidv005/Samsung-PD-Training/blob/df06222e0016e18df64560f8483c86817b7f4b35/SamsungPD%23day8%23lab12/set_load(min)_report1.png"> <br>

**Generated clock**

Generated clocks are always created w.r.t master clocks. The OUT_CLK needs to be constrained w.r.t OUT_CLK and the input clock. The below figure shows the commmands and result of new genrated clock.<br> 
<img width="600" alt="create_generated_clock" src="https://github.com/Sidv005/Samsung-PD-Training/blob/df06222e0016e18df64560f8483c86817b7f4b35/SamsungPD%23day8%23lab13/create_generated_clock.png"> <br>

Till now OUT_Y is constrained w.r.t MY_CLK which is a master clock as we can see in below figure.<br>
<img width="600" alt="OUT_Y%20wrt%20MYCLK" src="https://github.com/Sidv005/Samsung-PD-Training/blob/df06222e0016e18df64560f8483c86817b7f4b35/SamsungPD%23day8%23lab13/OUT_Y%20wrt%20MYCLK.png"> <br>

When we add constraints to the MYGEN_CLK we get timing with repect to MYGEN_CLK as we can see in below figure. <br>
<img width="600" alt="OUT_Y%20wrt%20MYGEN" src="https://github.com/Sidv005/Samsung-PD-Training/blob/df06222e0016e18df64560f8483c86817b7f4b35/SamsungPD%23day8%23lab13/OUT_Y%20wrt%20MYGEN.png"> <br>

The design used for this experiment is as follows:

```ruby
module lab8 circuit (input rst, input clk , input IN_A , input IN_B , output OUT_Y , output out_clk output reg out_div_clk)
reg REGA, REGB , REGC ;
always @ (posedge clk , posedge rst )
begin
	if(rst)
	begin
		REGA <= 1'b0 ;
		REGB <= 1'b0 ;
		REGC <= 1'b0 ;
		out_div_clk <= 1'b0 ;
	end
	else
	begin
		REGA= IN_A | IN_B;
		REGB<- IN_A ^ IN_B;
		REGC <= !(REGA & REGB) ;
		out_div_clk <= ~out_div_clk
	end
end
assign OUT_Y = ~REGC ;
assign out_clk = clk;
endmodule
```
Loading the modified design.<br>
<img width="1000" alt="read_verilog_modified" src="https://github.com/Sidv005/Samsung-PD-Training/blob/df06222e0016e18df64560f8483c86817b7f4b35/SamsungPD%23day8%23lab13/read_verilog_modified.png"> <br>

We can create a .tcl program and then source it to avoid writing command for constraints. Below image shows the tcl file.<br>
<img width="600" alt="lab8_cons_tcl" src="https://github.com/Sidv005/Samsung-PD-Training/blob/df06222e0016e18df64560f8483c86817b7f4b35/SamsungPD%23day8%23lab13/lab8_cons_tcl.png"> <br>

The report_timing after sourcing the tcl script is as follows:<br>
<img width="600" alt="lab8_cons_tcl_report_clock" src="https://github.com/Sidv005/Samsung-PD-Training/blob/df06222e0016e18df64560f8483c86817b7f4b35/SamsungPD%23day8%23lab13/lab8_cons_tcl_report_clocks.png"><br>

**Creating virtual clock for constraining a combinational circuit and using set_max_delay**

Now consider the case where two inputs In_C and In_D are given to combinational logic and it should be constraint , This design is independent of the original design.<br>
<img width="600" alt="comb_logic" src="https://github.com/Sidv005/Samsung-PD-Training/blob/198e1b0439381fe3af1d6316fdf2c57b3e22f5e2/SamsungPD%23day8%23lab15/comb_logic.jpeg"><br>

After loading new modified verilog file clock report is genrated which is present in the below image.<br>
<img width="600" alt="report_clocks_ports" src="https://github.com/Sidv005/Samsung-PD-Training/blob/df06222e0016e18df64560f8483c86817b7f4b35/SamsungPD%23day8%23lab15/report_clocks_ports.png"><br>

In the below figure observe that path is unconstrained.<br>
<img width="600" alt="report_path_unconstrained" src="https://github.com/Sidv005/Samsung-PD-Training/blob/198e1b0439381fe3af1d6316fdf2c57b3e22f5e2/SamsungPD%23day8%23lab15/report_path_unconstrained.png"><br>

Some new command are shown in the figure below with their results.<br>
<img width="600" alt="all_new_commands" src="https://github.com/Sidv005/Samsung-PD-Training/blob/198e1b0439381fe3af1d6316fdf2c57b3e22f5e2/SamsungPD%23day8%23lab15/all_new_commands.png"><br>

All fanout command is shown below with its results.<br>
<img width="600" alt="all_fanout" src="https://github.com/Sidv005/Samsung-PD-Training/blob/198e1b0439381fe3af1d6316fdf2c57b3e22f5e2/SamsungPD%23day8%23lab15/all_fanout.png"><br>

Script is written to display the collection of pins connected to IN_A along with their reference name.<br>
<img width="600" alt="foreach_in(all_fanout)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/198e1b0439381fe3af1d6316fdf2c57b3e22f5e2/SamsungPD%23day8%23lab15/foreach_in(all_fanout).png"><br>

All fanin command is shown below with its results.<br>
<img width="600" alt="all_fanin" src="https://github.com/Sidv005/Samsung-PD-Training/blob/198e1b0439381fe3af1d6316fdf2c57b3e22f5e2/SamsungPD%23day8%23lab15/all_fanin.png"><br>

We need to constrain path from IN_C & D to OUT_Z.
The command is :-
```ruby
set_max_latency -from [<source_port_name>] -to [<destination_port_name>]
```
Observe in below image that slack is viloated because earlier no path constraint was present. So tool has not optimized it.<br>
<img width="600" alt="constraint_slack(violated)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/198e1b0439381fe3af1d6316fdf2c57b3e22f5e2/SamsungPD%23day8%23lab15/constraint_slack(violated).png"><br>

Now write *compile_ultra* and observe thet slack is not viloated now since the tool has optimized it by using inv_4 and xnor2_1 for D to Z path.<br>
<img width="600" alt="slack(good)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/198e1b0439381fe3af1d6316fdf2c57b3e22f5e2/SamsungPD%23day8%23lab15/slack(good).png"><br>

The schematic of the design is represented in below figure.<br> 
<img width="1000" alt="schematic%20(out_Z)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/198e1b0439381fe3af1d6316fdf2c57b3e22f5e2/SamsungPD%23day8%23lab15/schematic%20(out_Z).png"><br>

**Virtual CLock**

Virtual CLock is a clock created without a definition point.
Creating virtual clock.<br>
<img width="600" alt="create_MYVCLK" src="https://github.com/Sidv005/Samsung-PD-Training/blob/198e1b0439381fe3af1d6316fdf2c57b3e22f5e2/SamsungPD%23day8%23lab15(P2)/create_MYVCLK.png"><br>

Observe in below figure that path is unconstrained.<br>
<img width="600" alt="path_unconstrain" src="https://github.com/Sidv005/Samsung-PD-Training/blob/198e1b0439381fe3af1d6316fdf2c57b3e22f5e2/SamsungPD%23day8%23lab15(P2)/path_unconstrain.png"><br>

Constraining the clock is done using below commands.

```ruby
set_input_delay -max 5 [get_ports IN_C] -clock [det_clocks MYVCLK]
set_input_delay -max 5 [get_ports IN_D] -clock [det_clocks MYVCLK]
set_output_delay -max 4.9 [get_ports OUT_Z] -clock [det_clocks MYVCLK]
```
When we execute report_timing -to OUT_Z -sig 4 , we get the slack violated.<br>
<img width="600" alt="slack(violate)_MYVCLK" src="https://github.com/Sidv005/Samsung-PD-Training/blob/198e1b0439381fe3af1d6316fdf2c57b3e22f5e2/SamsungPD%23day8%23lab15(P2)/slack(violate)_MYVCLK.png"><br>

WHen we execute *compile_ultra* the DC tool optimizes the design and slack is met as shown in figure below.<br>
<img width="600" alt="slack(good)_MYVCLK1" src="https://github.com/Sidv005/Samsung-PD-Training/blob/198e1b0439381fe3af1d6316fdf2c57b3e22f5e2/SamsungPD%23day8%23lab15(P2)/slack(good)_MYVCLK1.png"><br>
</details>

## Day9- Optimization ## 
<details>
 <summary> Overview of Combinational and Sequential Optimization</summary>
VLSI optimization plays a pivotal role in the development of efficient and high-performing integrated circuits (ICs). It encompasses the enhancement of multiple facets within IC design, including minimizing power consumption, optimizing area utilization, refining timing characteristics, and ensuring manufacturability.

- Cost function based Optimization
1. Optimization till cost is met
2. Over optimization of one goal can harm other goals.

- Goals for Synthesis

1. Meet Timing
2. Meet Area
3. Meet power

***Combinational logic Optimisation***:  employs various techniques and methodologies to create compact and power-efficient designs while meeting performance requirements in VLSI circuits.

1. constant propagation(Direct propagation)
2. Boolean Logic Optimization(K-Means ,QUine Mckluskey)
3. Squeezing Logic (Area and Power Saving)

Below circuit is an example of constant propogation.<br>
<img width="800" alt="CP" src="https://github.com/Sidv005/Samsung-PD-Training/blob/a8bb097839cae43fd5ace85a8c8e2fc3a745cbaa/%23day9/lab16(p1)/CP.jpeg"><br>

Below circuit is an example of Boolean Logic optimization.
<img width="800" alt="boole" src="https://github.com/Sidv005/Samsung-PD-Training/blob/a8bb097839cae43fd5ace85a8c8e2fc3a745cbaa/%23day9/lab16(p1)/boole.jpeg"><br>

**Resource Sharing**
Resource sharing is a fundamental strategy within VLSI design, frequently used to enhance the efficient utilization of constrained resources while upholding or even enhancing the intended functionality.

Below image shows the optimization and explanation.
<img width="800" alt="RS" src="https://github.com/Sidv005/Samsung-PD-Training/blob/25946880d7c7c0021b444c51bb3ef79a9894ba3f/%23day9/lab16(p1)/RS.jpeg"><br>

**Logic Sharing**
Logic sharing in VLSI design involves the efficient reuse or sharing of logical components, such as gates or functional blocks, to diminish the overall complexity, area footprint, and power consumption of an integrated circuit (IC). This prevalent approach serves to optimize chip designs while preserving the essential functionality.
Below image shows the optimization and explanation.<br>
<img width="800" alt="LS" src="https://github.com/Sidv005/Samsung-PD-Training/blob/25946880d7c7c0021b444c51bb3ef79a9894ba3f/%23day9/lab16(p1)/LS.jpeg"><br>

***Sequential Optimization***
- Basic Sequential Optimization
1. Sequential Constant propagation
2. Retiming
3. Unused Flop Removal
4. Clock Gating

- Advanced
1. State Optimization
2. Sequential logic cloning

Below image shows the Sequential Constant propagation optimization and explanation.<br>
<img width="800" alt="seqCP" src="https://github.com/Sidv005/Samsung-PD-Training/blob/1120f5ccc4a2f0d02ddace7278fdf882911f995c/%23day9/lab16(p1)/seqCP.jpeg"><br>
</details>

<details>
 <summary> Labs on Sequential and Combinational Optimization</summary>

The RTL design file of the opt_check is as follows:

```ruby
module opt_check (input a , input b , input c , output y1, output y2);
wire a1;
assign y1 = a?b:0;
assign y2 = ~((a1 & b) | c);
assign a1 = 1'b0;
endmodule
```

Below screenshot represents the timing report to y1 and y2 output ports.<br>
<img width="400" alt="report_timings(y1%20y2)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/1120f5ccc4a2f0d02ddace7278fdf882911f995c/%23day9/lab16(p1)/report_timings(y1%20y2).png"><br>

The schematic is presented below.<br>
<img width="800" alt="schema_opt_check" src="https://github.com/Sidv005/Samsung-PD-Training/blob/1120f5ccc4a2f0d02ddace7278fdf882911f995c/%23day9/lab16(p1)/schema_opt_check.png"><br>

The RTL design file of the opt_check2 is as follows:

```ruby
module opt_check2 (input a , input b , output y);
assign y = a?1:b;
endmodule
```
The schematic is presented below.<br>
<img width="800" alt="schema_opt_check2" src="https://github.com/Sidv005/Samsung-PD-Training/blob/1120f5ccc4a2f0d02ddace7278fdf882911f995c/%23day9/lab16(p1)/schema_opt_check2.png"><br>

The RTL design file of the opt_check3 is as follows:

```ruby
module opt_check3 (input a , input b, input c , output y);
assign y = a?(c?b:0):0;
endmodule
```
The schematic is presented below.<br>
<img width="800" alt="schema_opt_check3" src="https://github.com/Sidv005/Samsung-PD-Training/blob/1120f5ccc4a2f0d02ddace7278fdf882911f995c/%23day9/lab16(p1)/schema_opt_check3.png"><br>

The RTL design file of the opt_check3 is as follows:

```ruby
module opt_check4 (input a , input b , input c , output y);
assign y = a?(b?(a & c ):c):(!c);
endmodule
```
The schematic is presented below.<br>
<img width="800" alt="schema_opt_check4" src="https://github.com/Sidv005/Samsung-PD-Training/blob/1120f5ccc4a2f0d02ddace7278fdf882911f995c/%23day9/lab16(p1)/schema_opt_check4.png"><br>

The report timing after linking and compiling the design in presented below.<br>
<img width="500" alt="report_timng_80ps" src="https://github.com/Sidv005/Samsung-PD-Training/blob/1120f5ccc4a2f0d02ddace7278fdf882911f995c/%23day9/lab16(p1)/report_timng_80ps.png"><br>

After constraining the maximum delay to 60 ps using command *setup_max_delay 0.06 -from [all_inputs] -to [get_ports y]* The report is below.<br>
<img width="500" alt="report_timng(slack%20violate)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/1120f5ccc4a2f0d02ddace7278fdf882911f995c/%23day9/lab16(p1)/report_timng(slack%20violate).png"><br>

Further this lohgic cant get optimize The report is below.<br>
<img width="500" alt="further_cant_optimized(slack%20violate)" src="https://github.com/Sidv005/Samsung-PD Training/blob/1120f5ccc4a2f0d02ddace7278fdf882911f995c/%23day9/lab16(p1)/further_cant_optimized(slack%20violate).png"><br>

After setting the cell size of U4 to xnor2_4 we get the violated report as follows:<br>
<img width="500" alt="size_cell(slack%20violate)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/1120f5ccc4a2f0d02ddace7278fdf882911f995c/%23day9/lab16(p1)/size_cell(slack%20violate).png"><br>

After using *compile_ultra* result got better but still violated by 20ps.<br>
<img width="500" alt="size_cell(slack%20violate%2020ps)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/1120f5ccc4a2f0d02ddace7278fdf882911f995c/%23day9/lab16(p1)/size_cell(slack%20violate%2020ps).png"><br>

**Lab on Resource Sharing**

The RTL design file for resource sharing is given below as example.

```ruby
module resource_sharing_mult_check (input [3:0] a , input [3:0] b, input [3:0] c , input [3:0] d, output [7:0] y  , input sel);
   assign y = sel ? (a*b) : (c*d);

endmodule
```
Schematic is shown below.<br>
<img width="800" alt="schema_resource_sharingpng" src="https://github.com/Sidv005/Samsung-PD-Training/blob/0b093254e988145a940d79e9958c273923b36ce7/SamsungPD%23day9%23lab16(p2)/schema_resource_sharingpng"><br>

Below image shows the no.of ports as 25, no. of cells as 37 and area as 342.83. <br>
<img width="500" alt="area_run1" src="https://github.com/Sidv005/Samsung-PD-Training/blob/0b093254e988145a940d79e9958c273923b36ce7/SamsungPD%23day9%23lab16(p2)/area_run1"><br>

Timing report is below:<br>
<img width="500" alt="area_run1_(pathuncons)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/0b093254e988145a940d79e9958c273923b36ce7/SamsungPD%23day9%23lab16(p2)/area_run1_(pathuncons)"><br>

Area report  after setting max delay of 2.5ns and using *compile_ultra* is below:<br>
<img width="500" alt="area_run1_(after_cons)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/0b093254e988145a940d79e9958c273923b36ce7/SamsungPD%23day9%23lab16(p2)/area_run1_(after_cons)"><br>

After setting max delay of 0.1ns from *sel* to outputs timing report is shown as follows:<br>
<img width="500" alt="timing_run2_(slack_violate)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/0b093254e988145a940d79e9958c273923b36ce7/SamsungPD%23day9%23lab16(p2)/timing_run2_(slack_violate)"><br>

Schematic is given below:<br>
<img width="800" alt="schema_run2_(962)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/0b093254e988145a940d79e9958c273923b36ce7/SamsungPD%23day9%23lab16(p2)/schema_run2_(962)"><br>

Area report is shown below:<br>
<img width="500" alt="area_run2_(962)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/0b093254e988145a940d79e9958c273923b36ce7/SamsungPD%23day9%23lab16(p2)/area_run2_(962)"><br>

After applying *set_max_area 800* Timing report is shown below:<br>
<img width="500" alt="timing_run3_(slackmet)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/0b093254e988145a940d79e9958c273923b36ce7/SamsungPD%23day9%23lab16(p2)/timing_run3_(slackmet)"><br>

Area report is shown below:<br>
<img width="500" alt="area_run3_(783)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/0b093254e988145a940d79e9958c273923b36ce7/SamsungPD%23day9%23lab16(p2)/area_run3_(783)"><br>

**Labs on Sequential Optimizations**

***Example of Tie cells***
Tie cells, also referred to as tie-high and tie-low cells, play a crucial role in VLSI design by ensuring that particular signals maintain a predefined logic state, irrespective of the input conditions.

The design file for dff_const1.v is below:

```ruby
 module dff_const1(input clk, input reset, output reg q);
  always @(posedge clk, posedge reset)
  begin
  	if(reset)
  		q <= 1'b0;
  	else
  		q <= 1'b1;
  end
endmodule
```
Schematic is shown in the below figure having a flop since its not a sequential constant.<br>
<img width="900" alt="schema(dffconst1)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/16f2d031387302965ed0ec92a2a9ffb3cd4a46f0/SamsungPD%23day9lab17/schema(dffconst1)"><br>

After scripting for cell name and reference name results is shown below.<br>
<img width="900" alt="foreach(dffconst1)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/16f2d031387302965ed0ec92a2a9ffb3cd4a46f0/SamsungPD%23day9lab17/foreach(dffconst1)"><br>

The design file for dff_const2.v is below:
```ruby
module dff_const2(input clk, input reset, output reg q);
always @(posedge clk, posedge reset)
begin
	if(reset)
		q <= 1'b1;
	else
		q <= 1'b1;
end
endmodule
```
Flops are optimized since it has sequential constant as shown below.<br>
<img width="900" alt="schema(dffconst2)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/16f2d031387302965ed0ec92a2a9ffb3cd4a46f0/SamsungPD%23day9lab17/schema(dffconst2)"><br>

After executing *set compile_seqmap_propagate_constants false* we can prevent from removal of flop. Schematic is shown below.<br>
<img width="900" alt="schema_seqmap_false(dffconst2)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/16f2d031387302965ed0ec92a2a9ffb3cd4a46f0/SamsungPD%23day9lab17/schema_seqmap_false(dffconst2)"><br>

The design file for dff_const3.v is below:

```ruby
module dff_const3(input clk, input reset, output reg q);
reg q1;
always @(posedge clk, posedge reset)
begin
	if(reset)
	begin
		q <= 1'b1;
		q1 <= 1'b0;
	end
	else
	begin
		q1 <= 1'b1;
		q <= q1;
	end
end
endmodule
```

Schematic is shown below:<br>
<img width="900" alt="schema(dffconst3)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/16f2d031387302965ed0ec92a2a9ffb3cd4a46f0/SamsungPD%23day9lab17/schema(dffconst3)"><br>

The design file for dff_const4.v is below:

```ruby
module dff_const4(input clk, input reset, output reg q);
reg q1;
always @(posedge clk, posedge reset)
begin
	if(reset)
	begin
		q <= 1'b1;
		q1 <= 1'b1;
	end
	else
	begin
		q1 <= 1'b1;
		q <= q1;
	end
end
endmodule
```
Schematic is shown below:<br>
<img width="900" alt="schema(dffconst4)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/16f2d031387302965ed0ec92a2a9ffb3cd4a46f0/SamsungPD%23day9lab17/schema(dffconst4)"><br>


After executing *set compile_seqmap_propagate_constants true* shows tie cell of logic 1. Schematic is shown below.<br>
<img width="600" alt="schema_seqmap_true(dffconst4)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/16f2d031387302965ed0ec92a2a9ffb3cd4a46f0/SamsungPD%23day9lab17/schema_seqmap_true(dffconst4)"><br>

The design file for dff_const5.v is below:

```ruby
module dff_const5(input clk, input reset, output reg q);
reg q1;

always @(posedge clk, posedge reset)
begin
	if(reset)
	begin
		q <= 1'b0;
		q1 <= 1'b0;
	end
	else
	begin
		q1 <= 1'b1;
		q <= q1;
	end
end

endmodule
```
Schematic is shown below:<br>
<img width="900" alt="schema(dffconst5)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/16f2d031387302965ed0ec92a2a9ffb3cd4a46f0/SamsungPD%23day9lab17/schema(dffconst5)"><br>

After executing *set compile_seqmap_propagate_constants true*. Schematic is shown below.<br>
<img width="900" alt="schema_seqmap_true(dffconst5)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/16f2d031387302965ed0ec92a2a9ffb3cd4a46f0/SamsungPD%23day9lab17/schema_seqmap_true(dffconst5)"><br>

</details>

<details>
 <summary> Labs on Special Optimizations</summary>
	
***Boundary Optimization***

When sub module is having any logic which is connected to another logic present in top module then tool may vanish the boundary between the module and combine the logic circuit within a single top module.
Benefit is that we an get best optimized logic but a drawback is that if we want to perform any further changes in design it will be very difficult in future.

```ruby
module check_boundary (input clk , input res , input [3:0] val_in , output reg [3:0] val_out);
wire en;
internal_module u_im (.clk(clk) , .res(res) , .cnt_roll(en));

always @ (posedge clk , posedge res)
begin
	if(res)
		val_out <= 4'b0;
	else if(en)
		val_out <= val_in;	
end
endmodule

module internal_module (input clk , input res , output cnt_roll);
reg [2:0] cnt;

always @(posedge clk , posedge res)
begin
	if(res)
		cnt <= 3'b0;
	else
		cnt <= cnt + 1;
end

assign cnt_roll = (cnt == 3'b111);
endmodule
```

Below figure shows the circuit without boundary as we can see *u_im cells* within the logic circuit.<br>
<img width="900" alt="without_boundary" src="https://github.com/Sidv005/Samsung-PD-Training/blob/79dc237cef7c5ed354cb3c8b689c8806a8d20730/SamsungPD%23day9%23lab18/without_boundary"><br>

After running *set_boundary_optimization u_im false* we can prevent the removal of u_im boundary (submodule) within the top module. We can view the hierarchy. Below schematic shows the same.<br>
<img width="900" alt="with_boundary" src="https://github.com/Sidv005/Samsung-PD-Training/blob/79dc237cef7c5ed354cb3c8b689c8806a8d20730/SamsungPD%23day9%23lab18/with_boundary"><br>

***Register Retiming***

Register retiming is a strategy employed in Very Large Scale Integration (VLSI) design to enhance the efficiency of digital circuits by repositioning the registers within the circuit, all the while preserving its functionality. The primary objective of register retiming is to reduce the critical path delay, which is the lengthiest route in the circuit from an input to an output.<br>
<img width="700" alt="rr" src="https://github.com/Sidv005/Samsung-PD-Training/blob/bd883714c7c6e1c23a743fc91690d9dffd741220/SamsungPD%23day9%23lab19/rr.png"><br>

In case1 combinational logic is too huge so we obtain critcical path delay of 50ns i.e max frequency = 20MHz. But when combinational logic is spilted and 2 more flip flops are added in circuit then we obtain  critcical path delay of 20ns i.e max frequency = 50MHz. 

Let's explore an example involving a 4-bit multiplier tasked with multiplying two 4-bit numbers, with the product data being transferred through a trio of 8-bit registers on its path to the output.

```ruby
module check_reg_retime (input clk , input [3:0] a, input [3:0] b , output [7:0] c , input reset);
wire [7:0] mult;
assign mult = a * b;
reg [7:0] q1;
reg [7:0] q2;
reg [7:0] q3;
always @ (posedge clk , posedge reset)
begin
	if(reset)
	begin
		q1 <= 8'b0;
		q2 <= 8'b0;
		q3 <= 8'b0;
	end
	else
	begin
		q1 <= mult;
		q2 <= q1;
		q3 <= q2;
	end
end
assign c = q3;
endmodule
```

The schematic before retime is shown below.<br>
<img width="800" alt="rr" src="https://github.com/Sidv005/Samsung-PD-Training/blob/bd883714c7c6e1c23a743fc91690d9dffd741220/SamsungPD%23day9%23lab19/schema_retime1"><br>

tcl script is used to apply constraints which is as follows:<br>
<img width="600" alt="reg_retime_const_tcl" src="https://github.com/Sidv005/Samsung-PD-Training/blob/bd883714c7c6e1c23a743fc91690d9dffd741220/SamsungPD%23day9%23lab19/reg_retime_const_tcl"><br>

After constraing the design timing report is analysed which shows slack violation as shown below.<br>
<img width="600" alt="report_time(const_tcl)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/bd883714c7c6e1c23a743fc91690d9dffd741220/SamsungPD%23day9%23lab19/report_time(const_tcl)"><br>

We retime it using following command
*compile_ultra -retime*  
The timing report is given below.<br>
<img width="600" alt="report_time(after_compile_ultra)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/bd883714c7c6e1c23a743fc91690d9dffd741220/SamsungPD%23day9%23lab19/report_time(after_compile_ultra)"><br>

***Isolating Output ports***

In the field of VLSI (Very Large Scale Integration) design, the term "isolating output ports" commonly denotes the practice of guaranteeing that the output signals from a circuit or module are effectively separated, preventing unwanted interference among themselves or with other system components. This isolation is vital to preserve signal integrity, minimize noise, and avert unintended interactions.
Let's examine the following scenario: In a given example, there are multiple outputs to be connected after the implementation of a design. This situation can potentially lead to internal delay violations, as the cell delay is influenced by the load capacitance. To prevent internal failures, a solution is to insert a buffer at the output port. Consequently, the buffer takes on the role of driving the external load, effectively decoupling the internal paths from the output paths.<br>
<img width="600" alt="iso_ckt" src="https://github.com/Sidv005/Samsung-PD-Training/blob/9f7fd8a4d30fb247be7d9384c0f92cc36091e65f/SamsungPD%23day9%23lab20/iso_ckt.png"><br>

Design file is mentioned below.

```ruby
module check_boundary (input clk , input res , input [3:0] val_in , output reg [3:0] val_out);
wire en;
internal_module u_im (.clk(clk) , .res(res) , .cnt_roll(en));

always @ (posedge clk , posedge res)
begin
	if(res)
		val_out <= 4'b0;
	else if(en)
		val_out <= val_in;	
end
endmodule

module internal_module (input clk , input res , output cnt_roll);
reg [2:0] cnt;
always @(posedge clk , posedge res)
begin
	if(res)
		cnt <= 3'b0;
	else
		cnt <= cnt + 1;
end

assign cnt_roll = (cnt == 3'b111);
endmodule
```

The schematic prior to isolate is shown below.<br>
<img width="600" alt="zoom_in_out_load" src="https://github.com/Sidv005/Samsung-PD-Training/blob/0d717765c73f126bbab7af939fed04a74edef884/SamsungPD%23day9%23lab20/zoom_in_out_load"><br>

Timing report before isolate command is as follows:<br>
<img width="600" alt="timing(before_iso)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/7534197241139f86a34ce81127385f77f08399c0/SamsungPD%23day9%23lab20/timing(before_iso).png"><br>

The command for isolating ports

set_isolate_ports -type buffer [all_outputs]

The Schematic after isolating the ports is in below figure.<br>
<img width="600" alt="added_buffer" src="https://github.com/Sidv005/Samsung-PD-Training/blob/7534197241139f86a34ce81127385f77f08399c0/SamsungPD%23day9%23lab20/added_buffer"><br>

Timing report after isolate command is as follows:<br>
<img width="600" alt="after_iso" src="https://github.com/Sidv005/Samsung-PD-Training/blob/04dd72a3ced47298dfb8f2eb56a5da0dff31b82c/SamsungPD%23day9%23lab20/after_iso.png"><br>

***False_paths***

False paths are non-critical paths within a digital circuit that do not need to meet timing constraints. Recognizing and managing them is a vital aspect of VLSI design to optimize timing analysis, resource allocation, and overall design efficiency. The identification and proper handling of false paths are crucial for accurate timing analysis, optimizing resource utilization, meeting timing closure, and ensuring the overall functionality and performance of the integrated circuit.

***Multicycle path***

A multicycle path in VLSI design is a timing path where the clock signal does not adhere to the usual single-cycle constraints. It allows for flexibility in meeting timing requirements and is used for specific design scenarios where standard synchronous timing does not apply or is not necessary.

The RTL design code
```ruby
module mcp_check (input clk , input res  , input [7:0] a , input [7:0] b, input en , output reg [15:0] prod);
reg valid; 
always @ (posedge clk , posedge res)
begin
	if(res)
		valid <= 1'b0;
	else 
		valid <= en;
end

always @ (posedge clk , posedge res)
begin
	if(res)
		prod <= 16'b0;
	else if (valid)
		prod <= a * b;
end
endmodule
```
Following is a tcl script for applying constraints.<br>
<img width="500" alt="mcp_tcl" src="https://github.com/Sidv005/Samsung-PD-Training/blob/109a8eff00f7e7b4cb444a6d36dd1ed6fe9b9411/SamsungPD%23day9%23lab21/mcp_tcl.png"><br>

Timing report before optimization is shown below.<br>
<img width="600" alt="violated1" src="https://github.com/Sidv005/Samsung-PD-Training/blob/109a8eff00f7e7b4cb444a6d36dd1ed6fe9b9411/SamsungPD%23day9%23lab21/violated1"><br>

<img width="600" alt="violated2" src="https://github.com/Sidv005/Samsung-PD-Training/blob/109a8eff00f7e7b4cb444a6d36dd1ed6fe9b9411/SamsungPD%23day9%23lab21/violated2"><br>

Now below command is used to meet slack

*set_multicycle_path -setup 2 -to prod_reg[*]/D -from [all_inputs]*

Timing report is shown in below figure.<br>
<img width="600" alt="slackmet1" src="https://github.com/Sidv005/Samsung-PD-Training/blob/109a8eff00f7e7b4cb444a6d36dd1ed6fe9b9411/SamsungPD%23day9%23lab21/slackmet1"><br>
<img width="600" alt="slackmet2" src="https://github.com/Sidv005/Samsung-PD-Training/blob/109a8eff00f7e7b4cb444a6d36dd1ed6fe9b9411/SamsungPD%23day9%23lab21/slackmet2"><br>

When we give *report_timing -delay min* we get the violated report as we have only optimized setup path and not hold path.<br>
<img width="600" alt="mcp_hold_time1" src="https://github.com/Sidv005/Samsung-PD-Training/blob/0836b7d124f7256e92c82204e47634f0308f9b6d/SamsungPD%23day9%23lab21/mcp_hold_time1.png"><br>

Optimizing the hold path is done by the following command

*set_multicycle_path -hold 1 -to prod_reg[]/D -from [all_inputs] -to prod_reg[]/D*

Timing report after optimizing hold path.<br>
<img width="600" alt="mcp_hold_time2" src="https://github.com/Sidv005/Samsung-PD-Training/blob/0836b7d124f7256e92c82204e47634f0308f9b6d/SamsungPD%23day9%23lab21/mcp_hold_time2.png"><br>

But the output slack is not met , because huge load on the output end.<br>
<img width="600" alt="mcp_hold_time3" src="https://github.com/Sidv005/Samsung-PD-Training/blob/0836b7d124f7256e92c82204e47634f0308f9b6d/SamsungPD%23day9%23lab21/mcp_hold_time3.png"><br>

We can rectify this issue by isolating the port.<br>
<img width="600" alt="mcp_hold_time4" src="https://github.com/Sidv005/Samsung-PD-Training/blob/0836b7d124f7256e92c82204e47634f0308f9b6d/SamsungPD%23day9%23lab21/mcp_hold_time4.png"><br>

</details>

## Day-10-QOR ##
<details>
 <summary> Report_timing</summary>
	Quality checks play a pivotal role in the world of Very Large Scale Integration (VLSI) design and manufacturing, serving as essential safeguards to guarantee the reliability and functionality of integrated circuits (ICs). These quality checks span the entirety of the design and manufacturing phases, encompassing a range of stages aimed at detecting and addressing potential issues.

In VLSI, the process of ensuring quality is an ongoing and iterative one, maintaining a persistent presence from start to finish. This steadfast commitment to quality is driven by the overarching goals of ensuring reliability, optimizing performance, and enhancing the manufacturability of integrated circuits. To execute these checks efficiently, the industry leverages advanced simulation and verification tools, which not only automate but also streamline the entire quality assurance process.

Rising Edge Propagation Delay (tpdr) is the duration required for the output signal to shift from a low (0) to a high (1) level following a corresponding transition in the input signal.

Falling Edge Propagation Delay (tpdf) signifies the elapsed time for the output signal to shift from a high (1) to a low (0) level following a commensurate transition in the input signal.<br>
<img width="600" alt="fig1" src="https://github.com/Sidv005/Samsung-PD-Training/blob/90ed46d77a3e3126388d76cc77630401a1e8e7bb/SamsungPD%23day10/lab1/fig1.png"><br>

Inverter gate :

A rise -> Y fall (0.5 ns)

A fall -> Y rise (0.4 ns)

AND gate :

A rise -> Y rise (0.7 ns)

A fall -> Y fall (0.65 ns)

B rise -> Y rise (0.65 ns)

B fall -> Y fall (0.6 ns)

Now the different timing paths along with delays are as follows

1. DFFA(Clk -> Q r) -> INV(A r) -> INV(Y f) -> AND(A f) -> AND(Y f) -> DFFC(f)

0.5 + 0.5 + 0.65 = 1.65ns

2. DFFA(Clk -> Q f) -> INV(A f) -> INV(Y r) -> AND(A r) -> AND(Y r) -> DFFC(f)

0.4 + 0.4 + 0.7 = 1.5ns

3. DFFA(Clk -> Q r) -> AND(B r) -> AND(Y r) -> DFFC(r)

0.5 + 0.65 = 1.15 ns

4. DFFA(Clk -> Q f) -> AND(B f) -> AND(Y f) -> DFFC(f)

0.4 + 0.6 = 1.0 ns

The critical path refers to the longest path through the digital circuit that determines the maximum time it takes for a signal to propagate from the input to the output. It plays a crucial role in determining the overall performance and speed of the integrated circuit (IC).

Following commands with their corresponding results are shown below.

- report_timing -from DFFA/CLK -to DFFC/D -delay max

we obtain the first path

- report_timing -from DFFA/CLK -to DFFC/D -delay min

we obtain the second path

- report_timing -delay max -from DFFB/D -to DFFC/D

we obtain the third path

- report_timing -delay min -to DFFC/D

we obtain fourth path

- report_timing -delay max -rise_to DFFC/D

we obtain the second path

- report_timing -delay max -fall_to DFFC/D

we obtain the first path

Let us consider the clock period as 5 ns, setup time is 0.5 ns and hold time is 0.4 ns.

DFFA(Clk -> Q r) -> INV(A r) -> INV(Y f) -> AND(A f) -> AND(Y f) -> DFFC(f)

0.5 + 0.5 + 0.65 = 1.65ns

This time is called as arrival time

Required time = Clock period - setup time -uncertainty

5 - 0.5 - 0 = 4.5ns

setup slack = Required - Arrival = (4.5 - 1.65 = 2.85 ns)

Hold Time of DFFC = 0.1ns

DFFB(Clk -> Q f) -> AND(A f) -> AND(Y f) -> DFFC(f)

0.4 + 0.6 = 1.0 ns

Required time = hold time + uncertainity = 0.1 + 0 = 0.1 ns

Hold slack = Arrival - Required = (1 - 0.1 = 0.9 ns)

Let us consider another example<br>
<img width="600" alt="fig2" src="https://github.com/Sidv005/Samsung-PD-Training/blob/f8d29770848051bd10af62f1bf1299b5faaa0c1e/SamsungPD%23day10/lab1/fig2.png"><br>

- report_timing -max_paths 2

This command results to the two worst slack paths one from each endpoint. In this case the path with slacks -1.2 ns and -1.0 ns will be shown.

- report_timing -max_paths 2 -nworst 2

This command results to the worst slack , In this example it is -1.2 ns and -1.1 ns

</details>

<details>
 <summary>Lab on Report timing </summary>
The example used is lab8_circuit_modified.v having the following design code.

```ruby
module lab8_circuit (input rst, input clk , input IN_A , input IN_B , output OUT_Y , output out_clk , output reg out_div_clk);
reg REGA , REGB , REGC ; 

always @ (posedge clk , posedge rst)
begin
   if(rst)
   begin
   	REGA <= 1'b0;
   	REGB <= 1'b0;
   	REGC <= 1'b0;
   	out_div_clk <= 1'b0;
   end
   else
   begin
   	REGA <= IN_A | IN_B;
   	REGB <= IN_A ^ IN_B;
   	REGC <= !(REGA & REGB);
   	out_div_clk <= ~out_div_clk; 
   end
end

assign OUT_Y = ~REGC;

assign out_clk = clk;

endmodule
```
Following tcl script is used to apply the constraints.<br>
<img width="600" alt="lab8_cons_tcl" src="https://github.com/Sidv005/Samsung-PD-Training/blob/c17cfcc834bfadb028b7b3755b36c10ad7a95b52/SamsungPD%23day10/lab1/lab8_cons_tcl.png"><br>

Now for doing setup check following command is run.
- report_timing -sig 4 -cap -nets -trans -nosplit -inp <br>
<img width="600" alt="lab8_rep_time1" src="https://github.com/Sidv005/Samsung-PD-Training/blob/c17cfcc834bfadb028b7b3755b36c10ad7a95b52/SamsungPD%23day10/lab1/lab8_rep_time1.png"><br>

 Now we use *report_timing -sig 4 -cap -nets -trans -nosplit -inp -from IN_A > t1.rpt*
 <img width="600" alt="t1_rpt" src="https://github.com/Sidv005/Samsung-PD-Training/blob/c17cfcc834bfadb028b7b3755b36c10ad7a95b52/SamsungPD%23day10/lab1/t1_rpt.png"><br>

 Now we use *report_timing -sig 4 -cap -nets -trans -nosplit -inp -rise_from IN_A > t2.rpt*
 <img width="600" alt="t2(rise)_rpt" src="https://github.com/Sidv005/Samsung-PD-Training/blob/c17cfcc834bfadb028b7b3755b36c10ad7a95b52/SamsungPD%23day10/lab1/t2(rise)_rpt.png"><br>

Comparing t1.rp and t2.rpt observe rise to fall and fall to rise delay mismatch in nor and inv gates.
 <img width="600" alt="comp_t1_t2_rpt" src="https://github.com/Sidv005/Samsung-PD-Training/blob/c17cfcc834bfadb028b7b3755b36c10ad7a95b52/SamsungPD%23day10/lab1/comp_t1_t2_rpt.png"><br>

Now we use *report_timing -sig 4 -cap -nets -trans -nosplit -inp -rise_from IN_A -to REGA_reg/D > t3.rpt*
Comparing t1.rp and t3.rpt observe rise to fall and fall to rise delay mismatch in U14 and U12 cells.
 <img width="600" alt="comp_t1_t3_rpt" src="https://github.com/Sidv005/Samsung-PD-Training/blob/c17cfcc834bfadb028b7b3755b36c10ad7a95b52/SamsungPD%23day10/lab1/comp_t1_t3_rpt.png"><br>

Now we use *report_timing -delay min -from IN_A*. It is reporting U15 in REGA to REGB
Observe hold check in below screenshot<br>
<img width="600" alt="min_delay(from%20A)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/c17cfcc834bfadb028b7b3755b36c10ad7a95b52/SamsungPD%23day10/lab1/min_delay(from%20A).png"><br>

Now we use *report_timing -thr U15/Y*
Observe delay of 50ps in U15.<br>
<img width="600" alt="through_U15(50ps)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/c17cfcc834bfadb028b7b3755b36c10ad7a95b52/SamsungPD%23day10/lab1/through_U15(50ps).png"><br>

Now we run *report_timing -thr U15/Y -delay min*<br>
<img width="600" alt="through_U15(70ps)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/c17cfcc834bfadb028b7b3755b36c10ad7a95b52/SamsungPD%23day10/lab1/through_U15(70ps).png"><br>

Conclude that for max_delay tool shows worst path according to total delay irrespective of cell contribution.
</details>

<details>
 <summary>Lab on Check_timing,design,set max_cap </summary>
Human error may happen like not constrainging all paths and not loading design properly. Therefore tool must have commands to overcome this.

*check_design* is used to check whether design is linked properly or not.

*check_timing* is used to display all the endpoints which are unconstrained<br>
<img width="600" alt="check_time1" src="https://github.com/Sidv005/Samsung-PD-Training/blob/29bbf554c5a2da7665bc2b35db0fdca2417f8cc5/SamsungPD%23day10/lab2/check_time1.png"><br>

*report_constraints* used to give the default value of the constraints<br>
<img width="600" alt="rep_cons1" src="https://github.com/Sidv005/Samsung-PD-Training/blob/29bbf554c5a2da7665bc2b35db0fdca2417f8cc5/SamsungPD%23day10/lab2/rep_cons1.png"><br>

After contraining the paths using.tcl script run *check timing*<br>
<img width="600" alt="check_timing1" src="https://github.com/Sidv005/Samsung-PD-Training/blob/29bbf554c5a2da7665bc2b35db0fdca2417f8cc5/SamsungPD%23day10/lab2/check_timing1.png"><br>
From above image observe that all other unconstrained paths are removed only clocks are remaining.<br>

Now run *report_timing*<br>
<img width="600" alt="rep_timing1" src="https://github.com/Sidv005/Samsung-PD-Training/blob/29bbf554c5a2da7665bc2b35db0fdca2417f8cc5/SamsungPD%23day10/lab2/rep_timing1.png"><br>

Now run *report_constraints*<br>
<img width="600" alt="rep_cons1.1" src="https://github.com/Sidv005/Samsung-PD-Training/blob/29bbf554c5a2da7665bc2b35db0fdca2417f8cc5/SamsungPD%23day10/lab2/rep_cons1.1.png"><br>
Observe no negative slack is present above.<br>

Consider an example of 128 : 1 Mux

Following is the design code
```ruby
module mux_generate ( input [127:0] in, input [6:0] sel, output reg y);
integer k;
always @ (*)
begin
for(k = 0; k < 128; k=k+1) begin
	if(k == sel)
		y = in[k];
end
end
endmodule
```
After reading verilog file we see a latch which is due to usage of always block.<br> 
<img width="600" alt="mux_gen_read_verilog" src="https://github.com/Sidv005/Samsung-PD-Training/blob/29bbf554c5a2da7665bc2b35db0fdca2417f8cc5/SamsungPD%23day10/lab2/mux_gen_read_verilog.png"><br>

After running link and compile_ultra we execute *write -f verilog -out mux_generate_128_net.v* to get the netlist as shown below.<br>
<img width="600" alt="mux_gen_write_netlist" src="https://github.com/Sidv005/Samsung-PD-Training/blob/29bbf554c5a2da7665bc2b35db0fdca2417f8cc5/SamsungPD%23day10/lab2/mux_gen_write_netlist.png"><br>

From the above image we should see that hierarchical cells of sequential type are not present this is presented in below figure.<br>
<img width="1000" alt="mux_gen_get_cells" src="https://github.com/Sidv005/Samsung-PD-Training/blob/29bbf554c5a2da7665bc2b35db0fdca2417f8cc5/SamsungPD%23day10/lab2/mux_gen_get_cells.png"><br>

Run *report_timing* we see caps are negligible.<br>
<img width="600" alt="mux_gen_rep_time_cap(neg)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/29bbf554c5a2da7665bc2b35db0fdca2417f8cc5/SamsungPD%23day10/lab2/mux_gen_rep_time_cap(neg).png"><br>

Now run *check timing* Observe that y is unconstrained.<br>
<img width="600" alt="mux_gen_rep_time_cap(neg)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/29bbf554c5a2da7665bc2b35db0fdca2417f8cc5/SamsungPD%23day10/lab2/mux_gen_check_time(y_uncons).png"><br>

Now run *report_timing* Observe that slack is violated.<br>
<img width="600" alt="mux_gen_rep_time(slack_vio)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/29bbf554c5a2da7665bc2b35db0fdca2417f8cc5/SamsungPD%23day10/lab2/mux_gen_rep_time(slack_vio).png"><br>

We set the max capacitance

set_max_capacitance 0.025 [current_design]

Now run *report_constraints -all_violators*. Observe that slack violated of many paths.<br>
<img width="600" alt="mux_gen_rep_cons(slack_vio)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/29bbf554c5a2da7665bc2b35db0fdca2417f8cc5/SamsungPD%23day10/lab2/mux_gen_rep_cons(slack_vio).png"><br>

After *compile_ultra* run *report_constraints*. Observe that slack is met.<br>
<img width="600" alt="mux_gen_rep_cons(met)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/29bbf554c5a2da7665bc2b35db0fdca2417f8cc5/SamsungPD%23day10/lab2/mux_gen_rep_cons(met).png"><br>

Run *report_timing* we see arrival time is 3.43ns.<br>
<img width="600" alt="mux_gen_rep_time(arr.t)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/29bbf554c5a2da7665bc2b35db0fdca2417f8cc5/SamsungPD%23day10/lab2/mux_gen_rep_time(arr.t).png"><br>

Run *report_timing -net -cap -sig 4*. Observe that all fanout got splited and cap max is 25fF.<br>
<img width="600" alt="mux_gen_rep_time(cap%3C25fF)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/29bbf554c5a2da7665bc2b35db0fdca2417f8cc5/SamsungPD%23day10/lab2/mux_gen_rep_time(cap%3C25fF).png"><br>

Consider another example of 128 bit enable
 Design code for en_128.v is given below.
 ```ruby
module en_128 (input [127:0] x , output [127:0] y , input en);
	assign y[127:0] = en ?x[127:0]:128'b0;
endmodule
```
After reading verilog file and linking we get timing report showing 128 fanouts as follows.<br>
<img width="600" alt="en(fanout_128)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/29bbf554c5a2da7665bc2b35db0fdca2417f8cc5/SamsungPD%23day10/lab2/en(fanout_128).png"><br>

after setting the max cap as 0.03

Run *report_constraints*<br>
<img width="600" alt="en(rep_cons_cap_vio)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/29bbf554c5a2da7665bc2b35db0fdca2417f8cc5/SamsungPD%23day10/lab2/en(rep_cons_cap_vio).png"><br>

Now run *compile_ultra* and observe the timing report showing 17 fanouts.<br>
<img width="600" alt="en(rep_time_fanout_17)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/29bbf554c5a2da7665bc2b35db0fdca2417f8cc5/SamsungPD%23day10/lab2/en(rep_time_fanout_17).png"><br>

Now see the schematic in Design_vison by writing out ddc. <br>
<img width="600" alt="en(rep_time_fanout_17)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/29bbf554c5a2da7665bc2b35db0fdca2417f8cc5/SamsungPD%23day10/lab2/en(schema).png"><br>

Now run *report_timing -from en -nets -cap -sig 4 -trans*<br>
<img width="900" alt="en(schema)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/29bbf554c5a2da7665bc2b35db0fdca2417f8cc5/SamsungPD%23day10/lab2/en(rep_time_trans_bad).png"><br>

Before compile ultra *report_constraints*<br>
<img width="600" alt="en(rep_cons_trans_vio)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/29bbf554c5a2da7665bc2b35db0fdca2417f8cc5/SamsungPD%23day10/lab2/en(rep_cons_trans_vio).png"><br>

Now run *report_constraints -all_violators*<br>
<img width="600" alt="en(rep_cons_violators)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/29bbf554c5a2da7665bc2b35db0fdca2417f8cc5/SamsungPD%23day10/lab2/en(rep_cons_violators).png"><br>

Now run *set_max_transition 0.150 [current_design]* and run compile_ultra. Observe constraints showning no transition violation.<br>
<img width="600" alt="en(rep_cons_violators_noviolation)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/29bbf554c5a2da7665bc2b35db0fdca2417f8cc5/SamsungPD%23day10/lab2/en(rep_cons_violators_noviolation).png"><br>

Timing report is obtained showing transition < 150ps.<br>
<img width="600" alt="en(rep_time_tran%3C150ps)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/29bbf554c5a2da7665bc2b35db0fdca2417f8cc5/SamsungPD%23day10/lab2/en(rep_time_tran%3C150ps).png"><br>

Now run *report_timing -nosplit -sig 4 -inp -trans -cap -from en -to y[116]*.<br>
<img width="600" alt="en(rep_time_y116)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/29bbf554c5a2da7665bc2b35db0fdca2417f8cc5/SamsungPD%23day10/lab2/en(rep_time_y116).png"><br>

After comparing the above timing report with below it is concluded that data arrival time is reduced. Hence overall delay is improved.<br>
<img width="600" alt="en(rep_time_a.t%3D0.4425_compare)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/29bbf554c5a2da7665bc2b35db0fdca2417f8cc5/SamsungPD%23day10/lab2/en(rep_time_a.t%3D0.4425_compare).png"><br>
</details>

## Day 11: SOC ##
<details>
 <summary>Summary on SOC </summary>
The Qualcomm Snapdragon 660 is a mobile system-on-chip (SoC) designed for smartphones and other mobile devices. It was announced in 2017 and is part of Qualcomm's Snapdragon 600 series, which is positioned as a mid-range chipset with a good balance of performance and power efficiency. Let's take a closer look at its architecture:

- ***CPU (Central Processing Unit)***:

The Snapdragon 660 features an octa-core CPU, which means it has eight individual processing cores.
It uses a combination of ARM Cortex-A73 and Cortex-A53 cores arranged in a big.LITTLE configuration. This means there are four high-performance Cortex-A73 cores and four power-efficient Cortex-A53 cores.
The Cortex-A73 cores are used for demanding tasks and provide higher performance, while the Cortex-A53 cores handle less intensive tasks to save power.
The CPU cores are clocked at various frequencies to balance performance and power efficiency, with the Cortex-A73 cores typically running at higher clock speeds than the Cortex-A53 cores.

- ***GPU (Graphics Processing Unit)***:

The Snapdragon 660 incorporates the Adreno 512 GPU, which is designed to provide good graphics performance for gaming and multimedia applications.
The Adreno 512 supports various graphics technologies and APIs, enabling smooth gaming experiences and high-quality graphics rendering.

- ***Hexagon DSP (Digital Signal Processor)***:

The Hexagon DSP is a specialized processor designed for handling tasks related to audio, video, and other digital signal processing tasks efficiently.
It helps improve the performance and power efficiency of tasks such as voice recognition, image processing, and audio enhancements.

- ***ISP (Image Signal Processor)***:

The Snapdragon 660 includes an advanced Image Signal Processor (ISP) for processing images and videos from the device's camera.
It supports features like high-quality image capture, video recording, and advanced image post-processing.

- ***Connectivity***:

The SoC features an integrated X12 LTE modem, providing fast download and upload speeds over 4G LTE networks.
It also includes support for various wireless connectivity options, including Wi-Fi, Bluetooth, and NFC.

- ***Manufacturing Process***:

The Snapdragon 660 is manufactured using a 14nm FinFET process technology, which helps to strike a balance between performance and power efficiency.

- ***Security***:

Qualcomm's Secure Processing Unit (SPU) provides hardware-based security features, including support for fingerprint recognition and encryption.
Overall, the Snapdragon 660 is a mid-range SoC with a capable CPU-GPU combination, efficient power management, and support for various multimedia and connectivity features. It's suitable for mid-range smartphones and offers a good balance of performance and battery life. Keep in mind that this information is accurate as of my last knowledge update in September 2021, and there may have been newer iterations or advancements in Qualcomm's chipsets since then.
</details>

## Day 12- Overview on BabySoc ##

<details>
 <summary>LABS on Half Adder</summary>
To develop a half adder and simulate it. Design code is given below followed by the testbench.<br>
<img width="600" alt="ha_code" src="https://github.com/Sidv005/Samsung-PD-Training/blob/af2ae66cf4766e165ce2e8c0c83b0251d217f84b/SamsungPD%23day12/ha_code.png"><br>
Testbench is as follows.<br>
<img width="600" alt="tb_ha" src="https://github.com/Sidv005/Samsung-PD-Training/blob/af2ae66cf4766e165ce2e8c0c83b0251d217f84b/SamsungPD%23day12/tb_ha.png"><br>
simulated waveform:-<br>
<img width="600" alt="ha_wave" src="https://github.com/Sidv005/Samsung-PD-Training/blob/af2ae66cf4766e165ce2e8c0c83b0251d217f84b/SamsungPD%23day12/ha_wave.png"><br>
</details>

<details>
 <summary>LABS on BabySOC modelling</summary>
Initially we model rvmyth following is the command:-
	
```ruby
iverilog mythcore_test.v tb_mythcore_test.v 
./a.out
gtkwave tb_mythcore_test.vcd
```

Simulated waveform is shown below.<br>
<img width="600" alt="wave_myth" src="https://github.com/Sidv005/Samsung-PD-Training/blob/af2ae66cf4766e165ce2e8c0c83b0251d217f84b/SamsungPD%23day12/wave_myth.png"><br>

Now we model DAC following is the command:-
```ruby
iverilog avsddac.v avsddac_tb_test.v
./a.out
gtkwave avsddac_tb_test.vcd
```
Simulated waveform is shown below.<br>
<img width="600" alt="wave_dac" src="https://github.com/Sidv005/Samsung-PD-Training/blob/af2ae66cf4766e165ce2e8c0c83b0251d217f84b/SamsungPD%23day12/wave_dac.png"><br>

Now we model PLL following is the command:-
```ruby
iverilog avsd_pll_1v8.v pll_tb.v
./a.out
gtkwave test.vcd
```
Simulated waveform is shown below.<br>
<img width="600" alt="wave_pll" src="https://github.com/Sidv005/Samsung-PD-Training/blob/af2ae66cf4766e165ce2e8c0c83b0251d217f84b/SamsungPD%23day12/wave_pll.png"><br>

Now we model the interface DAC with rvmyth following is the command:-
```ruby
iverilog rvmyth_avsddac.v rvmyth_avsddac_TB.v
./a.out
gtkwave rvmyth_avsddac.vcd
```
Simulated waveform is shown below.<br>
<img width="600" alt="wave_rvmyth_dac" src="https://github.com/Sidv005/Samsung-PD-Training/blob/af2ae66cf4766e165ce2e8c0c83b0251d217f84b/SamsungPD%23day12/wave_rvmyth_dac.png"><br>

Now we model the interface PLL with rvmyth following is the command:-
```ruby
iverilog rvmyth_pll.v rvmyth_pll_tb.v
./a.out
gtkwave test1.vcd
```
Simulated waveform is shown below.<br>
<img width="600" alt="wave_rvmyth_pll" src="https://github.com/Sidv005/Samsung-PD-Training/blob/af2ae66cf4766e165ce2e8c0c83b0251d217f84b/SamsungPD%23day12/wave_rvmyth_pll.png"><br>

Now we model the interface of all the modules following is the command:-
```ruby
iverilog vsdbabysoc.v testbench.v avsdpll.v avsddac.v mythcore_test.v
./a.out
gtkwave dump.vcd
```
Simulated waveform is shown below.<br>
<img width="600" alt="wave_vsdbabysoc" src="https://github.com/Sidv005/Samsung-PD-Training/blob/af2ae66cf4766e165ce2e8c0c83b0251d217f84b/SamsungPD%23day12/wave_vsdbabysoc.png"><br>
</details>

## Day 13- Demonstration of Post synthesis ##

<details>
 <summary>LABS ON SYNTHESIS OF HALF ADDER</summary>
Here post synthesis is done in dc_shell. Following commands are used to perform synthesis.

```ruby
set target_library <path_of_target_library>
set link library { * <path_of_target_library> }
read_verilog ha.v
link
compile_ultra
```
Schematic view of half adder is shown below.
<img width="600" alt="ha_schema" src="https://github.com/Sidv005/Samsung-PD-Training/blob/45ac2ac38a7179b2ceb5cc87695ec359fa3b898e/SamsungPD%23day13/ha_schema.png"><br>

Command used to write netlist is:-
- write -f verilog ha_net.v

Netlist code is as follows:<br>
<img width="600" alt="ha_netlist" src="https://github.com/Sidv005/Samsung-PD-Training/blob/45ac2ac38a7179b2ceb5cc87695ec359fa3b898e/SamsungPD%23day13/ha_netlist.png"><br>

Commands used for simulation
```ruby
iverilog <netlist_file_name> <testbench>
./a.out
gtkwave <vcd_file_name>
```
Simulated waveform is shown below.
<img width="600" alt="post_ha_wave" src="https://github.com/Sidv005/Samsung-PD-Training/blob/45ac2ac38a7179b2ceb5cc87695ec359fa3b898e/SamsungPD%23day13/post_ha_wave.png"><br>
</details>

<details>
 <summary>LABS ON BabySOC Post Simulation</summary>
BabySOC comprises of 3 IP's which are as follows:

1. RVMYTH
2. DAC
3. PLL

Out of these only ***RVMYTH*** is synthesizable

Commands for synthesizing

```ruby
set target_library <path_of_target_library>
set link library { * <path_of_target_library> }
read_verilog mythcore_test.v
link
compile_ultra
write -f verilog -output rvmyth_core_test_net.v
```

Current design is changed to core.
```ruby
current_design core
write -f verilog -out rvmyth_net.v
```

```ruby
iverilog -DFUNCTIONAL -DUNIT_DELAY=#1 rvmyth_net.v tb_mythcore_test.v primitives.v sky130_fd_sc_hd.v
./a.out
gtkwave tb_mythcore_test.vcd
```
Above commands are used to generate the simulated waveform.
Simulated waveform after the synthesis is shown below.<br>
<img width="600" alt="post_syn(mythcore)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/45ac2ac38a7179b2ceb5cc87695ec359fa3b898e/SamsungPD%23day13/post_syn(mythcore).png"><br>

We can observe from the above waveform that the sum of first n natural numbers upto 1000 and then it again decrements in the same manner since the MSB bit of a temporary register becomes high.

***BabySOC Post Synthesis***

Now BabySOC is synthesized using the mythcore_test netlist, PLL and DAC. Commands are as follows:

```ruby
iverilog -DFUNCTIONAL -DUNIT_DELAY=#1 rvmyth_net.v testbench.v primitives.v sky130_fd_sc_hd.v avsddac.v avsdpll.v vsdbabysoc.v
./a.out
gtkwave dump.vcd
```
Simulated waveform after the gate level synthesis is shown below.<br>
<img width="600" alt="post_syn(vsdbabysoc)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/45ac2ac38a7179b2ceb5cc87695ec359fa3b898e/SamsungPD%23day13/post_syn(vsdbabysoc).png"><br>
</details>

## Day-14- Timing Analysis of VSDBabySoC comprising of RISC-V core, PLL and DAC ## 

<details>
 <summary>Basics of PVT Corners </summary>
In VLSI design and semiconductor manufacturing, the term "PVT corners" refers to specific combinations of Process, Voltage, and Temperature conditions used for testing and characterizing integrated circuits. These corners are essential for ensuring that a semiconductor device or integrated circuit functions correctly under a range of operating conditions.

1. **Process Corner**: The process corner represents variations in the manufacturing process. Semiconductor fabrication processes are subject to small variations due to factors like equipment tolerances, material properties, and environmental conditions. The process corner typically includes the following variations:

- Fast Process Corner: This corner represents a scenario where the manufacturing process results in faster transistors with better performance characteristics. It is typically associated with optimistic process parameters.
- Slow Process Corner: This corner represents a scenario where the manufacturing process results in slower transistors with potentially worse performance characteristics. It is typically associated with pessimistic process parameters.
- Nominal Process Corner: This corner represents the expected or average manufacturing process conditions.

2. **Voltage Corner**: The voltage corner refers to variations in the supply voltage provided to the integrated circuit. Integrated circuits need to function correctly across a range of supply voltages, as voltage levels can fluctuate due to factors such as power supply noise or voltage drop across the chip.

- Low Voltage Corner: This corner represents a scenario where the supply voltage is at the lower end of the specified range.
- High Voltage Corner: This corner represents a scenario where the supply voltage is at the higher end of the specified range.
- Nominal Voltage Corner: This corner represents the typical or expected supply voltage.

3. **Temperature Corner**: Temperature can significantly impact the performance of integrated circuits. The temperature corner accounts for variations in temperature conditions.

- Hot Temperature Corner: This corner represents a scenario where the chip is operating at a higher temperature, which can affect the speed and power consumption of the device.
- Cold Temperature Corner: This corner represents a scenario where the chip is operating at a lower temperature.
- Nominal Temperature Corner: This corner represents the expected or typical operating temperature.

By characterizing an integrated circuit's behavior at different combinations of these corners (e.g., fast process, low voltage, hot temperature), designers can ensure that the circuit will work reliably under a wide range of conditions. This testing and characterization process helps identify potential issues and allows for necessary design adjustments, ensuring that the final product meets performance and reliability requirements.

- PVT corners are crucial for designing robust and reliable integrated circuits, especially for applications where variations in operating conditions are expected, such as consumer electronics, automotive, and industrial applications.
</details>

<details>
 <summary>LABS ON TIMING ANALYSIS of BabySoC for different PVT corners  </summary>

Firstly we got the .lib files by cloning https://github.com/Geetima2021/vsdpcvrd.git then .lib is converted to .db file using lc_shell and remove the errors if present.
Following commands are used.
```ruby
read_lib <library_name>
write_lib <library_name> -f db -o <name_of_the_db_file>
```
A constraint file is scripted which is as follows:
```ruby
 set_units -time ns
create_clock -name MYCLK -per 2 [get_pins {pll/CLK}];

set_clock_latency -source 1 [get_clocks MYCLK]
set_clock_uncertainty -setup 0.5 [get_clocks MYCLK]; 
set_clock_uncertainty -hold 0.4 [get_clocks MYCLK]; 

set_input_delay -max 1 -clock \[get_clocks MYCLK] [all_inputs];
set_input_delay -min 0.5 -clock \[get_clocks MYCLK] [all_inputs];
set_output_delay -max 1 -clock \[get_clocks MYCLK] [all_outputs];
set_output_delay -min 0.5 -clock \[get_clocks MYCLK] [all_outputs];

set_input_transition -max 0.2 \[all_inputs];
set_input_transition -min 0.1 \[all_inputs];

set_max_area  800;

set_load -max 0.2 \[all_outputs];
set_load -min 0.1 \[all_outputs];
```
A tcl script is designed to run set of commands for synthesis of VSDbabySoC which are follows:
```ruby
set target_library { <sky130_PVT_corner> , avsddac.db , avsdpll.db}
set link_library {* sky130_PVT_corner> , avsddac.db , avsdpll.db}
read_verilog vsdbabysoc.v
link
source <constraints_file_name>
compile
report_qor
```
Now screenshots of outputs showing the WNS, TNS for setup and hold analysis at different PVT corners are represented below:
1. sky130_fd_sc_hd__ff_100c_1v65<br>
<img width="600" alt="sky130_fd_sc_hd__ff_100c_1v65(violate)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/50ec50344e163ccee14f99156172151e73c8cfcc/SamsungPD%23day15/sky130_fd_sc_hd__ff_100c_1v65(violate).png"><br>

2. sky130_fd_sc_hd__ff_100c_1v95<br>
<img width="600" alt="sky130_fd_sc_hd__ff_100c_1v95(violate)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/50ec50344e163ccee14f99156172151e73c8cfcc/SamsungPD%23day15/sky130_fd_sc_hd__ff_100c_1v95(violate).png"><br>

3. sky130_fd_sc_hd__ff_n40C_1v56<br>
<img width="600" alt="sky130_fd_sc_hd__ff_n40c_1v56(violate)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/50ec50344e163ccee14f99156172151e73c8cfcc/SamsungPD%23day15/sky130_fd_sc_hd__ff_n40c_1v56(violate).png"><br>

4. sky130_fd_sc_hd__ff_n40C_1v65<br>
<img width="600" alt="sky130_fd_sc_hd__ff_100c_1v65(violate)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/50ec50344e163ccee14f99156172151e73c8cfcc/SamsungPD%23day15/sky130_fd_sc_hd__ff_100c_1v65(violate).png"><br>

5. sky130_fd_sc_hd__ff_n40C_1v76<br>
<img width="600" alt="sky130_fd_sc_hd__ff_100c_1v76(violate)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/50ec50344e163ccee14f99156172151e73c8cfcc/SamsungPD%23day15/sky130_fd_sc_hd__ff_40c_1v76(violate).png"><br>

6. sky130_fd_sc_hd__ss_100C_1v40<br>
<img width="600" alt="sky130_fd_sc_hd_ss_100c_1v40(violate)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/50ec50344e163ccee14f99156172151e73c8cfcc/SamsungPD%23day15/sky130_fd_sc_hd_ss_100c_1v40(violate).png">

7.  sky130_fd_sc_hd__ss_100C_1v60<br>
<img width="600" alt="sky130_fd_sc_hd__ss_100c_1v60(violate)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/50ec50344e163ccee14f99156172151e73c8cfcc/SamsungPD%23day15/sky130_fd_sc_hd__ss_100c_1v60(violate).png"><br>

8.  sky130_fd_sc_hd__ss_n40C_1v28<br>
<img width="600" alt="sky130_fd_sc_hd__ss_n40c_1v28(violate)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/50ec50344e163ccee14f99156172151e73c8cfcc/SamsungPD%23day15/sky130_fd_sc_hd__ss_n40c_1v28(violate).png"><br>

9.  sky130_fd_sc_hd__ss_n40C_1v35<br>
<img width="600" alt="sky130_fd_sc_hd__ss_n40c_1v35(violate)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/50ec50344e163ccee14f99156172151e73c8cfcc/SamsungPD%23day15/sky130_fd_sc_hd__ss_n40c_1v35(violate).png"><br>

10.  sky130_fd_sc_hd__ss_n40C_1v40<br>
<img width="600" alt="sky130_fd_sc_hd__ss_n40c_1v40(violate)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/50ec50344e163ccee14f99156172151e73c8cfcc/SamsungPD%23day15/sky130_fd_sc_hd__ss_n40c_1v40(violate).png"><br>

11.  sky130_fd_sc_hd__ss_n40C_1v44<br>
<img width="600" alt="sky130_fd_sc_hd__ss_n40c_1v44(violate)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/50ec50344e163ccee14f99156172151e73c8cfcc/SamsungPD%23day15/sky130_fd_sc_hd_ss_n40c_1v44(violate).png"><br>

12.  sky130_fd_sc_hd__ss_n40C_1v76<br>
<img width="600" alt="sky130_fd_sc_hd_ss_n40c_1v76(violate)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/50ec50344e163ccee14f99156172151e73c8cfcc/SamsungPD%23day15/sky130_fd_sc_hd_ss_n40c_1v76(violate).png"><br>

13.  sky130_fd_sc_hd__tt_25C_1v80<br>
<img width="600" alt="sky130_fd_sc_hd__ff_n40c_1v56(violate)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/50ec50344e163ccee14f99156172151e73c8cfcc/SamsungPD%23day15/sky130_fd_sc_hd__ff_n40c_1v56(violate).png"><br>

- Table and Graph for Setup<br>
 <img width="600" alt="setup_table" src="https://github.com/Sidv005/Samsung-PD-Training/blob/9dcd7fa79215cafc0395461860bfce10c2cfed8c/SamsungPD%23day15/setup_table.png"><br>
 <img width="600" alt="wns_setup" src="https://github.com/Sidv005/Samsung-PD-Training/blob/9dcd7fa79215cafc0395461860bfce10c2cfed8c/SamsungPD%23day15/wns_setup.PNG"><br>
 <img width="600" alt="tns_setup" src="https://github.com/Sidv005/Samsung-PD-Training/blob/9dcd7fa79215cafc0395461860bfce10c2cfed8c/SamsungPD%23day15/tns_setup.PNG"><br>

 -Table and Graph for Hold<br>
 <img width="600" alt="hold_table" src="https://github.com/Sidv005/Samsung-PD-Training/blob/9dcd7fa79215cafc0395461860bfce10c2cfed8c/SamsungPD%23day15/hold_table.PNG"><br>
 <img width="600" alt="whs_hold" src="https://github.com/Sidv005/Samsung-PD-Training/blob/9dcd7fa79215cafc0395461860bfce10c2cfed8c/SamsungPD%23day15/whs_hold.PNG"><br>
 <img width="600" alt="ths_hold" src="https://github.com/Sidv005/Samsung-PD-Training/blob/9dcd7fa79215cafc0395461860bfce10c2cfed8c/SamsungPD%23day15/ths_hold.PNG"><br>

 *Conclusion*:-
 Hold violations significantly occurs in faster cells and setup violations significantly occurs in slower cells.
</details>

## Day-15- Inception of EDA and PDK ## 

<details>
 <summary>Introduction </summary>

1. *Die* - A "die" refers to a small, individual rectangular or square section of a silicon wafer. Each die contains a single integrated circuit (IC) or microchip. These dies are created through a series of complex processes, including photolithography, etching, and doping, on a single silicon wafer. After the manufacturing process is complete, the wafer is diced or cut along its edges to separate the individual dies. Each die can then be packaged as a discrete electronic component.
	
 2.*Core* - A "core" typically refers to a central processing unit (CPU) or a specialized processing unit within an integrated circuit (IC) or chip.
	
 3.*Macro* - A "macro" typically refers to a pre-designed and pre-verified functional block or module that can be integrated into a larger chip or system. Macros are used to simplify the chip design process, reduce development time, and ensure the reliability and performance of complex systems.<br>
	
 Below screenshot represents the structure of chip.<br>
	 <img width="600" alt="die" src="https://github.com/Sidv005/Samsung-PD-Training/blob/64b70d255620d6421e8e4a16056212b1c3de6d11/SamsungPD_training/day1-openlane/die.PNG"><br>
	
 4.*RISC V* - The RISC-V architecture is an open-standard instruction set architecture (ISA) based on the principles of Reduced Instruction Set Computing (RISC). It is designed to be a simple and modular architecture that can be used for a wide range of applications, from embedded systems to high-performance computing. 
	
 5.*EDA Tools* - EDA, or Electronic Design Automation, tools are software applications used by engineers and designers to design, analyze, and simulate electronic circuits and systems. These tools are essential for the development of integrated circuits (ICs), printed circuit boards (PCBs), and other electronic hardware. EDA tools help streamline the design process, improve design quality, and reduce time-to-market. 
	
 6.*PDK* -  PDK stands for "Process Design Kit." A Process Design Kit is a collection of files, libraries, data, and tools provided by semiconductor foundries or manufacturers to assist integrated circuit (IC) designers in developing chips that are compatible with a specific semiconductor manufacturing process. 
</details>

<details>
 <summary>Overview on RTL to GDSII </summary>

 Below image shows the RTL to GDS II flow.<br>
<img width="600" alt="rtlgds" src="https://github.com/Sidv005/Samsung-PD-Training/blob/5f141861a60562264f2686011b0c8476b6af483c/SamsungPD_training/day1-openlane/rtlgds.PNG"><br>

1. *Synthesis* - Synthesis is the pivotal phase in VLSI design where a high-level hardware description of a digital circuit, usually expressed in a hardware description language like VHDL or Verilog, is converted into a netlist that represents the logical and physical components constituting the actual integrated circuit. This transformation is essential for building the IC.

At the heart of this process are standard cells, which serve as the fundamental building blocks. These cells are meticulously designed with a regular layout and come with various representations, including electrical, HDL, and SPICE models. Additionally, standard cells offer abstract and detailed layout views. They hold a central role in the assembly of the final integrated circuit layout.

2. *Floor planning* - Floor planning in chip design is the initial stage of the physical design process where the layout and arrangement of different functional blocks and components on an integrated circuit (IC) are determined. This process involves defining the physical boundaries, locations, and rough sizes of various elements to optimize the chip's performance, power consumption, and manufacturability. Here are key aspects of floor planning in chip design:

- Block Placement: The primary objective of floor planning is to determine where each functional block or module of the IC will be placed on the silicon die. Careful placement is essential to minimize wire lengths, reduce signal delays, and achieve efficient power distribution.

- Signal Flow: Floor planning considers the flow of signals between blocks. Critical paths and signal paths with specific timing requirements are analyzed to ensure that the layout minimizes signal delays and meets performance goals.

- Power Distribution: The distribution of power and ground connections is a critical consideration in floor planning. Efficient power grid design is necessary to ensure that each block receives a stable and adequate power supply, minimizing voltage drops and power dissipation.

- Heat Dissipation: Effective floor planning takes into account thermal considerations. Placing power-hungry blocks near each other can lead to localized heating, which can affect chip reliability and performance. Floor planning should include provisions for heat dissipation, such as the placement of thermal vias and heat sinks.

- I/O Placement: The placement of input and output pads or pins is an essential part of floor planning. Ensuring that these connections are appropriately positioned and organized helps in achieving efficient I/O operation and ease of PCB integration.

- Hierarchical Organization: In complex IC designs, floor planning is often done hierarchically, with larger blocks representing major functions and smaller blocks representing subfunctions. This hierarchical organization helps manage complexity and simplifies the design process.

- Design Constraints: Various design constraints, such as area limitations, manufacturing rules, and design rules set by the foundry, must be considered during floor planning to ensure that the chip design remains manufacturable.

- Iterative Process: Floor planning is often an iterative process that may require adjustments and refinements to meet design objectives. Designers may use floor planning tools and simulations to assess and optimize the placement of blocks.

- Area Optimization: One of the key goals of floor planning is to optimize the use of available silicon area. Efficient use of space is crucial for minimizing manufacturing costs and maximizing chip performance.

- Documentation: The outcome of the floor planning process is typically documented in a floor plan diagram or document that provides a visual representation of the chip's physical layout and placement of functional blocks.

3. *Placement* - Placement constitutes a pivotal phase in the physical design of integrated circuits (ICs). This critical step entails the strategic positioning of each logical cell, particularly standard cells, within the chip's silicon area. Proficient placement profoundly influences key factors, including performance, power efficiency, and the effective utilization of chip space. The primary goal of placement is to organize standard cells in a manner that minimizes the cumulative length of connecting wires (known as wirelength), optimizes the utilization of the chip's area, and satisfies a range of design constraints, encompassing timing, power requirements, and manufacturability.

4. *CTS* - CTS, or Clock Tree Synthesis, is a pivotal phase in the physical design of integrated circuits (ICs). This process is dedicated to creating and refining the network responsible for distributing clock signals within the chip. The primary aim of CTS is to ensure the efficient and dependable delivery of clock signals to all flip-flops and sequential elements, thus minimizing variations in signal arrival times (known as clock skew) and adhering to specified timing requirements. In essence, CTS plays a vital role in VLSI design, significantly impacting overall performance, power efficiency, and the robustness of integrated circuits. It leverages advanced algorithms and tools to automate and enhance the CTS procedure, especially for intricate and high-performance ICs.

5. *Routing* - Routing is a foundational process in VLSI (Very Large Scale Integration) design, and it constitutes a vital stage in the physical design of integrated circuits (ICs). This essential step revolves around establishing the physical pathways, typically metal traces or wires, that connect different components and logic elements on the chip. The primary objective is to ensure the efficient and constraint-compliant routing of data signals, control signals, and power throughout the IC. Routing's significance lies in its profound impact on the IC's performance, power efficiency, and overall operational capabilities.

6. *Sign off* - "Sign-off" is the last phase in the design process just before sending an integrated circuit (IC) design for manufacturing. During sign-off, a thorough series of assessments, examinations, and validations takes place to confirm that the IC design complies with all required criteria, constraints, and specifications. This step is crucial because overlooking design errors or issues at this stage can lead to expensive and time-consuming complications either during manufacturing or after the ICs are in use.

7. *Physical verification* - Physical verification in VLSI (Very Large Scale Integration) refers to the process of systematically inspecting and validating the physical layout of an integrated circuit (IC) design to ensure that it adheres to design rules, manufacturing constraints, and industry standards. The goal of physical verification is to identify and rectify any potential design errors or violations that could lead to issues during fabrication, assembly, or operation of the IC. Here are key aspects of physical verification in VLSI:

- Design Rule Checking (DRC): DRC is a fundamental component of physical verification. It involves the examination of the IC layout to ensure that it complies with specific manufacturing rules and guidelines set by the semiconductor foundry. These rules encompass aspects like minimum feature sizes, spacing between components, metal layer stackup, and more.

- LVS (Layout versus Schematic) Verification: LVS verification compares the physical layout of the IC with its logical representation (schematic) to confirm that there are no inconsistencies or mismatches between the two. It ensures that the connections and components on the layout correspond correctly to the intended circuit functionality.

- Electrical Rule Checking (ERC): ERC focuses on checking electrical connectivity and functionality. It identifies issues such as floating nodes, unconnected pins, and electrical shorts or opens that can impact circuit performance or reliability.

- Antenna Rule Check: Antenna effect verification is essential for preventing charge buildup in MOS (Metal-Oxide-Semiconductor) devices during the fabrication process. It ensures that sufficient charge-neutralization mechanisms are in place to protect against damage.

- Differential Stress Analysis: This analysis assesses the physical stress distribution in the IC to identify potential areas of mechanical stress that could impact the device's long-term reliability.

- Parasitic Extraction: Parasitic extraction involves extracting parasitic elements, such as capacitances and resistances, from the IC layout. These parasitic elements can affect signal timing and power consumption and must be accurately accounted for in circuit simulations.

- Manufacturability Checks: Physical verification also encompasses manufacturability checks to ensure that the design can be successfully fabricated with the selected process technology. It considers aspects like lithography, mask generation, and process compatibility.

- Compliance with Industry Standards: IC designers often need to ensure that their designs comply with industry standards, such as those related to electromagnetic interference (EMI) and electrostatic discharge (ESD) protection.

- Iterative Process: Physical verification is an iterative process, and multiple iterations may be necessary to resolve design issues and achieve a clean and error-free layout.

- Documentation and Reporting: The results of physical verification are typically documented, and reports are generated to provide feedback to the design team. Any identified issues or violations must be addressed before the design can proceed to the manufacturing phase.
</details>

<details>
 <summary>Introduction to OpenLANE </summary>

OpenLane is an open-source, fully automated digital ASIC (Application-Specific Integrated Circuit) design flow toolchain. It provides a comprehensive set of tools and scripts that facilitate the design, implementation, and verification of custom digital integrated circuits, ranging from small-scale digital logic designs to complex, large-scale ICs. OpenLane is primarily used for digital IC design in VLSI (Very Large Scale Integration) and is especially valuable for academic, research, and industry projects where creating custom chips is required.

Here is an introduction to the key features and components of OpenLane:

- Fully Automated Flow: OpenLane offers an end-to-end, fully automated design flow for digital ICs. It streamlines the entire process, from RTL (Register Transfer Level) design to GDSII (Graphic Data System II) tape-out, which is the final file format for semiconductor manufacturing.

- Uses OpenROAD and Skywater PDK: OpenLane leverages the OpenROAD project's infrastructure and uses the Skywater 130nm process design kit (PDK) as its reference process. This PDK includes libraries, technology files, and manufacturing rules necessary for IC design in this technology node.

- RTL to GDSII: The toolchain supports RTL synthesis, placement, clock tree synthesis, routing, and other steps required to convert high-level RTL descriptions of a design into a manufacturable GDSII file.

- Advanced Node Support: OpenLane initially focused on the Skywater 130nm process, but it has expanded to support multiple semiconductor process nodes, allowing designers to target different manufacturing technologies.

- Customization and Configuration: OpenLane is highly configurable, allowing designers to customize various aspects of the design flow, such as design constraints, optimization settings, and tool options to meet specific project requirements.

- Design Exploration: OpenLane supports design space exploration, allowing designers to explore different design trade-offs and optimizations to achieve the desired balance between performance, area, and power consumption.

- Built-in Testing: The toolchain includes built-in testing and verification capabilities to ensure that the resulting IC design meets functional and performance specifications.

- Community and Collaboration: OpenLane has a growing community of users and contributors who actively develop and improve the toolchain. This collaborative approach fosters innovation and knowledge sharing.

- Open Source: As an open-source project, OpenLane is freely available to anyone, and its source code can be modified and extended to suit specific needs.

OpenLane simplifies the complex process of digital IC design, making it more accessible to a broader range of users while promoting transparency and collaboration within the VLSI community. It has gained popularity as a versatile tool for both educational and practical applications in the field of integrated circuit design.

**Overview on OpenLANE ASIC Flow**

The OpenLane ASIC flow is a complete, open-source digital ASIC design flow that automates the process of designing custom integrated circuits. It employs various open-source tools and scripts to guide the design through multiple stages. Here is an overview of the OpenLane ASIC flow with the names of the key tools used at each step:

- RTL Design:
Tool: Your choice of hardware description language (e.g., Verilog, VHDL)

- Synthesis:
Tool: Yosys

- DFT:
  Tool: Fault
  
- Floorplanning:
Tool: Magic

-Placement:
Tool: RePLace

- Clock Tree Synthesis (CTS):
Tool: TritonCTS

- Routing:
Global Routing Tool: FastRoute
Detailed Routing Tool: TritonRoute

- Static Timing Analysis (STA):
Tool: OpenSTA

- Design Rule Checking (DRC):
Tool: Magic

- Layout vs. Schematic (LVS) Verification:
Tool: Netgen (for LVS), Magic (for DRC)

- Parasitic Extraction:
Tool: Qflow

- Final Tape-out (GDSII Generation):
Tool: Magic

- Manufacturing and Testing:
The GDSII file generated in the previous step is used by a semiconductor foundry for manufacturing. Testing and quality assurance are carried out during and after manufacturing.

The OpenLane ASIC flow is highly configurable, allowing users to customize various aspects of the design process to meet their specific requirements. It is designed to support both educational and research purposes, as well as practical ASIC design projects. 
</details>

<details>
 <summary>LABS </summary>

Below screenshot shows the files present in openLANE directory like open_pdks and sky130A.<br>
<img width="600" alt="ss1" src="https://github.com/Sidv005/Samsung-PD-Training/blob/ee2c8611b81d5a848e131a7d011730d645edb74b/SamsungPD_training/day1-openlane/ss1.png"><br>

Below screenshot shows the .lef and .tlech files.<br>
<img width="600" alt="ss2" src="https://github.com/Sidv005/Samsung-PD-Training/blob/ee2c8611b81d5a848e131a7d011730d645edb74b/SamsungPD_training/day1-openlane/ss2.png"><br>

Below screenshot shows how the OpenLANE is invoked.<br>
<img width="600" alt="openlane(invoke)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/ee2c8611b81d5a848e131a7d011730d645edb74b/SamsungPD_training/day1-openlane/openlane(invoke).png"><br>

Below screenshot shows the config.tcl script.<br>
<img width="600" alt="openlane(config.tcl)1" src="https://github.com/Sidv005/Samsung-PD-Training/blob/ee2c8611b81d5a848e131a7d011730d645edb74b/SamsungPD_training/day1-openlane/openlane(config.tcl)1.png"><br>

Below screenshot shows the execution of prep -design. Here config.tcl is sourced and merging of lef and tech lef file is occuring.<br>
<img width="600" alt="prep-design" src="https://github.com/Sidv005/Samsung-PD-Training/blob/ee2c8611b81d5a848e131a7d011730d645edb74b/SamsungPD_training/day1-openlane/prep-design.png"><br>

Below image shows the merged.lef script where we observe the layers ,vias and macros information.<br>
<img width="600" alt="merged_lef" src="https://github.com/Sidv005/Samsung-PD-Training/blob/ee2c8611b81d5a848e131a7d011730d645edb74b/SamsungPD_training/day1-openlane/merged_lef.png"><br>

Below screenshot shows the successfull runing of synthesis command i.e *run_synthesis*.<br>
<img width="600" alt="run_syn" src="https://github.com/Sidv005/Samsung-PD-Training/blob/ee2c8611b81d5a848e131a7d011730d645edb74b/SamsungPD_training/day1-openlane/run_syn.png"><br>

Below screenshot shows the timing report after synthesis which is generated by OpenSTA tool.<br>
<img width="600" alt="timing_rpt" src="https://github.com/Sidv005/Samsung-PD-Training/blob/ee2c8611b81d5a848e131a7d011730d645edb74b/SamsungPD_training/day1-openlane/timing_rpt.png"><br>

Below screenshot shows the report after synthesis.<br> 
<img width="600" alt="flop_ratio" src="https://github.com/Sidv005/Samsung-PD-Training/blob/ee2c8611b81d5a848e131a7d011730d645edb74b/SamsungPD_training/day1-openlane/flop_ratio.png"><br>

Here we can observe that <br>
no. of cells = 14876 <br>
no. of flops = 1613.<br>

The Flop ratio can be calculated by dividing no. of flops with no. of cells which equals to 0.10842.

</details>

## Day16 - Good Floorplan vs Bad Floorplan and Introduction to Library cells
<details>
 <summary>Chip Floorplanning Considerations </summary>
 
1. *Utilization Factor* - The utilization factor in floorplanning measures how efficiently the available chip area is occupied by functional blocks or logic elements in an integrated circuit design. Designers aim to maximize this factor while considering various constraints and trade-offs to achieve a well-balanced and high-quality chip layout. It is ratio of area occupied by the netlist and Total core area.
Practically 50% - 60% is core utilization. 

2. *Aspect Ratio* - The aspect ratio in floor planning defines the physical shape of an integrated circuit layout by specifying the ratio of Height of core and width of core. It is a critical parameter that influences chip design and is considered alongside various design requirements and constraints to achieve optimal results.
- If Aspect Ratio is 1 that signifies square chip other than 1 signifies rectangular chip.

3. *Preplaced cells* - Preplaced cells refer to a set of specific functional blocks or standard cells that are manually or automatically placed at predetermined locations within the chip layout. These cells are typically strategically positioned before the automated placement and routing processes are executed for the rest of the design.

4. *Decoupling Capacitors* - Decoupling capacitors are an integral part of chip design, providing a critical role in maintaining electrical stability and performance. Their proper selection, placement, and configuration are essential for achieving reliable and noise-free operation in integrated circuits. In complex chips, multiple decoupling capacitors of varying capacitance values are often used in parallel. This combination helps filter noise across a broader frequency spectrum.

5. *Tap cells* - Tap cells are a fundamental component of IC design, especially in CMOS technology, as they serve to prevent latch-up by isolating transistor regions and providing a safe path for unwanted substrate currents to flow. Their proper placement and configuration are critical to ensure the reliable and stable operation of integrated circuits.

6. *Power planning* - Power planning is a critical aspect of the ASIC (Application-Specific Integrated Circuit) design flow, focused on managing and distributing power throughout the chip to ensure reliable and efficient operation. Proper power planning is essential for controlling power consumption, minimizing voltage drops, and preventing potential issues such as overheating and electromigration.
    - Installing Decap to every element is not feasible so a Power supply is needed. Ground Bounce and Voltage droop may occur due to signal integrity issues.

7. *Ground bounce* -  Ground bounce is a transient voltage increase in the ground signal within an integrated circuit, primarily caused by the inductance and resistance of ground connections. It can lead to signal integrity issues and incorrect readings in digital circuits. Proper chip design techniques, including decoupling capacitors and careful power distribution network design, are essential to mitigate and control ground bounce.

8. *Voltage droop* - voltage droop is a temporary reduction in supply voltage that can occur due to rapid changes in current demand or parasitic elements in the power distribution network. It can have detrimental effects on chip operation and performance, so designers employ various techniques to mitigate and prevent voltage droop and ensure reliable and stable operation.

9. *Pin Placement* - Pin placement, also known as I/O (Input/Output) placement, is a critical step in the physical design process of creating integrated circuits (ICs). It involves determining the locations and assignments of input and output pins on the chip's package or footprint. Proper pin placement is crucial for ensuring signal integrity, ease of manufacturing, and compatibility with external interfaces. Designers use various software tools and simulations to aid in pin placement and signal routing.
    - It is a crucial step in the physical design process and requires careful consideration of signal integrity, I/O requirements, external interfaces, power distribution, thermal management, manufacturability, and compliance with standards. Proper pin placement is essential for the successful operation and performance of the integrated circuit.

Below screenshot shows the Pin Placement view.<br>
<img width="600" alt="pins" src="https://github.com/Sidv005/Samsung-PD-Training/blob/2d060ce5ce81b4cb85aa324fff33b40b47b55841/SamsungPD_training/day2_openlane/pins.PNG"><br>

- These pins are placed in random order.
- Clock pins are larger because they need to send the signals to all flip flops.
</details>

<details>
 <summary>Labs on Floorplan using Openlane </summary>
1. Below image shows the readme file prensent in openlane configuration. Here variables or switches need to be observed for every step.<br> 
<img width="600" alt="readme" src="https://github.com/Sidv005/Samsung-PD-Training/blob/4df9a2a4524c203e635bfd9a264ed4ccaee39fbf/SamsungPD_training/day2_openlane/readme.png"><br>
	
2. Below image shows the floorplan.tcl file which is prensent in openlane configuration. Here default values are set like FP_IO_MODE, VMETAL, HMETAL etc..<br> 
<img width="600" alt="fp_tcl" src="https://github.com/Sidv005/Samsung-PD-Training/blob/4df9a2a4524c203e635bfd9a264ed4ccaee39fbf/SamsungPD_training/day2_openlane/fp_tcl.png"><br>

3. Following screenshot displays the **run_floorplan**. Here observe that .def file is created after succesfull floorplan. <br>
<img width="600" alt="run_fp" src="https://github.com/Sidv005/Samsung-PD-Training/blob/4df9a2a4524c203e635bfd9a264ed4ccaee39fbf/SamsungPD_training/day2_openlane/run_fp.png"><br>

4. Following screenshot displays the config.tcl generated after floorplan. Here observe following parameters after succesfull floorplan.
   - HMETAL = 4
   - VMETAL = 3
   - CORE UTILIZATION = 35
   - ASPECT RATIO = 1 <br>
<img width="600" alt="fp_config_hmetal" src="https://github.com/Sidv005/Samsung-PD-Training/blob/4df9a2a4524c203e635bfd9a264ed4ccaee39fbf/SamsungPD_training/day2_openlane/fp_config_hmetal.png"><br>

5. Following screenshot displays the .def file generated where Die area needs to be observed which can be converted to micro meters.<br> 
<img width="600" alt="fp_picorv_def(area)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/4df9a2a4524c203e635bfd9a264ed4ccaee39fbf/SamsungPD_training/day2_openlane/fp_picorv_def(area).png"><br>

6. Actual Layout of Floorplan can viewd using Magic Tool. Below image shows the layout obtained after floorplan.<br>
<img width="600" alt="fp_layout" src="https://github.com/Sidv005/Samsung-PD-Training/blob/4df9a2a4524c203e635bfd9a264ed4ccaee39fbf/SamsungPD_training/day2_openlane/fp_layout.png"><br>

7. Below image shows the tkcon 2.3 Main Window where metal layer can be observed. Other cells like DECAP and TAP cells can also be observed.<br>
<img width="600" alt="fp_layout_tckon" src="https://github.com/Sidv005/Samsung-PD-Training/blob/4df9a2a4524c203e635bfd9a264ed4ccaee39fbf/SamsungPD_training/day2_openlane/fp_layout_tckon.png"><br>

</details>

<details>
 <summary>Netlist Binding and intial place design </summary>

1. **Netlist binding** is the process of associating or "binding" logical cells from a high-level or gate-level representation (the logical netlist) of the design to physical locations on the chip. It essentially maps the functional blocks or gates of the design to specific locations on the chip's layout.
- Libraries have different flavors of cells of varying Height and width. According to applications netlist is binded with those particular cells.
-  Netlist binding takes into account timing constraints, ensuring that cells are placed to meet required signal propagation delays and clock requirements.
- An effective netlist binding strategy considers the routing requirements, aiming to minimize wirelengths and congestion while allowing for efficient interconnections between cells.

2. **Initial placement** is the process of positioning the logical cells or blocks on the chip's floorplan, considering their netlist bindings. It sets the initial positions of cells, providing a starting point for subsequent optimization steps like detailed placement and routing.
- Initial placement considers timing constraints and may optimize cell positions to meet critical timing requirements.
- Initial placement is often an iterative process that may require feedback from subsequent steps in the design flow. Designers may refine the placement based on feedback from routing and timing analysis.
- Automated placement tools are commonly used to perform initial placement based on design constraints and objectives.
</details>

<details>
 <summary>Final placement optimization </summary>

- Consider 4 circuits of different colors like orange, yellow, blue, green containing FF1 - 1 - 2 - FF2 cells with different Data in and out pins.
- Different inputs pins are Din1, Din2, Din3, Din4.
- Different output pins are Dout1, Dout2, Dout3, Dout4.
- These are initially placed in the following manner as shown in figure.<br> 
<img width="700" alt="ini_place" src="https://github.com/Sidv005/Samsung-PD-Training/blob/8bfdc1f95926ab565a2000317be796b778cb987d/SamsungPD_training/day2_openlane/ini_place.PNG"><br>

- But here it requires repeators to avoid signal integrity issues whle propogating the data through the path.
- Hence Buffers are used in between the paths to mitigate the issues.
- Below figure shows the optimized placement.<br>
<img width="700" alt="final_place" src="https://github.com/Sidv005/Samsung-PD-Training/blob/8841b8b03e9e0e49635d432c8ffa36e086c33d00/SamsungPD_training/day2_openlane/final_place.PNG"><br>
</details>

<details>
 <summary> Labs on Placement </summary>
	
- Below screenshot shows the execution of **run_placement** and displays the successfull placement of picorv32a design.<br>
<img width="600" alt="run_place" src="https://github.com/Sidv005/Samsung-PD-Training/blob/8841b8b03e9e0e49635d432c8ffa36e086c33d00/SamsungPD_training/day2_openlane/run_place.png"><br>

From above figure we can see that picorv32a.placement.def file is generated.

- Actual layout after placment process is seen in below figure.<br>
<img width="600" alt="place_layout" src="https://github.com/Sidv005/Samsung-PD-Training/blob/8841b8b03e9e0e49635d432c8ffa36e086c33d00/SamsungPD_training/day2_openlane/place_layout.png"><br>

- In Placement step all standard cells are placed after zooming in we can observe those standard cells placed in rows.
  
- Below figure shows the layout view after zooming in to display the standard cells.<br>
<img width="600" alt="place_layout2" src="https://github.com/Sidv005/Samsung-PD-Training/blob/8841b8b03e9e0e49635d432c8ffa36e086c33d00/SamsungPD_training/day2_openlane/place_layout2.png"><br>
</details>

## Day-17 Standard Cell Characterizations ##

<details>
 <summary>IO placer revised </summary>
 You can adjust the alignment of the Input/Output (I/O) pins by modifying the value of the FP_IO_MODE parameter. By default, this parameter is set to 1, but you can change it using the following command:

 ```ruby
set ::env(FP_IO_MODE) 2
```
After changing the mode following image is obtained.<br>
<img width="600" alt="fp_pin_uneven2" src="https://github.com/Sidv005/Samsung-PD-Training/blob/befa507f9dfa9062514315167655ed907184f0bf/SamsungPD_training/day3_openlane/fp_pin_uneven2.png"><br>

Below image is the zoomed version of above image.<br>
<img width="600" alt="fp_pin_uneven_zoom" src="https://github.com/Sidv005/Samsung-PD-Training/blob/befa507f9dfa9062514315167655ed907184f0bf/SamsungPD_training/day3_openlane/fp_pin_uneven_zoom.png"><br>

Here you can observe that pins are place in uneven order.
</details>

<details>
 <summary>Spice Simulation lab for CMOS Inverter</summary>
	
 1. The initial step involves generating a SPICE Deck file that encompasses essential details, such as the netlist's connectivity information, specified input sources, and designated points for observing outputs. In the creation of this SPICE Deck, the process entails defining the interconnections among components, specifying component values, as well as recognizing and labeling nodes accordingly.
	
 2. A CMOS inverter is a digital logic gate that takes an input signal and produces an output signal that is the logical complement (opposite) of the input. In other words, when the input is high (1), the output is low (0), and when the input is low (0), the output is high (1).
  
 3. A CMOS inverter is constructed using complementary pairs of both NMOS (n-channel metal-oxide-semiconductor) and PMOS (p-channel metal-oxide-semiconductor) transistors. When one transistor is on (conducting), the other is off (non-conducting), allowing for low-power consumption and high noise immunity.
 
 4. A node is identified when a component is positioned between two nodes.

- The SPICE deck for CMOS inverter is as follows.

```ruby
M1 out in vdd vdd pmos W=0.375u L=0.25u
M2 out in 0 0 nmos W=0.375u W=0.25u
cload out 0 10f
Vdd vdd 0 2.5
Vin in 0 2.5
** Simulation Commands**
.op
.dc Vin 0 2.5 0.05
** .include tsmc_025um_model.mod **
.LIB "tsmc_025um_model.mod" CMOS_MODELS
.end
```

1. Component M1 represents a PMOS transistor with its drain connected to the OUT node, its gate linked to the IN node, and its substrate and source connected to VDD. M1 also features a specified width-to-length (W/L) ratio.
2. Component M2 represents an NMOS transistor with its drain linked to the OUT node, its gate connected to the IN node, and its substrate and source tied to the ground (0V). M2 also includes a defined W/L ratio.
3. The load capacitance, with a value of 10fF, is connected between the OUT node and ground. Likewise, the supply voltages, set at 2.5V, are connected between the ground and their respective nodes.
4. The Simulation command signifies the incremental variation of the gate voltage, ranging from 0V to 2.5V, in steps of 0.05V. This procedure is executed to observe and record the output characteristics concerning changes in the input voltage. The model file should be structured as follows, providing a comprehensive description of both NMOS and PMOS transistors, including their respective dimensions (length and width).

The layout of the CMOS inverter is as follows:<br>
<img width="600" alt="layout_inv" src="https://github.com/Sidv005/Samsung-PD-Training/blob/befa507f9dfa9062514315167655ed907184f0bf/SamsungPD_training/day3_openlane/layout_inv.png"><br>

Below image shows that poly is connected to PMOS and NMOS.<br>
<img width="600" alt="layout_inv" src="https://github.com/Sidv005/Samsung-PD-Training/blob/befa507f9dfa9062514315167655ed907184f0bf/SamsungPD_training/day3_openlane/layout_tckon(n%2Cp).png"><br>

Following commands are runned in tckon Main window.
```ruby
extract all
ext2spice cthresh 0 rthresh 0
ext2spice
```
The spice netlist generated as shown below.<br>
<img width="600" alt="spice_gen" src="https://github.com/Sidv005/Samsung-PD-Training/blob/befa507f9dfa9062514315167655ed907184f0bf/SamsungPD_training/day3_openlane/spice_gen.png"><br>
</details>

<details>
 <summary>16 Mask CMOS Fabricaion</summary>

The manufacturing process involves several key steps:

1.Substrate Preparation: Commences with a silicon wafer as the initial material, which undergoes rigorous cleaning and pre-processing to prepare it for further stages.

2.Gate Oxide Formation (Mask 1): A thin layer of silicon dioxide (SiO2) is either grown or deposited onto the silicon wafer. This layer functions as the gate dielectric.

3.Polysilicon Gate Formation (Mask 2): Polysilicon is deposited and precisely patterned to create gate electrodes for both NMOS and PMOS transistors.

4.N-Well and P-Well Formation (Mask 3): The creation of regions for NMOS and PMOS transistors involves the use of n-type and p-type ion implantation processes.

5.Source and Drain Formation (Masks 4 and 5): Ion implantation, followed by annealing processes, is employed to define the source and drain regions of the transistors.

6.Gate Spacer and Silicidation (Masks 6 and 7): Insulating spacers are introduced around the gate structures, and metal silicide is formed on the source and drain regions to reduce contact resistance.

7.Interlayer Dielectric (ILD) Deposition (Mask 8): A layer of insulating material, typically silicon dioxide, is deposited and planarized to create a level surface for metal interconnections.

8.Contact and Via Formation (Masks 9 and 10): Etching processes create contact holes through the ILD, facilitating connections between metal interconnects and the underlying transistor nodes.

9.Metal Layer 1 (Mask 11): The formation of metal lines and interconnects allows for connections between different parts of the circuit.

10.Intermetal Dielectric (IMD) Deposition (Mask 12): Another insulating layer is deposited to provide separation between metal layers and isolation.

11.Metal Layer 2 (Mask 13): Additional layers of metal interconnects may be added as required.

13.Passivation Layer (Mask 14): A protective layer is deposited to shield the underlying layers and offer electrical insulation.

14.Pad Opening (Mask 15): Openings are created in the passivation layer to enable wire bonding or solder bump connections.

15.Testing and Packaging (Mask 16): Chips undergo rigorous testing for functionality and performance, followed by packaging to prepare them for their final use.

This comprehensive process forms the foundation of semiconductor device manufacturing, allowing for the creation of integrated circuits with intricate electronic functionalities.

***CMOS Inverter layout in Magic***

- When we select nmos and pmos box in Magic and run *what* command in tckon window we obtain below image.<br>
<img width="600" alt="layout_tckon(n%2Cp)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/befa507f9dfa9062514315167655ed907184f0bf/SamsungPD_training/day3_openlane/layout_tckon(n%2Cp).png"><br>

- The connection of Y to both the drain terminals of the PMOS and NMOS transistors is depicted as illustrated in the figure.<br>
<img width="600" alt="layout_Y_con" src="https://github.com/Sidv005/Samsung-PD-Training/blob/befa507f9dfa9062514315167655ed907184f0bf/SamsungPD_training/day3_openlane/layout_Y_con.png"><br>
- The connections of the PMOS source and NMOS source are established as follows:<br>
<img width="600" alt="layout_NMOS_source" src="https://github.com/Sidv005/Samsung-PD-Training/blob/befa507f9dfa9062514315167655ed907184f0bf/SamsungPD_training/day3_openlane/layout_NMOS_source.png"><br>
<img width="600" alt="layout_PMOS_source" src="https://github.com/Sidv005/Samsung-PD-Training/blob/befa507f9dfa9062514315167655ed907184f0bf/SamsungPD_training/day3_openlane/layout_PMOS_source.png"><br>

- When we delete some layers we get drc errors same is illustrated in below image.<br>
<img width="600" alt="layout_Drc" src="https://github.com/Sidv005/Samsung-PD-Training/blob/befa507f9dfa9062514315167655ed907184f0bf/SamsungPD_training/day3_openlane/layout_Drc.png"><br>

- Below image is obtained after removing Drc Errors.<br>
<img width="600" alt="layout_inv" src="https://github.com/Sidv005/Samsung-PD-Training/blob/befa507f9dfa9062514315167655ed907184f0bf/SamsungPD_training/day3_openlane/layout_inv.png"><br>
</details>

<details>
 <summary>Labs on DRC</summary>
	
- Initially, it is necessary to duplicate the 'open_pdks.git' repository from RTimothyEdwards. Now all the magic files is with us. We will look for mtal3.mag. So metal3.mag file now with us.

- *cif see VIA2* command is runned in tckon window to obtain metal 3 contacts.
- When we see the layout of metal3.mag in Magic it is the same as shown below.<br>
<img width="600" alt="layout_metal3" src="https://github.com/Sidv005/Samsung-PD-Training/blob/3d749d7d212dcf9f2c67be43a5160b9c3384e187/SamsungPD_training/day3_openlane/layout_metal3.png"><br>

- Now width and height of the box is shown in below image which determine distance between the metal contact and metal layer boundary. <br>
<img width="600" alt="layout_metal3_tckon" src="https://github.com/Sidv005/Samsung-PD-Training/blob/3d749d7d212dcf9f2c67be43a5160b9c3384e187/SamsungPD_training/day3_openlane/layout_metal3_tckon.png"><br>

- Now poly.mag is loaded in Magic Following image shows the tckon window.<br>
<img width="600" alt="layout_poly_tckon" src="https://github.com/Sidv005/Samsung-PD-Training/blob/3d749d7d212dcf9f2c67be43a5160b9c3384e187/SamsungPD_training/day3_openlane/layout_poly_tckon.png"><br>

- Below image of tckon window shows the width box in poly.<br>
<img width="600" alt="layout_poly_tckon_box" src="https://github.com/Sidv005/Samsung-PD-Training/blob/3d749d7d212dcf9f2c67be43a5160b9c3384e187/SamsungPD_training/day3_openlane/layout_poly_tckon_box.png"><br>

- Now sky130A.tech file is edited by adding ***allpolynonres*** in poly.9. After editting we load the tech file and check drc using *drc check* in tckon window. This is shown in below image.<br> 
<img width="600" alt="tech_edit1_layout" src="https://github.com/Sidv005/Samsung-PD-Training/blob/3d749d7d212dcf9f2c67be43a5160b9c3384e187/SamsungPD_training/day3_openlane/tech_edit1_layout.png"><br>
- Here we can obsevre that no drc error is occuring. Hence we succesfully fixed poly.9 error. 
</details>


## Day-18 Pre timing Analysis and Importance of good clock tree ##

<details>
 <summary>Steps to convert Grid into track info</summary>
	
 - Library Exchange Format (LEF) is a standard format used in the field of Very Large Scale Integration (VLSI) design. It is primarily used to describe the physical properties and characteristics of standard cells, macros, and other elements in a semiconductor library. 
- LEF files provide crucial information that is essential for the physical design and manufacturing processes of integrated circuits. LEF files are typically used in conjunction with Design Exchange Format (DEF), which describes the logical design of the circuit.
- LEF files describe the characteristics of individual cells or components within a semiconductor library.
- Here we are converting .mag files of inverter to .lef .

The track info detail is as follows:<br>
<img width="600" alt="tracks_info" src="https://github.com/Sidv005/Samsung-PD-Training/blob/782a7481f9e71a461b90bd38d4e5c4224b2a80e6/SamsungPD_training/day4_final/tracks_info.png"><br>
- Now grid is set as hsown in below figure.<br>
<img width="600" alt="tckon_grid" src="https://github.com/Sidv005/Samsung-PD-Training/blob/782a7481f9e71a461b90bd38d4e5c4224b2a80e6/SamsungPD_training/day4_final/tckon_grid.png"><br>

1. Rule 1 : Input and output port should lie on the intersection of horizontal and vertical track

2. Rule 2 : The width of a standard cell should be odd multiple of the horizontal track pitch<br>
<img width="600" alt="grid_check" src="https://github.com/Sidv005/Samsung-PD-Training/blob/0894a12dbc3fcd72cd41a580a9cba75abfff0717/SamsungPD_training/day4_final/grid_check.PNG"><br>

- Here we can observe that the width equals to 3 times the horizontal track pitch.
</details>

<details>
 <summary>Steps to convert magic layout to lef</summary>

- Save the layout with your name For e.g. sky130_siddhant

Then use ***lef_write*** command this creates a .lef file

Following image shows the inclusion of the sky130_siddhant.lef file in src.<br>
<img width="600" alt="src_content" src="https://github.com/Sidv005/Samsung-PD-Training/blob/0894a12dbc3fcd72cd41a580a9cba75abfff0717/SamsungPD_training/day4_final/src_content.png"><br>

The contents of .lef file shown in below image.<br>
<img width="600" alt="siddhant.lef" src="https://github.com/Sidv005/Samsung-PD-Training/blob/0894a12dbc3fcd72cd41a580a9cba75abfff0717/SamsungPD_training/day4_final/siddhant.lef.png"><br>

</details>

<details>
 <summary>Introduction to timing libs and steps to include lef cell</summary>

```ruby
cd ~/Desktop/work/tools/openlane_working_dir/openlane/vsdstdcelldesign
cp sky130_siddhant.lef ~/Desktop/work/tools/openlane_working_dir/openlane/designs/picorv32a/src
cd ~/Desktop/work/tools/openlane_working_dir/openlane/vsdstdcelldesign/libs
cp sky130_fd_sc_hd__* ~/Desktop/work/tools/openlane_working_dir/openlane/designs/picorv32a/src
cd ~/Desktop/work/tools/openlane_working_dir/openlane/designs/picorv32a/
vim config.tcl
```
Below screenshot displays the modified config.tcl file.<br>
<img width="600" alt="config" src="https://github.com/Sidv005/Samsung-PD-Training/blob/8b203812883cf396508a7b9c7b3c8d05e47c5eb5/SamsungPD_training/day4_final/config.PNG"><br>

Following image demonstrates how the .lef file is added before synthesizing.<br>
<img width="600" alt="siddhant.lef_added" src="https://github.com/Sidv005/Samsung-PD-Training/blob/8b203812883cf396508a7b9c7b3c8d05e47c5eb5/SamsungPD_training/day4_final/siddhant.lef_added.png"><br>

Following image demonstrates how the custom cell is merged into the design during synthesis.<br>
<img width="600" alt="siddhantinv_mergerd" src="https://github.com/Sidv005/Samsung-PD-Training/blob/8b203812883cf396508a7b9c7b3c8d05e47c5eb5/SamsungPD_training/day4_final/siddhantinv_mergerd.png"><br>

- We can observe that the cell of our name is getting used.
</details>

<details>
 <summary>Introduction to Delay Table</summary>

- Clock gating is a power-saving technique in digital circuit design. It involves using control logic to disable the clock signal to specific circuit blocks when they are not in use. This reduces dynamic power consumption, heat generation, and can extend battery life in low-power devices. The example of clock gating can be seen in the below image.<br>
<img width="600" alt="pic1_gating" src="https://github.com/Sidv005/Samsung-PD-Training/blob/02ddba812831bd12ca3271a69608cf8c5ec1085f/SamsungPD_training/day4_final/pic1_gating.PNG"><br>

- For each level of buffering, we should have an identical buffer being used, and each node should be driving the same node.

- Keep in mind that the load at the output will be varying, and since the load of one buffer is varying, the input transition of the following buffer will also vary.<br>
<img width="600" alt="pic2_gating" src="https://github.com/Sidv005/Samsung-PD-Training/blob/02ddba812831bd12ca3271a69608cf8c5ec1085f/SamsungPD_training/day4_final/pic2_gating.PNG"><br>

The example of delay table is as follows:<br>
<img width="600" alt="pic3" src="https://github.com/Sidv005/Samsung-PD-Training/blob/02ddba812831bd12ca3271a69608cf8c5ec1085f/SamsungPD_training/day4_final/pic3.PNG"><br>

- Each type of cell will be having its own individual delay table, as the internal pmos and nmos width/length ratio gets varied, the resistance changes, then RC constant gets varied as well, meaning the delay of each cell gets varied.
- The values of delay which are not available in the table are extrapolated based on the given data.
- If the Starting delay is 40 ps with C load as 50 pF the value will be between x9 and x10. As shown in the figure<br>

<img width="600" alt="pic4_gating" src="https://github.com/Sidv005/Samsung-PD-Training/blob/02ddba812831bd12ca3271a69608cf8c5ec1085f/SamsungPD_training/day4_final/pic4_gating.PNG"><br>
The observations of the delay table are as shown in the figure<br>
<img width="600" alt="pic5" src="https://github.com/Sidv005/Samsung-PD-Training/blob/02ddba812831bd12ca3271a69608cf8c5ec1085f/SamsungPD_training/day4_final/pic5.PNG"><br>
</details>

<details>
 <summary>Steps to configure synthesis settings to fix slack and include vsdinv</summary>
	
The various configuration of Synth are as follows

1. SYNTH_STRATEGY: control the area and timing
2. SYNTH_SIZING: control in cell sizing instead of buffering
3. SYNTH_BUFFERING: control if we want to buffer high fanout net
4. SYNTH_DRIVING_CELL: ensure more drive strength cell to drive input

In openlane
```ruby
echo $::env(SYNTH_STRATEGY)
set ::env(SYNTH_STRATEGY) "DELAY 0"
echo $::env(SYNTH_STRATEGY)
echo $::env(SYNTH_BUFFERING)
echo $::env(SYNTH_SIZING)
set ::env(SYNTH_SIZING) 1
echo $::env(SYNTH_SIZING)
echo $::env(SYNTH_DRIVING_CELL)
```
- With SYNTH_STRATEGY of Delay 0, the tool will focus more on optimizing/minimizing the delay, index can be 0 to 3 where 3 is the most optimized for timing (sacrificing more area).
- SYNTH_SIZING of 1 will enable cell sizing where cell will be upsize or downsized as needed to meet timing.<br>
<img width="600" alt="SET_STRATEGY1" src="https://github.com/Sidv005/Samsung-PD-Training/blob/02ddba812831bd12ca3271a69608cf8c5ec1085f/SamsungPD_training/day4_final/SET_STRATEGY1.png"><br>

After modifying the configuration when we give run_synthesis<br>
<img width="600" alt="slack%3D-10(reduced)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/02ddba812831bd12ca3271a69608cf8c5ec1085f/SamsungPD_training/day4_final/slack%3D-10(reduced).png"><br>
When we give run_floorplan we get a error of macro placement so we need to comment the lines from flooplan.tcl. Then when we run_floorplan it works<br>
<img width="600" alt="run_floorplan" src="https://github.com/Sidv005/Samsung-PD-Training/blob/02ddba812831bd12ca3271a69608cf8c5ec1085f/SamsungPD_training/day4_final/run_floorplan.png"><br>

Then we need to give run_placement<br>
<img width="600" alt="run_placement" src="https://github.com/Sidv005/Samsung-PD-Training/blob/02ddba812831bd12ca3271a69608cf8c5ec1085f/SamsungPD_training/day4_final/run_placement.png"><br>

<img width="600" alt="place_layout" src="https://github.com/Sidv005/Samsung-PD-Training/blob/02ddba812831bd12ca3271a69608cf8c5ec1085f/SamsungPD_training/day4_final/place_layout.png"><br>
</details>

<details>
 <summary>Setup Time analsysis and flop setup time</summary>
	
*Setup Time (Ts) < Clock Period (T) - Combinational Delay (o)*

In this condition, Ts represents the minimum required time for the data to be stable before the clock edge arrives. The clock period T is the time between consecutive clock edges, and "o" is the combinational delay, which is the time taken by the logic between the data input and the flip-flop's clock input to process the data.

- This inequality ensures that there is sufficient time for the data to settle before the clock edge, preventing metastability or incorrect data capture in the flip-flop or latch.<br>
<img width="600" alt="pic_setup" src="https://github.com/Sidv005/Samsung-PD-Training/blob/48dc18c3c1d6a4345ce30928ae694884a256e207/SamsungPD_training/day4_final/pic_setup.PNG"><br>
<img width="600" alt="pic_setup2" src="https://github.com/Sidv005/Samsung-PD-Training/blob/48dc18c3c1d6a4345ce30928ae694884a256e207/SamsungPD_training/day4_final/pic_setup2.PNG"><br>

**Clock Jitter and Uncertainity**
- Clock jitter, found in electronics and digital systems, denotes the deviation from the expected, regular timing of a clock signal.
- This irregularity can stem from multiple factors and is of significant concern in situations demanding precise timing, including high-speed digital communication, signal processing, and high-performance computing.

Consider the below example<br>
<img width="600" alt="jitter1" src="https://github.com/Sidv005/Samsung-PD-Training/blob/48dc18c3c1d6a4345ce30928ae694884a256e207/SamsungPD_training/day4_final/jitter1.PNG"><br>

- In this context, we anticipate the clock signal to arrive precisely at the clock pin at either 0 seconds or at Ts. However, in practical situations, achieving exact timing can be challenging due to inherent variations in clock source generation. As a result, we need to adjust our understanding of combinational delay to accommodate the inherent uncertainty introduced by clock jitter.
- This means that the combinational delay becomes more critical and should consider the impact of clock jitter on timing requirements.<br>

<img width="600" alt="jitter2" src="https://github.com/Sidv005/Samsung-PD-Training/blob/48dc18c3c1d6a4345ce30928ae694884a256e207/SamsungPD_training/day4_final/jitter2.PNG"><br>
</details>

<details>
 <summary>Steps to configure OpenSTA</summary>
- Firstly we have to write a pre_sta.conf file<br>
<img width="600" alt="pre_sta_conf" src="https://github.com/Sidv005/Samsung-PD-Training/blob/65a532a682167581f10bdfb2c7c311cb7c2f8446/SamsungPD_training/day4_final/pre_sta_conf.tcl.PNG"><br>
- Then we need to run sta pre_sta.conf<br>
<img width="600" alt="pre_sta_conf" src="https://github.com/Sidv005/Samsung-PD-Training/blob/65a532a682167581f10bdfb2c7c311cb7c2f8446/SamsungPD_training/day4_final/pre_sta.png"><br>

</details>

<details>
 <summary>Clock Tree Synthesis TritconCTS and signal integrity</summary>
	
In STA use the below command
```ruby
write_verilog ~/Desktop/work/tools/openlane_working_dir/openlane/designs/picorv32a/runs/crct2/results/synthesis/picorv32a.synthesis.v
```
- Now we need to use the below commands in openlane<br>
```ruby
run_floorplan
run_placement
run_cts
```
.def file is generated in cts which is shown below.<br>
<img width="600" alt="(after_cts_def)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/65a532a682167581f10bdfb2c7c311cb7c2f8446/SamsungPD_training/day4_final/(after_cts_def).png"><br>

*Verifying the CTS design*

- Use the below commands in openlane
```ruby
echo $::env(LIB_TYPICAL)
echo $::env(CURRENT_DEF)
echo $::env(CTS_MAX_CAP)
echo $::env(CTS_CLK_BUFFER_LIST)
echo $::env(CTS_ROOT_BUFFER)
```

<img width="600" alt="(after_cts_def)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/65a532a682167581f10bdfb2c7c311cb7c2f8446/SamsungPD_training/day4_final/(after_cts_verify).png"><br>

</details>

<details>
 <summary>Timing Analysis with real clocks</summary>

Executing these commands in OpenLANE:
```ruby
openroad                                                                                                       
read_lef designs/picorv32a/runs/13-01_14-09/tmp/merged.lef
read_def designs/picorv32a/runs/13-01_14-09/results/cts/picorv32a.cts.def
write_db pico_cts.db
read_db pico_cts.db
read_verilog designs/picorv32a/runs/crct2/results/synthesis/picorv32a.synthesis_cts.v
read_liberty -max $::env(OPENLANE_ROOT)/designs/picorv32a/src/sky130_fd_sc_hd__slow.lib
read_liberty -min $::env(OPENLANE_ROOT)/designs/picorv32a/src/sky130_fd_sc_hd__fast.lib
set_propagated_clock [all_clocks]
read_sdc designs/picorv32a/src/my_base.sdc
report_checks -path_delay min_max -format full_clock_expanded -digits 4
```
These are the outputs of the above commands shown in below figure.<br>
<img width="600" alt="(openroad_commands)2" src="https://github.com/Sidv005/Samsung-PD-Training/blob/65a532a682167581f10bdfb2c7c311cb7c2f8446/SamsungPD_training/day4_final/(openroad_commands)2.png"><br>

From the below image we can observe that min slack is met.<br> 
<img width="600" alt="(openroad_min_slack)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/65a532a682167581f10bdfb2c7c311cb7c2f8446/SamsungPD_training/day4_final/(openroad_min_slack).png"><br>
Max is violating<br>
<img width="600" alt="(openroad_max_slack)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/65a532a682167581f10bdfb2c7c311cb7c2f8446/SamsungPD_training/day4_final/(openroad_max_slack).png"><br>

***Steps to execute STA with right timing library***

In order to meet the max slack we follow the below commands:-
```ruby
exit        (Exit openroad)
openroad
read_db pico_cts.db
read_verilog /openLANE_flow/designs/picorv32a/runs/13-01_14-09/results/synthesis/picorv32a.synthesis_cts.v
read_liberty $::env(LIB_SYNTH_COMPLETE)
link_design picorv32a
read_sdc designs/picorv32a/src/my_base.sdc
set_propagated_clock [all_clocks]
report_checks -path_delay min_max -fields {slew trans net cap input pin} -format full_clock_expanded
echo $::env(CTS_CLK_BUFFER_LIST)
```
Following the verification of checks in the report, we observe that both the minimum and maximum requirements have been satisfied.<br>
<img width="600" alt="slack_met1" src="https://github.com/Sidv005/Samsung-PD-Training/blob/299e9f62c6ad297ccc575256fe1916b6c40f6c77/SamsungPD_training/day4_final/slack_met1.PNG"><br>
<img width="600" alt="slack_met2" src="https://github.com/Sidv005/Samsung-PD-Training/blob/299e9f62c6ad297ccc575256fe1916b6c40f6c77/SamsungPD_training/day4_final/slackmet2.PNG"><br>

*Steps to observe impact of bigger CTS buffers on setup and hold timing*

Initially, we need to execute these commands in OpenLANE. In this process, we are converting the current DEF (Design Exchange Format) file to a placement-specific DEF file.
```ruby
exit 
echo $::env(CTS_CLK_BUFFER_LIST)
set ::env(CTS_CLK_BUFFER_LIST) [lreplace $::env(CTS_CLK_BUFFER_LIST) 0 0]
echo $::env(CURRENT_DEF)
set ::env(CURRENT_DEF) /openLANE_flow/designs/picorv32a/runs/13-01_14-09/results/placement/picorv32a.placement.def
run_cts
```
The output of the above commands is shown below.<br>
<img width="600" alt="commands1" src="https://github.com/Sidv005/Samsung-PD-Training/blob/d3a9c83fc1937f943217921722ab4623f4ef7e89/SamsungPD_training/day4_final/commands1.PNG"><br>

In OpenLANE, these commands must be executed to assess the effect of large buffers. In this case, we are solely focused on timing analysis by loading the DEF, LEF, and cts.v files.<br>
```ruby
openroad
read_lef /openLANE_flow/designs/picorv32a/runs/13-01_14-09/tmp/merged.lef
read_def /openLANE_flow/designs/picorv32a/runs/13-01_14-09/results/cts/picorv32a.cts.def
write_db pico_cts1.db
read_db pico_cts1.db
read_verilog /openLANE_flow/designs/picorv32a/runs/13-01_14-09/results/synthesis/picorv32a.synthesis_cts.v
read_liberty $::env(LIB_SYNTH_COMPLETE)
link_design picorv32a
read_sdc designs/picorv32a/src/my_base.sdc
set_propagated_clock [all_clocks]
report_checks -path_delay min_max -fields {slew trans net cap input pin} -format full_clock_expanded
```
We can observe that max slack got improved from 5.10 to 5.18.<br>
<img width="600" alt="commands1" src="https://github.com/Sidv005/Samsung-PD-Training/blob/d3a9c83fc1937f943217921722ab4623f4ef7e89/SamsungPD_training/day4_final/slackmet3.PNG"><br>
</details>

## Day-19 Final Step RTL to GDSII ##
<details>
 <summary>Introduction to maze Routing use Lee's Algorithm</summary>

***Routing***

Routing in the context of VLSI (Very Large Scale Integration) pertains to the intricate task of establishing connections among different elements within an integrated circuit, including transistors, logic gates, and various electronic components. This is achieved by creating an intricate network of interconnected wires or metal layers. The quality and efficiency of routing are of paramount importance as they directly impact the performance and functionality of VLSI chips. VLSI routing primarily consists of two main categories: global routing and detailed routing.

***Maze Routing Lee's Algorithm***

The Lee algorithm, which is sometimes referred to as the Lee-Moore algorithm, is a widely employed pathfinding or maze routing technique within the realm of computer science, notably in the domains of VLSI design and printed circuit board (PCB) design. Its primary function is to determine the most efficient route between two points on a grid or maze while accounting for obstacles or obstructed areas. This algorithm operates on a breadth-first search (BFS) principle and is frequently utilized during the intricate routing phases in VLSI design.

<img width="800" alt="pic1" src="https://github.com/Sidv005/Samsung-PD-Training/blob/7d341dd1400516ddbd940e228b96f016f0c1eda5/day19/pic1.PNG"><br>

The procedural steps in Lee Algorithm is as follows. 

*Initialization :*

To prepare for the pathfinding process, begin by establishing a grid or maze where each cell has two potential states: it can either be unoccupied (open) or obstructed. Designate one of these cells as the starting point, denoting it as the source cell, and choose another cell as the destination point, which will serve as the target cell. Next, create a queue data structure to keep track of the cells that need to be examined during the exploration.

*Breadth-First Search :*

Commence by taking the source cell and placing it into the queue.
Assign a step count of 0 to the source cell.
Initiate a loop that will continue as long as there are cells in the queue.
For each cell within the queue:

- Examine the adjacent cells in all four directions (up, down, left, and right). Ensure that these neighboring cells are unobstructed and haven't been visited yet.
- If a neighboring cell is unvisited, mark it as visited, enqueue it, and set its step count as the current cell's step count incremented by one.
- Continue this process until the destination cell is reached or until there are no more cells to explore.

*Backtracking :*

Upon reaching the destination cell, the algorithm can backtrack its steps from the destination back to the source. This is achieved by inspecting neighboring cells and selecting the one with a shorter distance value at each stage, effectively retracing the shortest path from the destination to the source.

*Path Construction:*

- Following the backtracking process, the algorithm reconstructs the path from the source to the destination, ultimately determining the shortest route.

- The Lee algorithm holds particular significance in the context of detailed routing for VLSI design. This is because it excels in identifying the shortest path, all while considering the grid's layout and potential obstacles. It offers an efficient means to navigate around hindrances, steer clear of congestion, and establish connections between different elements on an integrated circuit.

<img width="600" alt="pic2" src="https://github.com/Sidv005/Samsung-PD-Training/blob/7d341dd1400516ddbd940e228b96f016f0c1eda5/day19/pic2.PNG"><br>

<img width="800" alt="pic3" src="https://github.com/Sidv005/Samsung-PD-Training/blob/7d341dd1400516ddbd940e228b96f016f0c1eda5/day19/pic3.PNG"><br>

The Lee algorithm boasts a notable advantage in that it assures the discovery of the shortest path. Nevertheless, it should be noted that its memory requirements can be substantial, and it may become computationally demanding when dealing with sizable grids or mazes. To mitigate these constraints, a variety of adaptations and enhancements have been developed. These include the bidirectional Lee algorithm, the A* algorithm, and hierarchical iterations tailored for PCB routing, all of which aim to optimize and refine the original Lee algorithm.
</details>

<details>
 <summary>Design Rule Checks</summary>

- Design Rule Checks (DRC) play a pivotal role in the integrated circuit (IC) design and manufacturing workflow, particularly in the realm of Very Large Scale Integration (VLSI) design.

- DRC encompasses a series of directives and assessments employed to verify that the IC's layout complies with both manufacturing and design standards. These standards are indispensable in ensuring the successful manufacturing of the IC and its subsequent performance in alignment with the intended specifications.

Some of the Design Rule checks are illustrated in the below figure.<br>
<img width="600" alt="pic4" src="https://github.com/Sidv005/Samsung-PD-Training/blob/8628a922c6bd7c820ab305342bfe1355a0010711/day19/pic4.PNG"><br>
- A signal short, classified as a DRC violation, occurs when two wires that shouldn't be connected inadvertently make contact on the same layer. Such an occurrence can potentially result in functional failures, necessitating prompt attention.

- To resolve this issue, a straightforward solution involves relocating one of the wires to a separate metal layer. It's essential to bear in mind that this adjustment must adhere to any new DRC rules that have been introduced.
  
<img width="600" alt="pic5" src="https://github.com/Sidv005/Samsung-PD-Training/blob/8628a922c6bd7c820ab305342bfe1355a0010711/day19/pic5.PNG"><br>

- Conducting parasitic extraction involves the retrieval of resistance and capacitance values associated with the wires, which will subsequently be applied in downstream procedures.
  </details>

  <details>
 <summary>Labs</summary>

To run OpenLANE following commands are executed.
```ruby
cd work/tools/openlane_working_dir/openlane
make mount
pwd
ls -ltr
./flow.tcl -interactive
package require openlane 0.9
prep -design picorv32a -tag 13-01_14-09
```
In OpenLANE
```ruby
echo $::env(CURRENT_DEF)    (Ensure current_def is on the CTS stage)
gen_pdn                     (To generate power distribution network)
```

Below images illustrates the occurence of errors when above commands are runned.<br>
<img width="600" alt="route_pic7" src="https://github.com/Sidv005/Samsung-PD-Training/blob/799df10e787d03f566a7e068394ae1f66348237e/day19/route_pic7.PNG"><br>
<img width="600" alt="route_pic8" src="https://github.com/Sidv005/Samsung-PD-Training/blob/799df10e787d03f566a7e068394ae1f66348237e/day19/route_pic8.PNG"><br>

***Fundamentals of global and detail routing and configure TritonRoute***

```ruby
echo $::env(CURRENT_DEF)            (Ensure the def file of pdn has been created)
echo $::env(ROUTING_STRATEGY)
set ::env(CURRENT_DEF) <path_of_cts.def>
run_routing
```

Executing the "run_routing" command yields the following result:<br>
<img width="600" alt="route_pic9" src="https://github.com/Sidv005/Samsung-PD-Training/blob/799df10e787d03f566a7e068394ae1f66348237e/day19/route_pic9.PNG"><br>

Below screenshot shows the results folder.<br>
<img width="600" alt="route_pic10" src="https://github.com/Sidv005/Samsung-PD-Training/blob/799df10e787d03f566a7e068394ae1f66348237e/day19/route_pic10.PNG"><br>

</details>

## Day-20 Floorplanning and power planning labs ##
<details>
 <summary>Theory</summary>
	The physical design flow in VLSI (Very Large Scale Integration) is a series of steps that transform a high-level hardware description of a digital circuit into a physical layout that can be fabricated as an integrated circuit (IC) on a semiconductor wafer. This flow involves several stages and a range of tools and methodologies. Here is an overview of the typical steps in the physical design flow:

1. Design Specification: This is the initial step where you gather requirements and specifications for the digital circuit. It includes understanding the functionality, power consumption, performance, area constraints, and other design goals.

2. RTL Design: Register Transfer Level (RTL) design involves creating a high-level representation of the digital circuit in a hardware description language (HDL) like VHDL or Verilog. The RTL description typically consists of flip-flops, registers, and the interconnections between them.

3. Logic Synthesis: This step involves converting the RTL description into a gate-level representation. Logic synthesis tools map the RTL to a library of standard cells, optimizing for area, power, and speed while meeting the design constraints.

4. Floor Planning: In this phase, you decide on the placement of different functional blocks and macros on the chip. It involves defining the size and location of each block to optimize for area, power, and signal routing.

5. Power Planning: Power distribution networks are designed to ensure that all parts of the chip receive a stable and adequate power supply. This includes the design of power grids and voltage regulation circuits.

6. Placement: The placement stage determines the physical locations of each standard cell on the chip. Tools aim to minimize wirelength, optimize for timing, and meet other design constraints.

7. Clock Tree Synthesis (CTS): CTS is the process of designing a clock distribution network to ensure that clock signals reach all the flip-flops and latches with minimal skew and low power consumption.

8. Routing: The routing step involves creating the physical wires (metal layers) that connect the gates, ensuring that all connections meet design requirements and constraints. Global and detailed routing are usually performed.

9. Design for Manufacturing (DFM): DFM considerations address manufacturability issues like lithography, etching, and other process-related aspects to ensure the chip can be manufactured with high yield.

10. Design Verification: Extensive verification is carried out at each stage of the physical design flow to ensure that the final layout adheres to the original design specifications and that it is free from logical and physical errors.

11. Physical Verification: This involves checking the design against manufacturing rules, including design rule checking (DRC) and layout vs. schematic (LVS) checks.

12. Extraction: Parasitic capacitances and resistances are extracted from the layout and included in the simulation models to accurately predict circuit behavior.

13. Sign-off: This is the final review and approval stage before tape-out, where the design is deemed ready for fabrication.

14. Tape-out: Once the design is thoroughly reviewed, validated, and optimized, it is sent for semiconductor fabrication. A set of files representing the design layout is created and submitted to the foundry.

15. Post-Tapeout Tasks: After fabrication, there may be additional tasks such as package design, testing, and assembly before the final IC is ready for use.

The physical design flow in VLSI is a complex and iterative process that requires careful planning and the use of various EDA (Electronic Design Automation) tools. Success in physical design depends on meeting the design goals and constraints while optimizing for power, area, and performance.
</details>

<details>
 <summary>Labs</summary>
	
```ruby
git clone https://github.com/manili/VSDBabySoC.git
git clone https://github.com/Devipriya1921/VSDBabySoC_ICC2.git
git clone https://github.com/bharath19-gs/synopsys_ICC2flow_130nm.git
git clone https://github.com/kunalg123/icc2_workshop_collaterals.git
git clone https://github.com/google/skywater-pdk-libs-sky130_fd_sc_hd.git
git clone https://github.com/kunalg123/sky130RTLDesignAndSynthesisWorkshop.git
```

 ```ruby
gvim vsdbabysoc.tcl &
gvim avsdpll.lib &
```

*vsdbabysoc.tcl*
- Modifying the contents to my path, remove -lib in read_lib commands, and replace MYCLK to clk since the clock used in the design is {clk}
- All of the commands have been inserted in gvim and the tool will run it once at a time.<br>
<img width="800" alt="1.vsdbabysoc.tcl" src=" https://github.com/Sidv005/Samsung-PD-Training/blob/5867dee56a51d6d04d937d6db09f9af1480ebff6/day20/1.vsdbabysoc.tcl.png"><br>

 *avsdpll.lib*
 
- Remove the unwanted pins<br>
  
<img width="800" alt="3.avsdpll.lib" src="https://github.com/Sidv005/Samsung-PD-Training/blob/5867dee56a51d6d04d937d6db09f9af1480ebff6/day20/3.avsdpll.lib.png"><br>

```ruby
dc_shell
source vsdbabysoc.tcl
```
***Reports***

Report timing image is shown below.<br>
<img width="800" alt="pic3_timing" src="https://github.com/Sidv005/Samsung-PD-Training/blob/5867dee56a51d6d04d937d6db09f9af1480ebff6/day20/pic3_timing.png"><br>

Report area image is shown below.<br>
<img width="800" alt="pic4_area" src="https://github.com/Sidv005/Samsung-PD-Training/blob/5867dee56a51d6d04d937d6db09f9af1480ebff6/day20/pic4_area.png"><br>

Report power image is shown below.<br>
<img width="800" alt="pic5_power" src="https://github.com/Sidv005/Samsung-PD-Training/blob/5867dee56a51d6d04d937d6db09f9af1480ebff6/day20/pic5_power.png"><br>

***Output schematic***<br>
<img width="800" alt="sche_pic1" src="https://github.com/Sidv005/Samsung-PD-Training/blob/5867dee56a51d6d04d937d6db09f9af1480ebff6/day20/sche_pic1.png"><br>

*RVMYTH core*<br>
<img width="800" alt="sche_pic2" src="https://github.com/Sidv005/Samsung-PD-Training/blob/5867dee56a51d6d04d937d6db09f9af1480ebff6/day20/sche_pic2.png"><br>

***Performing physical design***

```ruby
gvim top.tcl
gvim icc2_common_setup.tcl
gvim icc2_dp_setup.tcl
gvim init_design.read_parasitic_tech_example.tcl
gvim init_design.mcmm_example.auto_expanded.tcl
gvim pns_example.tcl
```
*Modifying files*

1. top.tcl<br>
<img width="800" alt="3.top.tcl" src="https://github.com/Sidv005/Samsung-PD-Training/blob/5867dee56a51d6d04d937d6db09f9af1480ebff6/day20/3.top.tcl.png"><br>

2. icc2_common_setup.tcl<br>
<img width="800" alt="4.icc2_common.tcl" src="https://github.com/Sidv005/Samsung-PD-Training/blob/5867dee56a51d6d04d937d6db09f9af1480ebff6/day20/4.icc2_common.tcl.png"><br>

3. icc2_dp_setup.tcl<br>
<img width="800" alt="5.icc2_dp.tcl" src="https://github.com/Sidv005/Samsung-PD-Training/blob/5867dee56a51d6d04d937d6db09f9af1480ebff6/day20/5.icc2_dp.tcl.png"><br>

4. init_design.read_parasitic_tech_example.tcl<br>
<img width="800" alt="6.init_example.tcl" src="https://github.com/Sidv005/Samsung-PD-Training/blob/5867dee56a51d6d04d937d6db09f9af1480ebff6/day20/6.init_example.tcl.png"><br>
 
5. init_design.mcmm_example.auto_expanded.tcl<br>
<img width="800" alt="7.init_expanded.tcl" src="https://github.com/Sidv005/Samsung-PD-Training/blob/5867dee56a51d6d04d937d6db09f9af1480ebff6/day20/7.init_expanded.tcl.png"><br>

6. pns_example.tcl<br>
<img width="800" alt="8.pns_ex.tcl" src="https://github.com/Sidv005/Samsung-PD-Training/blob/5867dee56a51d6d04d937d6db09f9af1480ebff6/day20/8.pns_ex.tcl.png"><br>

**Observing for 40% of utilization**

***Output Layout***

```ruby
source top.tcl
```

<img width="800" alt="pic7_floorplan_plac" src="https://github.com/Sidv005/Samsung-PD-Training/blob/5867dee56a51d6d04d937d6db09f9af1480ebff6/day20/pic7_floorplan_plac.png"><br>

<img width="800" alt="pic8_chip" src="https://github.com/Sidv005/Samsung-PD-Training/blob/5867dee56a51d6d04d937d6db09f9af1480ebff6/day20/pic8_chip.png"><br>

Below screenshot displays the timing report showing slack = -5.31. <br>
<img width="800" alt="pic9_40%25_before_propagated" src="https://github.com/Sidv005/Samsung-PD-Training/blob/5867dee56a51d6d04d937d6db09f9af1480ebff6/day20/pic9_40%25_before_propagated.png"><br>

In icc2_shell

```ruby
set_propagated_clock [all_clocks]             (Converting clock object from ideal clock to propagated clock)
report_timing
```

<img width="800" alt="pic10_40%25_after_propagated" src="https://github.com/Sidv005/Samsung-PD-Training/blob/5867dee56a51d6d04d937d6db09f9af1480ebff6/day20/pic10_40%25_after_propagated.png"><br>

*violators.rpt*

```ruby
gvim violators.rpt	     (Reviewing violations report within the design)
```

<img width="800" alt="pic13_40-50%25violators" src="https://github.com/Sidv005/Samsung-PD-Training/blob/5867dee56a51d6d04d937d6db09f9af1480ebff6/day20/pic13_40-50%25violators.png"><br>

**Observing for 50% of utilization**

*Slacks*

<img width="800" alt="pic11_50%25_before_propagated" src="https://github.com/Sidv005/Samsung-PD-Training/blob/5867dee56a51d6d04d937d6db09f9af1480ebff6/day20/pic11_50%25_before_propagated.png"><br>

In icc2_shell

```ruby
set_propagated_clock [all_clocks]             (Converting clock object from ideal clock to propagated clock)
report_timing
```

Here observe that slack is getting increased.<br>
<img width="800" alt="pic12_50%25_after_propagated" src="https://github.com/Sidv005/Samsung-PD-Training/blob/5867dee56a51d6d04d937d6db09f9af1480ebff6/day20/pic12_50%25_after_propagated.png"><br>

Here we can observe that slack is getting increased when core utilization is increased from 40% to 50%.
</details>

## Day-21 Placement and CTS labs ##
<details>
 <summary>Theory</summary>

1. Placement in IC design refers to the vital process of determining the physical locations of electronic components within an integrated circuit (IC). This step is of paramount importance in the overall IC design process, as it significantly impacts the final performance, power consumption, and manufacturability of the chip. The primary objective of placement is to allocate a physical position for each logic gate, flip-flop, or other components on the chip, with the goal of minimizing wirelength, reducing congestion, and optimizing factors like signal delay and power consumption.

2. Routing in VLSI design involves the task of interconnecting various components, such as logic gates and flip-flops, placed on an integrated circuit (IC) with the necessary wires or interconnects. The primary goal of routing is to establish an efficient and reliable network of connections between these components on the chip. This network must meet timing constraints, minimize wirelength, and alleviate congestion issues.

3. Clock Tree Synthesis (CTS) is a critical phase in the design of digital integrated circuits, particularly those featuring synchronous logic, such as microprocessors and application-specific integrated circuits (ASICs). The primary purpose of CTS is to create a well-organized and optimized distribution network for clock signals, ensuring that all sequential elements, such as flip-flops, receive clock signals with minimal skew, low latency, and low power consumption.
</details>

<details>
 <summary>Labs</summary>
	
**Observing for 40% of utilization**

Generated vsdbabysoc.sdc after synthesis is shown below.<br>
<img width="800" alt="1.vsdbabysoc.sdc" src="https://github.com/Sidv005/Samsung-PD-Training/blob/6db24cbdb313b2f3ac3d6caa1cd2cbb4ea0af24f/day21/1.vsdbabysoc.sdc.png"><br>

Script in top.tcl

1. create_placement is used to create placement for the design. floorplan option is selected to make the design planning styled as placement.
2. Pin Placement is done by sourcing pns.tcl to sync with the current technology file regarding power grid creation.<br>
<img width="800" alt="pic1_create_placement" src="https://github.com/Sidv005/Samsung-PD-Training/blob/6db24cbdb313b2f3ac3d6caa1cd2cbb4ea0af24f/day21/pic1_create_placement.png"><br>

<img width="800" alt="pic2_create_placement" src="https://github.com/Sidv005/Samsung-PD-Training/blob/6db24cbdb313b2f3ac3d6caa1cd2cbb4ea0af24f/day21/pic2_create_placement.png"><br>

*Reports that were generated from the run*

```ruby
gvim check_design.pre_pin_placement
```
As shown in below figure there are 3 warnings in total for pre-placement while checking the design.
<img width="800" alt="pic3_pre_placement_warnings" src="https://github.com/Sidv005/Samsung-PD-Training/blob/6db24cbdb313b2f3ac3d6caa1cd2cbb4ea0af24f/day21/pic3_pre_placement_warnings.png"><br>

```ruby
gvim report_port_placement.rpt
```
Below image shows the report_port_placement.<br>
<img width="800" alt="pic4_report_port_placement.rpt" src="https://github.com/Sidv005/Samsung-PD-Training/blob/6db24cbdb313b2f3ac3d6caa1cd2cbb4ea0af24f/day21/pic4_report_port_placement.rpt.png"><br>

```ruby
gvim icc2_output.txt
```
Below image shows the icc2_output<br>
<img width="800" alt="pic5_icc2_output_txt" src="https://github.com/Sidv005/Samsung-PD-Training/blob/6db24cbdb313b2f3ac3d6caa1cd2cbb4ea0af24f/day21/pic5_icc2_output_txt.png"><br>
<img width="800" alt="pic6_icc2_output.txt" src="https://github.com/Sidv005/Samsung-PD-Training/blob/6db24cbdb313b2f3ac3d6caa1cd2cbb4ea0af24f/day21/pic6_icc2_output.txt.png"><br>

```ruby
gvim vsdbabysoc.post_estimated_timing.rpt
```
Below image shows the report of vsdbabysoc.post_estimated_timing <br>
<img width="800" alt="pic7_post_estimated_timing.rpt" src="https://github.com/Sidv005/Samsung-PD-Training/blob/6db24cbdb313b2f3ac3d6caa1cd2cbb4ea0af24f/day21/pic7_post_estimated_timing.rpt.png"><br>

From abve image we can see that slack is met at 0.47.

```ruby
gvim vsdbabysoc.post_estimated_timing.qor
```
Below image shows the qor report of vsdbabysoc.post_estimated_timing<br>
<img width="800" alt="pic8_post_estimated_timing.qor" src="https://github.com/Sidv005/Samsung-PD-Training/blob/6db24cbdb313b2f3ac3d6caa1cd2cbb4ea0af24f/day21/pic8_post_estimated_timing.qor.png"><br>
<img width="800" alt="pic9_post_estimated_timing.qor2" src="https://github.com/Sidv005/Samsung-PD-Training/blob/6db24cbdb313b2f3ac3d6caa1cd2cbb4ea0af24f/day21/pic9_post_estimated_timing.qor2.png"><br>

From above image we can observe that Post estimated timing qor shows there is no violating path reported with 61 nets having violations, 58 max trans violations, and 61 max cap violations.

```ruby
gvim vsdbabysoc.post_estimated_timing.qor.sum
```

Below image shows the summary on qor report of vsdbabysoc.post_estimated_timing <br>
<img width="800" alt="pic10_post_estimated_timing.qor.sum" src="https://github.com/Sidv005/Samsung-PD-Training/blob/6db24cbdb313b2f3ac3d6caa1cd2cbb4ea0af24f/day21/pic10_post_estimated_timing.qor.sum.png"><br>

CTS schematic design Analysis:-<br>
<img width="800" alt="pic11_pll_schematic" src="https://github.com/Sidv005/Samsung-PD-Training/blob/6db24cbdb313b2f3ac3d6caa1cd2cbb4ea0af24f/day21/pic11_pll_schematic.png"><br>

Fanout<br>
<img width="800" alt="pic12_chip_schematic" src="https://github.com/Sidv005/Samsung-PD-Training/blob/ca6217afe177fc0d689c543602a5391919fd13d1/day21/pic12_chip_schematic.png"><br>
 </details>

## Day-22 CTS Analysis ##

<details>
 <summary>Theory</summary>
	
**What is CTS?**

- Clock Tree Synthesis
- A technique for distributing the clock equally among all sequential parts of VLSI design
- It will balancing the delays to all clock input pins when the clock is distributed equally
- The goal of CTS is to minimize skew and insertion delay.

**H-tree algorithm**

- Find out all the flops present
- Find out the center of all the flops
- Trace clock port ot the center point
- Divide the core into two parts, trace both the parts and reach to each center
- From the center, again, divide the area into two and again trace till center at both the end
- Repeat this algo till the time we reach the flop clock pin

**Various CTS checks**

1.  Skew check
2.  Pulse width check
3.  Duty cycle check
4.  Latency check
5.  Power check
6.  Crosstalk Quality check
7.  Delta Delay Quality check
8.  Glitch Quality check


</details>

<details>
 <summary>LABS</summary>

**CTS Lab analysis**

*Using 40% of utilization*

- ***After CTS, we do synthesis***
- Before we synthesize the clock trees, use below command to verify that the clock trees are properly defined

```ruby
check_clock_tree                        (Checking the issues that can lead to bad QoR)
```
This is used to check for common problems that might impact CTS. Verifies the given clock tree in current design to display possible issues with netlist, timing performance, etc. One warning which states that there are some clock cells that does not have LEQ cells for resizing is shown in below image.<br>
<img width="800" alt="1.check_clock_tree" src="https://github.com/Sidv005/Samsung-PD-Training/blob/a743713ffa13028e27e51df27b2f3be15f4de07c/day22/1.check_clock_tree.png"><br>

```ruby
check_legality                          (Checking the legality of the current placement and report out the violation statistics)
```
This command checks the legality of the curreent_placement and yields to report of violation statistics as shown in below image.<br>
<img width="800" alt="2.check_legality" src="https://github.com/Sidv005/Samsung-PD-Training/blob/a743713ffa13028e27e51df27b2f3be15f4de07c/day22/2.check_legality.png"><br>

- In top.tcl as we can view that *clock_opt* is present, this is used to to perform clock tree synthesis and it optimizes the clock trees.<br>
<img width="800" alt="6.clock_opt_top.tcl" src="https://github.com/Sidv005/Samsung-PD-Training/blob/0b82ec75551edffd3b46f13399e06d17b72d8a3a/day22/6.clock_opt_top.tcl.png"><br>

Reports:-

```ruby
report_clock_timing -type summary
```

<img width="800" alt="3.report_timing_summ" src="https://github.com/Sidv005/Samsung-PD-Training/blob/0b82ec75551edffd3b46f13399e06d17b72d8a3a/day22/3.report_timing_summ.png"><br>

```ruby
report_clock_timing -type skew
```

<img width="800" alt="4.report_timing_skew" src="https://github.com/Sidv005/Samsung-PD-Training/blob/0b82ec75551edffd3b46f13399e06d17b72d8a3a/day22/4.report_timing_skew.png"><br>

```ruby
report_clock_timing -type latency
```

<img width="800" alt="5.report_timing_latency" src="https://github.com/Sidv005/Samsung-PD-Training/blob/0b82ec75551edffd3b46f13399e06d17b72d8a3a/day22/5.report_timing_latency.png"><br>

```ruby
report_clock_timing -type transition
```

<img width="800" alt="7.transition" src="https://github.com/Sidv005/Samsung-PD-Training/blob/97ec83e6cdc547bf6f3683ff5c3bcb240e0aa524/day22/7.transition.png"><br>

```ruby
report_clock_tree_options
```
Above command gives the Reports existing target skew/latency constraints, fanout-based ndr, etcfor clock trees. Below screenshot shows that no clock skew and latency is present since we have not set any constraints yet.<br>

<img width="800" alt="12.options" src="https://github.com/Sidv005/Samsung-PD-Training/blob/41aba70f2ce13a495f4ade13a5b3a7e21007bea5/day22/12.options.png"><br>

</details>
