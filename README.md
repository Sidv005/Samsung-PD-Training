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

***Synthesizing the clock trees***
- Before we synthesize the clock trees, use below command to verify that the clock trees are properly defined

```ruby
check_clock_tree                        (Checking the issues that can lead to bad QoR)
```
- Checks the clock trees of current design for possible problems with netlist, timing constraints, clock constraints, routing constraints, or other tool configurations that can adversely impact clock tree synthesis.
- This is used to check for common problems that might impact CTS. Verifies the given clock tree in current design to display possible issues with netlist, timing performance, etc. One warning which states that there are some clock cells that does not have LEQ cells for resizing is shown in below image.<br>
<img width="800" alt="1.check_clock_tree" src="https://github.com/Sidv005/Samsung-PD-Training/blob/a743713ffa13028e27e51df27b2f3be15f4de07c/day22/1.check_clock_tree.png"><br>

```ruby
check_legality                          (Checking the legality of the current placement and report out the violation statistics)
```
- This command checks the legality of the current_placement and yields to report of violation statistics as shown in below image.
- Checks basic rules such as overlap, cell_on_site, and legal_orient, and AL rules such as spacing_rule, and chipfinishing rules such as tap_coverage, continuity, etc.<br>
<img width="800" alt="2.check_legality" src="https://github.com/Sidv005/Samsung-PD-Training/blob/a743713ffa13028e27e51df27b2f3be15f4de07c/day22/2.check_legality.png"><br>

- In top.tcl as we can view that *clock_opt* is present, this is used to to perform clock tree synthesis and it optimizes the clock trees.
- The default behavior of this command is as follows:

1. Synthesizes and optimizes the clock trees.

2. Completes the detail routing of the clock trees.

3. Further optimizes the design for timing,electrical DRC violations, area, power, and routability, based on actual propagated clock latencies, and legalizes the design placement.<br>
<img width="800" alt="6.clock_opt_top.tcl" src="https://github.com/Sidv005/Samsung-PD-Training/blob/0b82ec75551edffd3b46f13399e06d17b72d8a3a/day22/6.clock_opt_top.tcl.png"><br>

Reports:-

```ruby
report_clock_timing -type summary
```
- It shows the Summary report, which shows the worst instances of transition time, latency and skew over the clock networks or subnetworks of interest.<br>
<img width="800" alt="3.report_timing_summ" src="https://github.com/Sidv005/Samsung-PD-Training/blob/0b82ec75551edffd3b46f13399e06d17b72d8a3a/day22/3.report_timing_summ.png"><br>

- The above report displays the two worst setup and two worst hold skews in the clock network of CLK, taking uncertainty into account.

- This is a summary report which shows the worst instances of transition time, latency and skew over the clock network. It gives the maximum setup launch latency which is the worst setup latency of a clock pin in this case it is for the pin *core1/CPU_br_tgt_pc_a3_reg[1]/CLK*. Similarly it gives minimum setup capture latency, minimum hold launch latency, maximum active transition , minimum active transition , maximum and minimum hold skew.

- In the report we can see that the design is working on func1 mode this is operated in single mode single corner.

```ruby
    r         Rising transition

    f         Falling transition

    p         Propagated clock to this pin

    i         Clock inversion to this pin

    -         Launching transition

    +         Capturing transition

    e         Exception on this pin
```
- rp-+ -> rising transition of propagated clock in the clock pin from launch to capture.

The symbol representation is as follows
```ruby
report_clock_timing -type skew
```
- It shows the Skew report.<br>
<img width="800" alt="4.report_timing_skew" src="https://github.com/Sidv005/Samsung-PD-Training/blob/0b82ec75551edffd3b46f13399e06d17b72d8a3a/day22/4.report_timing_skew.png"><br>

```ruby
report_clock_timing -type latency
```
- It shows the  Latency report.
<img width="800" alt="5.report_timing_latency" src="https://github.com/Sidv005/Samsung-PD-Training/blob/0b82ec75551edffd3b46f13399e06d17b72d8a3a/day22/5.report_timing_latency.png"><br>

```ruby
report_clock_timing -type transition
```
- It shows the Transition time report.<br>
<img width="800" alt="7.transition" src="https://github.com/Sidv005/Samsung-PD-Training/blob/97ec83e6cdc547bf6f3683ff5c3bcb240e0aa524/day22/7.transition.png"><br>

```ruby
report_clock_tree_options
```
Above command gives the Reports existing target skew/latency constraints, fanout-based ndr, etc. for clock trees. Below screenshot shows that no clock skew and latency is present since we have not set any constraints yet.<br>

<img width="800" alt="12.options" src="https://github.com/Sidv005/Samsung-PD-Training/blob/41aba70f2ce13a495f4ade13a5b3a7e21007bea5/day22/12.options.png"><br>
</details>

## Day-23 Clock gating technique And Routing ##

<details>
 <summary>Theory</summary>

**Advanced H-Tree for million flop clock end-points randomly placed**

- When CTS is performed, power consumption also needs to be taken care of, especially when designing a large number of clocks where the design might induce a larger power, as well as a larger power usage

- A digital circuit with a lot of clocks would be so huge with many buffers etc when designing its clock tree

- In order to fix that, the whole chip is sectioned into smaller versions where each section will have its own clock tree, and managed to get a complete routed tree

- Therefore, Clock Gating (CG) technique is introduced

**Introduction to Clock Gating technique**

What is Clock Gating (CG)?

It is used to reduce the clock power consumption by cutting off the idle clock cycles


Where/when clock gating is applied?

It is being inserted in synthesis stage and being optimized in the implementation stage (Physical Design stage)

Types of clock gating

1. AND gate
2. OR gate
3. Universal AND gate

**Routing**

What is routing?

The process of making physical connections between signal pins using metal layers

Types of routing

1. P/G routing
2. Clock routing
3. Signal routing: Global & Detailed routing

Basic flow of routing

- Basically, *route_opt* command is used during routing stage

 </details>

<details>
 <summary>LABS</summary>
 
***Script in routing stage***

Thre types of routing are P/G routing, Clock Routing and signal routing.

1. **P/G routing**<br>

We can observe this in pns_example.tcl file.

```ruby
gvim pns_example.tcl
```

<img width="800" alt="2.pnsexample.tcl" src="https://github.com/Sidv005/Samsung-PD-Training/blob/731e7f7c66413fb2b012a776e01ed35571f61606/day23/2.pnsexample.tcl.png"><br>

2. **Clock and signal routing**

1. *place_opt* is used to place and optimize the current design

2. *clock_opt* is used to synthesize and route the clocks, and then further optimize the design based on the propagated clock latencies

3. *route_auto* is used to run global routing, trace assignment, and detailed routing at once/automatically

```ruby
gvim top.tcl
```

<img width="800" alt="1.top.tcl" src="https://github.com/Sidv005/Samsung-PD-Training/blob/731e7f7c66413fb2b012a776e01ed35571f61606/day23/1.top.tcl.png"><br>
	
***Clock tree with clock buffer insertion***

- We need to add 3 lines between place_opt and clock_opt , to insert the clock buffers in the design

```ruby
set_lib_cell_purpose -include cts {sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__buf_*}
synthesize_clock_tree
set_propagated_clock [all_clocks]
```
<img width="800" alt="1.top.tcl(new)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/99286d3294b2c77f498f2f5a69c650585bee2f62/day23/1.top.tcl(new).png"><br>

**set_lib_cell_purpose -include cts {sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__buf_*}** command specifies that the library cells in the tech_lib library(sky130_fd_sc_hd__tt_025C_1v80) whose names start with "buf" should be used for clock tree synthesis.

**synthesize_clock_tree** This command synthesizes clock trees and updates the design database with the compiled clock trees. The compilation of the clock tree is skew driven. Optionally, this command can optimize compiled clock tree for slack metric.

- The command will work on clocks in active scenarios. It will have clocks balanced if either setup or hold analysis is active. It will fix the transition violations on clock pins if max_transition analysis is active, and fix the capacitance violation on clock nets if max_capacitance analysis is active. At the end of this command it will invoke mark_clock_trees to mark clock synthesized attributes on clock objects.

- Before running the synthesize_clock_trees command, the set_lib_cell_purpose command can be applied to select buffers or inverters which used during clock tree synthesis.

**set_propagated_clock [all_clocks]** This command specifies that delays be propagated through the clock network to determine latency at register clock pins, including the delay resulting from parasitic capacitance and resistance. If propagated clocking is not specified, the tool uses ideal clocking by default.

- Ideal clocking means clock networks have a specified latency (from the set_clock_latency command), or zero latency by default. Latency is the amount of time a clock signal takes to be propagated from the ideal waveform origin point to the clock pin of the sequential device.

- Propagated clock latency is used for after final clock tree generation and layout. Ideal clock latency specifies a prelayout estimate of the clock tree delay.

- If you apply the set_propagated_clock command to pins or ports, it affects all register clock pins in the transitive fanout of the specified pins or ports.

Before this we need to change the input voltage to 1.80V

<img width="800" alt="2.mcmm" src="https://github.com/Sidv005/Samsung-PD-Training/blob/99286d3294b2c77f498f2f5a69c650585bee2f62/day23/2.mcmm.png"><br>

- Then when we source this file we can see buffers in the design
- Following image shows the schematic.<br>
  <img width="800" alt="gui_buffer" src="https://github.com/Sidv005/Samsung-PD-Training/blob/99286d3294b2c77f498f2f5a69c650585bee2f62/day23/gui_buffer.png"><br>

- Below image shows some buffers which are inserted.<br>
 <img width="800" alt="1.gui_buffer" src="https://github.com/Sidv005/Samsung-PD-Training/blob/1191fe8a3d3f072986333f5cd5a3a5a588edb5cb/day23/1.gui_buffer.png"><br>

Here we can see that 12 buffers are added in the design.

- From the below image we can see that slack is reduced from -5.91 ns to -0.15 ns since clock buffers are inserted.

Before:-<br>
 <img width="800" alt="pic10_40%25_after_propagated" src="https://github.com/Sidv005/Samsung-PD-Training/blob/99286d3294b2c77f498f2f5a69c650585bee2f62/day20/pic10_40%25_after_propagated.png"><br>

After :-<br>
<img width="800" alt="4.slack_after_buf" src="https://github.com/Sidv005/Samsung-PD-Training/blob/99286d3294b2c77f498f2f5a69c650585bee2f62/day23/4.slack_after_buf.png"><br>

The clock buffers and ICG inserted in the circuit are as follows:
```ruby

Buffer/Inverter reference list for clock tree synthesis:
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__buf_1
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__buf_12
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__buf_16
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__buf_2
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__buf_4
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__buf_6
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__buf_8
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__bufbuf_16
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__bufbuf_8
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__clkbuf_1
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__clkbuf_16
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__clkbuf_2
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__clkbuf_4
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__clkbuf_8
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__clkdlybuf4s15_1
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__clkdlybuf4s15_2
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__clkdlybuf4s18_1
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__clkdlybuf4s18_2
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__clkdlybuf4s25_1
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__clkdlybuf4s25_2
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__clkdlybuf4s50_1
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__clkdlybuf4s50_2
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__dlygate4sd1_1
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__dlygate4sd2_1
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__dlygate4sd3_1
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__dlymetal6s2s_1
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__dlymetal6s4s_1
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__dlymetal6s6s_1
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__probe_p_8
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__probec_p_8
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__lpflow_clkbufkapwr_1
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__lpflow_clkbufkapwr_16
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__lpflow_clkbufkapwr_2
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__lpflow_clkbufkapwr_4
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__lpflow_clkbufkapwr_8
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__bufinv_16
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__bufinv_8
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__clkinv_1
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__clkinv_16
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__clkinv_2
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__clkinv_4
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__clkinv_8
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__clkinvlp_2
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__clkinvlp_4
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__inv_1
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__inv_12
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__inv_16
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__inv_2
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__inv_4
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__inv_6
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__inv_8
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__lpflow_clkinvkapwr_1
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__lpflow_clkinvkapwr_16
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__lpflow_clkinvkapwr_2
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__lpflow_clkinvkapwr_4
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__lpflow_clkinvkapwr_8

ICG reference list:
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__dlclkp_1
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__dlclkp_2
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__dlclkp_4
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__sdlclkp_1
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__sdlclkp_2
   sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__sdlclkp_4
```
 </details>

## Day-24 ECO ##

<details>
 <summary>LABS</summary>
	
- After performing CTS (with clock buffers) we can see that the slack is improved but it is not met.
As we can see in below images the slack is not metfor setup and hold.<br>
<img width="800" alt="1.setup(violate)_report_timing" src="https://github.com/Sidv005/Samsung-PD-Training/blob/dec2794113140a2ddf511b622515587b4b09e94f/day24/1.setup(violate)_report_timing.png"><br>
<img width="800" alt="2.setup(violate)_report_timing2" src="https://github.com/Sidv005/Samsung-PD-Training/blob/dec2794113140a2ddf511b622515587b4b09e94f/day24/2.setup(violate)_report_timing2.png"><br>
<img width="800" alt="3.hold(violate)_report_timing" src="https://github.com/Sidv005/Samsung-PD-Training/blob/dec2794113140a2ddf511b622515587b4b09e94f/day24/3.hold(violate)_report_timing.png"><br>

- From above images we can observe that the slacks have significantly improved compared with the previous case without buffers.
- To meet the slack we upsize/downsize the cell as per the requirement.

The schematic of critical path fro setup violation is as follows:-<br>
<img width="800" alt="4.gui_setup%26hold(violate)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/dec2794113140a2ddf511b622515587b4b09e94f/day24/4.gui_setup%26hold(violate).png"><br>

Now we will try to fix the violation by changing the drive strength of the cell.

- Upsizing the cell will increase the drive strength of the cell which helps in reducing the delay.
- Upsizing the cell using the command *size_cell*

```ruby
  size_cell core1/U86 sky130_fd_sc_hd__fa_2
  size_cell core1/U77 sky130_fd_sc_hd__fah_2
  size_cell core1/U617 sky130_fd_sc_hd__xor2_4
  size_cell core1/U337 sky130_fd_sc_hd__fa_2
```
- Now we can observe setup slack is met as shown in below figure.<br>
<img width="800" alt="8.setup_slack_met" src="https://github.com/Sidv005/Samsung-PD-Training/blob/dec2794113140a2ddf511b622515587b4b09e94f/day24/8.setup_slack_met.png"><br>

- But the hold slack is not met. It is violating by a small margin of 6.7ps.

To meet the hold slack we will insert buffer in the critical path to increase the path delay.

```ruby
insert_buffer core1/CPU_src1_value_a3_reg[27]/D sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__buf_12
 report_timing -from core1/CPU_Xreg_value_a4_reg[8][27] -to core1/CPU_src1_value_a3_reg[27] -delay min
```
From the above command we can say that buffer of drive strength 12 (sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__buf_12) is inserted over "D" pin of core1/CPU_src1_value_a3_reg[27]. Later we can notice the min delay of the critical path (core1/CPU_Xreg_value_a4_reg[8][27] -->  core1/CPU_src1_value_a3_reg[27]).

<img width="800" alt="9.hold_met" src="https://github.com/Sidv005/Samsung-PD-Training/blob/dec2794113140a2ddf511b622515587b4b09e94f/day24/9.hold_met.png"><br>

- Now hold violations are fixed by a margin of 0.19ns as we can view in above figure.

***Comparing results before and after ECO***

- Now quality of report is checked and comapared. Below image is showing qor before ECO.

BEFORE:-<br>
<img width="800" alt="5.report_qor_violations" src="https://github.com/Sidv005/Samsung-PD-Training/blob/dec2794113140a2ddf511b622515587b4b09e94f/day24/5.report_qor_violations.png"><br>
<img width="800" alt="6.report_qor_violations2" src="https://github.com/Sidv005/Samsung-PD-Training/blob/dec2794113140a2ddf511b622515587b4b09e94f/day24/6.report_qor_violations2.png"><br>

AFTER:-<br>
<img width="800" alt="10.report_qor_slack_met" src="https://github.com/Sidv005/Samsung-PD-Training/blob/dec2794113140a2ddf511b622515587b4b09e94f/day24/10.report_qor_slack_met.png"><br>
<img width="800" alt="11.report_qor_slack_met2" src="https://github.com/Sidv005/Samsung-PD-Training/blob/dec2794113140a2ddf511b622515587b4b09e94f/day24/11.report_qor_slack_met2.png"><br>

- After comparison we can observe that Cell area is incresed from 700854.13 microns to 700890.42 microns.
- We can view that max trans and max Cap are still violating by 4 and 1 repectively.
- Below command shows the total violations present in the design.

```ruby
report_constraints -max_transition -all_violators
```

- Fixing the trans violations is done by upsizing the cell in order to reduce the transition time.
- The cell which is driving a particular net having high transition time is needed to get higher drive strength. We can identify that specific driving cell by using below command.

```ruby
report_timing -through core1/HFSNET_4
```
where core1/HFSNET_4 is a net name.

- Below commands are also used to remove the max cap violations as well.

```ruby
size_cell core1/gre_mt_inst_2848 sky130_fd_sc_hd__clkbuf_2
size_cell core1/HFSINV_1403_5 sky130_fd_sc_hd__inv_4
size_cell core1/ctmTdsLR_1_2523 sky130_fd_sc_hd__clkinv_4
size_cell core1/HFSINV_264_47 sky130_fd_sc_hd__clkinv_4
```
- Now we can say that above commands are applied to remove max trans and max cap violations. 
- Command used for displaying max cap violation status is given below.

```ruby
report_constraints -max_capacitance -all_violators
```
Below image shows the trans violation status.<br>
<img width="800" alt="14.no_trans_violations" src="https://github.com/Sidv005/Samsung-PD-Training/blob/dec2794113140a2ddf511b622515587b4b09e94f/day24/14.no_trans_violations.png"><br>
Below image shows the cap violation status.<br>
<img width="800" alt="15.no_cap_violations" src="https://github.com/Sidv005/Samsung-PD-Training/blob/dec2794113140a2ddf511b622515587b4b09e94f/day24/15.no_cap_violations.png"><br>

- Both max trans and max cap are nox fixed.

**Impact of DECAP cells**
We added Decap cells to observe the impact on power. Above commands are added in top.tcl file.

```ruby
set FILLER_CELLS [get_object_name [sort_collection -descending [get_lib_cells sky130_fd_sc_hd__fill* sky130_fd_sc_hd__decap*] area]]
```
Image of top.tcl is shown below.<br>
<img width="800" alt="16.top.tcl_decaps" src="https://github.com/Sidv005/Samsung-PD-Training/blob/266646611844e56ef4347b5ee740860bda3a783e/day24/16.top.tcl_decaps.png"><br>

- Now power report is compared.

BEFORE:-<br>
<img width="800" alt="7.report_power_violate" src="https://github.com/Sidv005/Samsung-PD-Training/blob/dec2794113140a2ddf511b622515587b4b09e94f/day24/7.report_power_violate.png"><br>

AFTER:-<br>
<img width="800" alt="2.report_power_dcap_fixed_violations" src="https://github.com/Sidv005/Samsung-PD-Training/blob/266646611844e56ef4347b5ee740860bda3a783e/day24/2.report_power_dcap_fixed_violations.png"><br>

From the above images we can conclude that power is getting increased from 4.31e+06 nW to 4.34e+06 nW since high drive strength, buffers and Decap cells are utilized in the design. 

Schematic of DECAP cell is shown below.<br>
<img width="800" alt="gui_dcap" src="https://github.com/Sidv005/Samsung-PD-Training/blob/ab56eca941f802a306363ae5c3f15ca09a5b07f6/day24/gui_dcap.png"><br>
</details>


## Day 26 Introduction to Mixed signal flow ##

<details>
 <summary>Theory</summary>

**Mixed Signal Design**
In the context of integrated circuits (ICs), mixed-signal design refers to the design and integration of both analog and digital circuitry on a single semiconductor chip. This is often done to create complex systems-on-a-chip (SoCs) that can perform a wide range of functions, combining the capabilities of analog and digital components. Here's a more specific explanation of mixed-signal design in the context of ICs:

- Analog and Digital Integration:
Mixed-signal ICs combine analog and digital components on the same chip. Analog components might include amplifiers, analog-to-digital converters (ADCs), and oscillators, while digital components could be microcontrollers, processors, memory, and digital logic.

- Functionality:
These ICs are designed to perform a wide variety of tasks that require both analog and digital processing. For example, they may be used in applications like data acquisition, signal processing, communication, and control systems, where analog sensors or signals need to be processed, digitized, and then acted upon.

- A/D and D/A Conversion:
Analog-to-digital converters (ADCs) are often a crucial part of mixed-signal ICs. They convert real-world analog signals into digital data that can be processed by the digital components on the chip.
Conversely, digital-to-analog converters (DACs) are used when the IC needs to convert digital data back into analog signals for output or control purposes.

- Digital Signal Processing:
Mixed-signal ICs may include digital signal processing (DSP) blocks that manipulate and analyze the digitized analog data. This can involve filtering, modulation, control algorithms, and more.

- Real-world Interfaces:
These ICs often provide interfaces for connecting with external analog components, sensors, or actuators, bridging the gap between the digital world of the IC and the real-world analog environment.

- Power Management:
ICs designed for mixed-signal applications often include analog components for power management, voltage regulation, and efficient power conversion to ensure stable and reliable operation of the digital components.

- Noise and Signal Integrity:
Ensuring good signal integrity and minimizing noise is critical in mixed-signal IC design because noise can disrupt analog signals and affect the quality of converted data.

- Mixed-signal IC design is crucial in various applications, including:
1. Data converters: ICs that convert analog signals to digital (ADCs) or digital to analog (DACs).
2. Microcontrollers and SoCs: These chips often include both analog and digital components, enabling a wide range of functions in one package.
3. Communication ICs: For wireless communication, where analog RF components interface with digital data processing.
4. Audio ICs: Such as audio codecs, amplifiers, and processing units used in audio equipment and consumer electronics.
5. Sensor interfaces: ICs that interface with various sensors like temperature, pressure, and motion sensors.
 
Designing mixed-signal ICs is highly specialized and requires a deep understanding of both analog and digital circuit design, as well as semiconductor fabrication processes. Engineers aim to create ICs that perform efficiently while minimizing power consumption, noise, and other factors that can affect overall system performance.

**AMS**

In the context of electronics and integrated circuit (IC) design, "Analog and Mixed-Signal" (AMS) refers to a specialized field that focuses on the design, analysis, and testing of both analog and mixed-signal circuits and systems

Key aspects of Analog and Mixed-Signal (AMS) design include:

1. Analog Circuit Design: This involves designing circuits that handle analog signals, taking into consideration factors such as signal integrity, noise, and power consumption.

2. Digital Circuit Design: AMS engineers must also design digital components for tasks like signal processing, control, and interfacing with other digital systems.

3. Analog-to-Digital Conversion (ADC): Converting real-world analog signals into digital data is a common requirement in AMS design.

4. Digital-to-Analog Conversion (DAC): In some cases, digital data needs to be converted back into analog form for output or control purposes.

5. Real-World Interfaces: AMS circuits often provide interfaces for connecting with external analog components, sensors, and actuators.

6. Power Management: Efficient power management and voltage regulation are essential to ensure the proper operation of both analog and digital components.

**Files used for mixed signal design**

1. Library file:-
 A ".lib" file, or library file, is a vital component that stores comprehensive data about standard cells, often referred to as library cells or cell models. These standard cells serve as the foundational components used in designing digital integrated circuits.

- Inside the ".lib" file, you'll find extensive details about these library cells, which are pre-designed and reusable digital logic elements. These cells encompass fundamental logic gates like AND, OR, and NOT gates, as well as more complex components like flip-flops, latches, multiplexers, adders, and other essential building blocks used in digital circuit design.

2. Library Exchange Format:-
- A "LEF" file, short for "Library Exchange Format," serves as a standardized file format crucial for representing the physical characteristics of library cells, often called standard cells. These files are pivotal in the physical design and arrangement of integrated circuits.

- LEF files primarily house the definitions of standard cells that form the fundamental building blocks of digital logic within a microchip.

- Within LEF files, you'll find critical physical details about standard cells, such as their precise dimensions, pin placements, and the specific layers used in the chip manufacturing process. This information is essential for creating the physical layout of the integrated circuit.

- LEF files also outline the layers utilized during semiconductor fabrication, including materials, metal interconnections, vias, and other physical attributes relevant to the chip's construction.

3. Timing File
- A ".tf" file, commonly known as a timing file, holds vital data regarding timing constraints and delays within a design. It precisely defines timing attributes like input and output delays, setup times, hold times, clock-to-Q delays, and more.

- Timing files are of utmost importance, providing crucial insights into the timing characteristics and constraints of the digital components within an integrated circuit (IC).

- These files play a pivotal role in static timing analysis, ensuring that the design adheres to its performance and timing requirements.

- Throughout the design process, timing files find application in various stages, including synthesis, static timing analysis, and physical design, where they guide the accurate timing performance of the integrated circuit.

4. Transfer Function Lookup Table File
- A ".tlu" file commonly stores lookup tables that specify the performance characteristics of specific digital or "analog" components, like memory cells, logical operations, or transfer functions for analog devices.

- These files are essential for modeling and simulating the behavior of particular components or blocks within a design, enabling engineers to understand and analyze how these components function in a broader system.
</details>

## Day-27 Introduction to crosstalk glitch and delay ##
<details>
 <summary>Cross talk noise and reasons</summary>
	
- Crosstalk is the unwanted interference or signal coupling that occurs between neighboring conductive paths on an integrated circuit (IC) or chip. Very Large-Scale Integration (VLSI) design aims to densely pack numerous components and interconnections into a limited physical space, raising concerns about electrical interference issues, with crosstalk being a major issue. Crosstalk can have adverse effects on the performance, reliability, and functionality of VLSI circuits.

- For instance, consider a circuit used for sending and receiving messages. In the past, only one or two instances of this circuit may have been operating within the same area. However, with the reduction in the size of MOSFETs (Metal-Oxide-Semiconductor Field-Effect Transistors), now nine instances of this circuit can coexist in the same chip area. These instances can be engaged in a variety of activities, such as sending and receiving messages, handling calls, processing data, and running other applications concurrently.

- In summary, the shrinking of MOSFET size has enabled a significant increase in the number of applications running in a confined space on the chip, leading to the potential for increased crosstalk and interference challenges in VLSI design.

- Reducing the size of components in very advanced processes, particularly in those below 0.1 micrometers, can introduce interference issues, as illustrated in the figure below. This interference primarily occurs when two closely spaced nets or wires are in operation, leading to the main cause of crosstalk.

- Initially, there are 20 standard cells within the design. However, as the size is decreased, the number of standard cells increases by a factor of 9. These additional cells need to be interconnected, resulting in a significant rise in the number of routes and bringing them into close proximity.

- Consequently, this increased routing density can lead to design failures, where functionality issues arise, often referred to as crosstalk. This is attributed to the proximity of closely routed signals interfering with one another, affecting the intended operation of the circuit.

<img width="800" alt="crosstalk1" src="https://github.com/Sidv005/Samsung-PD-Training/blob/818cd5c1fbd6563a21b627a86ac29816f5da7ed8/day27/crosstalk1.PNG"><br>
</details>

<details>
 <summary>Dominant Lateral Capacitance</summary>
 Increase in number of metal layers resulting in increase in lateral capacitance is also one of the reason for increase in cross talk

- Why increasing lateral capacitance leads to increase in metal layer?

->Breaking into several metal layers helps in reducing the resistance where the higher the area, resulting in lower resistance. That's why we are having a wider metal layer.

->The overlap area between metal 1 and metal 2 as shown in the figure below, is pretty huge, that leads into an increase in interlayer capacitance. That's why 0.25 um and above process, we say that the interlayer capacitance was dominant.

<img width="800" alt="crosstalk2" src="https://github.com/Sidv005/Samsung-PD-Training/blob/818cd5c1fbd6563a21b627a86ac29816f5da7ed8/day27/crosstalk2.PNG"><br>

- Reducing the size of MOSFETs leads to an expansion in the number of standard cells, consequently increasing the number of connections required. Each cell must be linked to the edges of the standard cells, which elevates the connection density. This, in turn, results in a notable increase in the number of routing paths required to establish these connections.
- Due to the close proximity of routes and the challenge of accommodating the MOSFET area, reducing the width of the metal is often considered. However, even with a narrower metal width, the demand for routing area remains exceedingly high. Thus, simply reducing the width is insufficient to address this significant demand.
- So, we need to do the connections in different way (i.e. referring to the figure below) which is making the signal travelling in a straight line (only travelling across metal 1) without transferring the signal to metal 3 first. This is happened because of the limited amount of resources/routing resources available in the area. In this case, the amount of area is very compact and we need to accommodate it where we have to connect signals at any cost.

<img width="800" alt="crosstalk3" src="https://github.com/Sidv005/Samsung-PD-Training/blob/818cd5c1fbd6563a21b627a86ac29816f5da7ed8/day27/crosstalk3.PNG"><br>
</details>

<details>
 <summary>Noise Margin</summary>
	
 - Noise margin in Very Large-Scale Integration (VLSI) design is a critical concept used to characterize the robustness and reliability of digital circuits in the presence of noise, variations, and uncertainties. It represents the amount of noise or voltage fluctuations that a digital circuit can tolerate while still correctly interpreting logic levels (high or low) and producing the expected output. Noise margin is typically expressed in terms of voltage levels and is crucial for ensuring the correct operation of digital circuits.
 
- There are two main components of noise margin:

1. High-Level Noise Margin (NMH): NMH represents the maximum allowable noise on the high logic level (logical '1') before the circuit interprets it as a low logic level (logical '0'). In other words, it quantifies the resilience of the circuit against noise that might pull a high voltage down to the low level.

2. Low-Level Noise Margin (NML): NML represents the maximum allowable noise on the low logic level (logical '0') before the circuit interprets it as a high logic level (logical '1'). It measures the resilience of the circuit against noise that might push a low voltage up to the high level.

The key idea is that a digital circuit should have a sufficient gap or margin between its high and low voltage levels to account for variations in operating conditions, component tolerances, and external noise sources.

Noise margin is particularly important in VLSI design for several reasons:

- Reliability: It ensures that circuits are robust against variations in voltage, temperature, and manufacturing processes, which can affect the voltage levels.

- Interference and Crosstalk: Noise margin helps in designing circuits that can withstand interference and crosstalk between adjacent signal lines.

- Power Consumption: By maintaining adequate noise margins, designers can minimize the chances of false transitions and reduce power consumption.

- Manufacturing Variability: VLSI chips often have variations in transistor characteristics and other factors due to the manufacturing process. Noise margin helps account for these variations.

- Operational Variability: Voltage levels can fluctuate due to factors like power supply fluctuations and noise from other components on the chip. Noise margin ensures that the circuit can still function correctly under such conditions.

<img width="800" alt="crosstalk4" src="https://github.com/Sidv005/Samsung-PD-Training/blob/818cd5c1fbd6563a21b627a86ac29816f5da7ed8/day27/crosstalk4.PNG"><br>

Noise margin depends on several factors, including:

- Power Supply Voltage: Variations in the power supply voltage can directly impact the noise margin. A higher power supply voltage often leads to larger noise margins.

- Threshold Voltage Levels: The noise margin is related to the logic threshold levels, which determine the voltage ranges for logical high and low levels.

- Process Variations: Process variations in semiconductor manufacturing can affect transistor characteristics, leading to variations in logic thresholds and, consequently, noise margin.

- Temperature: Temperature fluctuations can also influence the noise margin by affecting transistor characteristics.
</details>

<details>
 <summary>LABS</summary>

 In ICC2_shell following commands are used to write spef of vsdbabysoc.
 ```ruby
update_timing
write_parasitics -format spef -output vsdbabysoc_spef
```
Below screenshot shows the execution.<br>
<img width="800" alt="1.write_spef" src="https://github.com/Sidv005/Samsung-PD-Training/blob/60f4b3f8a87f3a8981fc80a9af72cdde92445993/day27/1.write_spef.png"><br>

- Then we need to extract the zip file containing the synthesized netlist using *gzip -d*.
- Now pt_shell is invoked and further process is done in pt_shell.

```ruby
csh
pt_shell
```

In pt_shell

```ruby
set target_library "<location of avsddac.db> <location of avsdpll.db> <location of sky130_fd_sc_hd__tt_025C_1v80.db>"
set link_library [list  <location of avsddac.db> <location of avsdpll.db> <location of sky130_fd_sc_hd__tt_025C_1v80.db>]
read_verilog <location of the synthesized netlist>
link_design
current_design
```

<img width="800" alt="2.set_tar_link" src="https://github.com/Sidv005/Samsung-PD-Training/blob/60f4b3f8a87f3a8981fc80a9af72cdde92445993/day27/2.set_tar_link.png"><br>

<img width="800" alt="3.link_design" src="https://github.com/Sidv005/Samsung-PD-Training/blob/60f4b3f8a87f3a8981fc80a9af72cdde92445993/day27/3.link_design.png"><br>

- Then we need to provide sdc file and spef file

```ruby
read_sdc <location of .sdc>
set_app_var si_enable_analysis true
read_parasitics -keep_capacitive_coupling <location of spef>
```
<img width="800" alt="4.read_parasitic" src="https://github.com/Sidv005/Samsung-PD-Training/blob/60f4b3f8a87f3a8981fc80a9af72cdde92445993/day27/4.read_parasitic.png"><br>

The schematic of the loaded design is shown below.<br>
<img width="800" alt="9.schematic" src="https://github.com/Sidv005/Samsung-PD-Training/blob/60f4b3f8a87f3a8981fc80a9af72cdde92445993/day27/9.schematic.png"><br>

Below image displays the rvmyth core schematic.<br>
<img width="800" alt="8.rvmyth" src="https://github.com/Sidv005/Samsung-PD-Training/blob/60f4b3f8a87f3a8981fc80a9af72cdde92445993/day27/8.rvmyth.png"><br>

- Reports

```ruby
report_si_bottleneck              
report_bottleneck                 
report_si_delay_analysis
report_si_aggressor_exclusion
report_si_noise_analysis
```

- Execution of above commands are done which are shown below.<br>
<img width="800" alt="6.report_si.png" src="https://github.com/Sidv005/Samsung-PD-Training/blob/60f4b3f8a87f3a8981fc80a9af72cdde92445993/day27/6.report_si.png"><br>
<img width="800" alt="7.report_si.png" src="https://github.com/Sidv005/Samsung-PD-Training/blob/60f4b3f8a87f3a8981fc80a9af72cdde92445993/day27/7.report_si.png"><br>

- *report_qor* is executed as follows:
<img width="800" alt="5.qor.png" src="https://github.com/Sidv005/Samsung-PD-Training/blob/60f4b3f8a87f3a8981fc80a9af72cdde92445993/day27/5.qor.png"><br>

</details>

## Day-28 Introduction to DRC/LVS ##

<details>
 <summary>Theory</summary>

**Introduction to SkyWater PDKs and opensource EDA tools**

- SkyWater Open Source PDK is a joint project between Google and SkyWater Technology Foundry, where it provides a fully open source Process Design Kit (PDK), and its related resources.

- SkyWater open PDK public repository contains:
  
       - Documentation: https://skywater-pdk.readthedocs.io/en/main/
  
       - PDK Library and files: https://github.com/google/skywater-pdk
  
       - Community: https://invite.skywater.tools/

- "130" in SKY130 stands for the feature size, which is the length of smallest transistor that can be manufactured in the process.

**Physical Verification and Design Flow**

Physical verification is perfomed to check whether we have a mask layout that matches what we think the circuit should be.

There are 2 major steps in physical verification.

- Design Rule Checking (DRC) --> Verifies if layout satisfies rules required for manufacturing. Rules may vary from foundary to foundaryand for different technology will have different different rules. It ensures that the layout matches all the rules provided by the foundry for the specific process.

- Layout Vs. Schematic (LVS) --> It ensures that the layout netlist matches the schematic netlist. Usually extraction errors and comparison errors occurs during LVS stage. Extraction errors like short, open device extraction, missing device terminals, duplicate structure placement. Compare errors like ports are swapped, unmatched nets or devices or schematic.
</details>

<details>
 <summary>Lab</summary>

**Creating Sky130 Device Layout In Magic**

```ruby
cd /home/siddhant.v/Desktop
mkdir inverter
cd inverter
mkdir xschem
mkdir mag
mkdir netgen
```
<img width="1000" alt="1.mkdir.PNG" src="https://github.com/Sidv005/Samsung-PD-Training/blob/63d0273ac79243089b8db52bea1fa4c621ce5283/day28/1.mkdir.PNG"><br>

```ruby
cd xschem
ln -s /usr/share/pdk/sky130A/libs.tech/xschem/xschemrc
ln -s ln -s /usr/share/pdk/sky130A/libs.tech/ngspice/spinit .spiceinit
cd ../mag/
ln -s /usr/share/pdk/sky130A/libs.tech/magic/sky130A.magicrc .magicrc
cd ../netgen/
ln -s /usr/share/pdk/sky130A/libs.tech/netgen/sky130A_setup.tcl setup.tcl
cd inverter/xschem/
xschem
```
Above commands are used to link tools like xschem, netgen and magic.
<img width="1000" alt="2.ln%20-s.PNG" src="https://github.com/Sidv005/Samsung-PD-Training/blob/63d0273ac79243089b8db52bea1fa4c621ce5283/day28/2.ln%20-s.PNG"><br>

- This brings up a display for xschem with a lot of example schematics, SKY130 devices are shown in xschem as below.
- Note: Examples can be accessed by clicking the relevant rectangle and pressing the "E" key on the keyboard. We can return to the menu by pressing "CTRL+E". The "F" key resizes the schematic to fit the window.

<img width="800" alt="3.xschem.PNG" src="https://github.com/Sidv005/Samsung-PD-Training/blob/63d0273ac79243089b8db52bea1fa4c621ce5283/day28/3.xschem.PNG"><br>

<img width="800" alt="4.xschem2.PNG" src="https://github.com/Sidv005/Samsung-PD-Training/blob/63d0273ac79243089b8db52bea1fa4c621ce5283/day28/4.xschem2.PNG"><br>

```ruby
cd ../mag/
magic
magic -d XR     (To invoke a cairo graphics package that uses 3D acceleration to get better rendering than the default graphics)
magic -d -OGL   (An OpenGL based graphics package)
```

This brings up 2 magic windows, with the layout window displaying "Technology: sky130A", along with many colors and icons displaying the available layers in this technology, as shown below.
<img width="800" alt="5.magic.PNG" src="https://github.com/Sidv005/Samsung-PD-Training/blob/63d0273ac79243089b8db52bea1fa4c621ce5283/day28/5.magic.PNG"><br>

<img width="800" alt="6.nfet.PNG" src="https://github.com/Sidv005/Samsung-PD-Training/blob/63d0273ac79243089b8db52bea1fa4c621ce5283/day28/6.nfet.PNG"><br>

- Changing the device type to sky130_fd_pr__nfet_g5v0d10v5

<img width="800" alt="7.nfet_apply.PNG" src="https://github.com/Sidv005/Samsung-PD-Training/blob/63d0273ac79243089b8db52bea1fa4c621ce5283/day28/7.nfet_apply.PNG"><br>

**Creating Simple Schematic In Xschem**

```ruby
cd ../xschem/
xschem
```
Press "Insert" key to pop out Choose symbol window. Select the SkyWater library directory path to access SkyWater components and choose the fd_pr library. To create an inverter, a basic nfet and pfet are needed. Therefore, select nfet and pfet device from the insert window and place it anywhere in the schematic.


- As pins are not PDK specific, they can be found under the xschem library in the insert window. These are named as ipin.sym, opin.sym and iopin.sym.

- Press Q key to bring up the parameter window and Rename each pin to something sensible.

- Press Q key anfetr left click on component to bring up the parameter windows to configure the properties of the devices.

- For nfet, change the length to 0.18 from default value of 0.15 since its restricted to sram devices only. Set the number of fingers to 3, and the width of each finger to 1.5.

- Since we have 3 fingers now, the total width in the parameter window must be set to 3 times of the finger width, which is 4.5.

- Similarly, for pfet, adjust the parameters to 3 fingers, width of 1 per finger, and a length of 0.18. We must specify the body to be connected to the Vdd pin as it is a 3 pin pfet.

<img width="800" alt="8.nfet_prop.PNG" src="https://github.com/Sidv005/Samsung-PD-Training/blob/63d0273ac79243089b8db52bea1fa4c621ce5283/day28/8.nfet_prop.PNG"><br>

<img width="800" alt="9.pfet_prop.PNG" src="https://github.com/Sidv005/Samsung-PD-Training/blob/63d0273ac79243089b8db52bea1fa4c621ce5283/day28/9.pfet_prop.PNG"><br>

Save the design by clicking tab File --> save as --> inverter.sch

Schematic is shown in below image.<br>
<img width="800" alt="10.schematic.PNG" src="https://github.com/Sidv005/Samsung-PD-Training/blob/63d0273ac79243089b8db52bea1fa4c621ce5283/day28/10.schematic.PNG"><br>

**Creating Symbol And Exporting Schematic In Xschem**

- Testbench is created seperately to verify the functionality of 

- Firstly, create a symbol for the schematic as the schematic will appear as a symbol in the testbench. To do this, click on the Symbol menu and select "Make symbol from schematic". Then, create a testbench schematic using new schematic option and insert the generated symbol from the local directory using the Insert key.

- Select new schematic in File tab and choose inverter.sch under home directory and paste it on the schematic window.

- The testbench will be very simple where we will generate a ramp input and observe the output response after connecting the power supplies. To do this, insert 2 voltage sources from the default xschem library, one for the input and one for the supply. Connect these and add a GND node to the supply connections. Create "ipins" and "opins" for the input and output signals to observe in Ngspice.

- Supply voltage is set to 1.8 V. For the input voltage, we must set the supply to a piece-wise linear function to get ramp. PWL function has voltage and time values stated that the supply will start at 0v, then start to ramp up from 20 ns till it reaches its final value at 900 ns of 1.8 V.

- Next, place two more statements for ngspice, but as these aren't specific to any component, they must be placed in text boxes. To place a text box, select the code_shown.sym component under the xschem library.

- The first text box will specify the location of the device models used in the device schematic, where it is using a .lib statement that selects a top level file that tells ngspice where to find all the models and also specifying a simulation corner for all the models. The first block specifying the typical corner with *value = ".lib /usr/share/pdk/sky130A/libs.tech/ngspice/sky130.lib.spice tt"*.

- For the second block, it specifies;

```ruby
value = ".control
tran 1n 1u
plot V(in) V(out)
.endc"
```
This will tell ngspice to run a transient simulation for 1 ns and monitor voltages for the in and out pins. Therefore, a complete testbench schematic is shown as below, and save this as inverter_tb.sch<br>
<img width="800" alt="11.tb_inverter_symbol.PNG" src="https://github.com/Sidv005/Samsung-PD-Training/blob/63d0273ac79243089b8db52bea1fa4c621ce5283/day28/11.tb_inverter_symbol.PNG"><br>

- To generate the netlist, click on the Netlist button, then simulate it in Ngspice by clicking the Simulate button.

- The waveform confirms that the schematic behaves as an inverter as shown below.

<img width="800" alt="12.plot.PNG" src="https://github.com/Sidv005/Samsung-PD-Training/blob/63d0273ac79243089b8db52bea1fa4c621ce5283/day28/12.plot.PNG"><br>

- After verifying the schematic, layout needs to be created. To do this, go back to the inverter schematic.

- Firstly, click on the Simulation menu and select "LVS netlist: Top Lvel is a .subckt" option.

- Wait for a while and go to the Simulation menu to check whether a tick mark appears or not. This verifies if we have properly defined a sub circuit for creating a layout cell with pins in the layout.

- A netlist is generated successfully for the schematic by clicking the Netlist button and quit Xschem.

**Importing Schematic To Layout And Inverter Layout Steps**

```ruby
cd ../mag/
magic -d XR
```

 Run the magic, then click on File -> Import SPICE and then select the inverter.spice file from the xschem directory. If done correctly, the following layout has been opened up in magic.
 
<img width="800" alt="13.magic(1)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/63d0273ac79243089b8db52bea1fa4c621ce5283/day28/13.magic(1).PNG"><br>

- Referring to the layout generated above, the schematic import is unaware about analog placing and routing as it is very complex. Therefore, We must place them in the best positions and wire them up manually.

- Now, place the pfet device above the nfet and adjust the placement of the input, output and supply pins. Refer below figure.

<img width="800" alt="14.magic2.PNG" src="https://github.com/Sidv005/Samsung-PD-Training/blob/63d0273ac79243089b8db52bea1fa4c621ce5283/day28/14.magic2.PNG"><br>

- Next, set some parameters that are only adjustable in the layout which will make it more convenient to wire the whole layout up.

- To pop out the parameter editing section, use S key and press I key to select the object, then use CTRL+P to open up the parameter options for the selected device.

- Start to paint the wires using metal1 layers by connecting the source of the pfet to Vdd and source of the nfet to Vss. Next, connect the drains of both mosfets to the output. Finally, connect the input to all the poly contacts of the gate.

<img width="800" alt="15.magic3.PNG" src="https://github.com/Sidv005/Samsung-PD-Training/blob/63d0273ac79243089b8db52bea1fa4c621ce5283/day28/15.magic3.PNG"><br>

Below image is obtained after fixing DRC errors.<br>
<img width="800" alt="16.magic_drc.PNG" src="https://github.com/Sidv005/Samsung-PD-Training/blob/63d0273ac79243089b8db52bea1fa4c621ce5283/day28/16.magic_drc.PNG"><br>

Save the file and Run following commands in magic console.

```ruby
extract do local    (Ensuring that magic writes all results to the local directory)
extract all         (Performing the actual extraction)
ext2spice lvs       (Simulating and setting up the netlist to hierarchical spice output in ngspice format with no parasitic components)
ext2spice           (Generating the spice netlist)
```
<img width="1000" alt="17.ext2spice%20lvs.PNG" src="https://github.com/Sidv005/Samsung-PD-Training/blob/63d0273ac79243089b8db52bea1fa4c621ce5283/day28/17.ext2spice%20lvs.PNG"><br>

```ruby
rm *.ext                                          (Clear any unwanted files -> .ext files are just intermediate results from the extraction)
/usr/share/pdk/bin/cleanup_unref.py -remove .     (Clean up extra .mag files -> files containing paramaterised cells that were created and saved but not used in the design)
netgen -batch lvs "../mag/inverter.spice inverter" "../xschem/inverter.spice inverter"    (Run LVS by entering the netgen subdirectory)
```

- Remember to always use the layout netlist first and schematic netlist second in the netgen command as in side by side, resulting the layout is on the left and the schematic is on the right.

- Each netlist is represented by a pair of keywords in quotes, where the first is the location of the netlist file and the second is the name of the subcircuit to compare.

<img width="1000" alt="18.remove.png" src="https://github.com/Sidv005/Samsung-PD-Training/blob/3bdda15570df7355490ad026d10df34c4f8f6aa4/day28/18.remove.png"><br>

<img width="1000" alt="19.lvs_done.PNG" src="https://github.com/Sidv005/Samsung-PD-Training/blob/3bdda15570df7355490ad026d10df34c4f8f6aa4/day28/19.lvs_done.PNG"><br>

Modify the test bench netlist file.<br>
<img width="1000" alt="20.tb_inverter_spice.PNG" src="https://github.com/Sidv005/Samsung-PD-Training/blob/3bdda15570df7355490ad026d10df34c4f8f6aa4/day28/20.tb_inverter_spice.PNG"><br>

```ruby
cp ../xschem/.spiceinit .
ngspice inverter_tb.spice
```
The result is almost the same as in previous simulation in xschem as shown below.

<img width="1000" alt="12.plot.PNG" src="https://github.com/Sidv005/Samsung-PD-Training/blob/3bdda15570df7355490ad026d10df34c4f8f6aa4/day28/12.plot.PNG"><br>
</details>



## Day 30 - Introduction to TCL WORKSHOP ##

<details>
 <summary>Introduction to TCL and VSDSYNTH Toolbox Usage</summary>

Task is to create a command (in my case, ***synui***) and pass a .csv file from the UNIX shell to the TCL script, taking into consideration mainly three general scenarios from the user's point of view.

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/979775914611d25ed4101edafc8de4ac5bcb0139/day30/p1.PNG)

**Review of input file - openMSP430_design_details.csv**

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/979775914611d25ed4101edafc8de4ac5bcb0139/day30/p2.PNG)


### Implementation

Creation of the *synui* command script and *synui.tcl* files.

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/979775914611d25ed4101edafc8de4ac5bcb0139/day30/p3.PNG)


*synui Code*
![image](https://github.com/Sidv005/Samsung-PD-Training/blob/979775914611d25ed4101edafc8de4ac5bcb0139/day30/p4.PNG)



The basic structure of bash code used for the implementation of general scenarios is shown below.

```bash
#Code to handle the scenario where user does not give any file, does not give .csv file, gives more than one file as argument

if [ $# -eq 0 ]
then
        echo "Info: Please provide a CSV file"
        exit 1
elif [ $# -gt 1 ]
then
        echo "Info: Please provide only 1 CSV file"
        exit 1
else
        if [[ $1 != *.csv  &&  $1 != "-help" ]]
        then
                echo "Info: Please provide a .csv format file"
                exit 1
        fi
fi
# Code to check if the .csv file is present in directory or not, and also to display information for -help argument.
if [ ! -f $1 ] || [ $1 == "-help" ]
then
        if [ $1 != "-help" ]
        then
                echo "Error: The file $1 is not found in current directory."
                exit 1
        else
                echo "USAGE: ./synui <csv_file>"
                echo
                echo " where <csv file> consists of 2 columns, below keyword being in 1st column and is Case Sensitive. Please request Niharika for sample csv file."
                echo
                echo " <Design Name> is the name of top level module."
                echo
                echo " <Output Directory> is the name of output directory where you want to dump synthesis script, synthesized netlist and timing reports."
                echo
                echo " <Netlist Directory> is the name of directory where all RTL netlist are present."
                echo
                echo " <Early Library Path> is the file path of the early cell library to be used for STA."
                echo
                echo " <Late Library Path> is file path of the late cell library to be used for STA."
                echo
                echo " <Constraints file> is csv file path of constraints to be used for STA."
                exit 1
        fi
else
        #Code to execute if the proper CSV file exists.
        echo "Info: CSV file accepted"
        tclsh synui.tcl $1
fi
```

In my command ***synui***, I have implemented a total of *5 general scenarios* from the user's point of view in the bash script.

#### 1. No input file provided

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/979775914611d25ed4101edafc8de4ac5bcb0139/day30/p5.PNG)


#### 2. File provided exists but is not of .csv format

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/979775914611d25ed4101edafc8de4ac5bcb0139/day30/p6.PNG)


#### 3. More than one file or parameters provided

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/979775914611d25ed4101edafc8de4ac5bcb0139/day30/p7.PNG)


#### 4. Provide a .csv file that does not exist

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/979775914611d25ed4101edafc8de4ac5bcb0139/day30/p8.PNG)


#### 5. Type "-help" to find out usage

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/979775914611d25ed4101edafc8de4ac5bcb0139/day30/p9.PNG)
</details>

<details>
 <summary> Variable Creation and Processing Constraints from CSV</summary>
	
Task is to create variables, check file/directory existence, and convert constraints csv file to format[1] and SDc format. This is done by writing the code in *synui.tcl*.

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/979775914611d25ed4101edafc8de4ac5bcb0139/day30/p10.PNG)


**Review of input file - openMSP430_design_constraints.csv**

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/979775914611d25ed4101edafc8de4ac5bcb0139/day30/p11.PNG)


### Implementation

I have successfully completed tasks, namely variable creation, file and directory existence checks, and the processing of the constraints csv file.

**synui.tcl snapshot**

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/979775914611d25ed4101edafc8de4ac5bcb0139/day30/p12.PNG)


#### Variable Creation

I have auto-created the variables (*have used special condition to identify design name*) from the csv file by converting it into a matrix and then to an array (*also added command to capture the start time of the script so that it can be used to calculate runtime at the end*). 

*Code*

```tcl
#!/bin/tclsh

set start_time [clock clicks -microseconds]
set csv_design [lindex $argv 0]

package require csv
package require struct::matrix

struct::matrix m

set f [open $csv_design]

csv::read2matrix $f m , auto

close $f

set n_columns [m columns]
set n_rows [m rows]

puts "\nInfo:Variable values"
puts "No. of rows =  $n_rows"
puts "No. of columns = $n_columns"

m link csv_arr

set i 0
while {$i < $n_rows} {
        puts "\nInfo: Setting $csv_arr(0,$i) as '$csv_arr(1,$i)'"
        if { ![string match "*/*" $csv_arr(1,$i)] && ![string match "*.*" $csv_arr(1,$i)] } {
                        set [string map {" " "_"} $csv_arr(0,$i)] $csv_arr(1,$i)
        } else {
                set [string map {" " "_"} $csv_arr(0,$i)] [file normalize $csv_arr(1,$i)]
        }
        set i [expr {$i+1}]
}


```

*Screenshot*

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/979775914611d25ed4101edafc8de4ac5bcb0139/day30/p12.PNG)


#### File / Directory Existence Check

Since the existence of these files and directories is essential to the program's operation, I have built code to check for their existence. If the input files do not exist, we exit from the code except for output directory in which case it  is created. Below are screenshots of the terminal displaying the functionality and the basic code for the same.

*Code*

```tcl
############# FILE EXISTENCE CHECK ###################
# IF the directory does not exist, then create one 


if { ![file isdirectory $Output_Directory] } {
        puts "\nInfo: Cannot find output directory $Output_Directory. Creating $Output_Directory"
        file mkdir $Output_Directory
} else {
        puts "\nInfo: Output directory found in path $Output_Directory"
}

# Checking if netlist directory exists if not exits
if { ![file isdirectory $Netlist_Directory] } {
        puts "\nError: Cannot find RTL netlist directory in path $Netlist_Directory. Exiting..."
        exit
} else {
        puts "\nInfo: RTL netlist directory found in path $Netlist_Directory"
}

# Checking if early cell library file exists if not exits
if { ![file exists $Early_Library_Path] } {
        puts "\nError: Cannot find early cell library in path $Early_Library_Path. Exiting..."
        exit
} else {
        puts "\nInfo: Early cell library found in path $Early_Library_Path"
}

# Checking if late cell library file exists if not exits
if { ![file exists $Late_Library_Path] } {
        puts "\nError: Cannot find late cell library in path $Late_Library_Path. Exiting..."
        exit
} else {
        puts "\nInfo: Late cell library found in path $Late_Library_Path"
}

# Checking if constraints file exists if not exits
if { ![file exists $Constraints_File] } {
        puts "\nError: Cannot find constraints file in path $Constraints_File. Exiting..."
        exit
} else {
        puts "\nInfo: Constraints file found in path $Constraints_File"
}


```

*Screenshots*

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/979775914611d25ed4101edafc8de4ac5bcb0139/day30/p14.PNG)

#### Processing of the constraints openMSP430_design_constraints.csv file

The file was successfully analyzed and turned into a matrix. The beginning rows of the clocks, inputs, and outputs were also extracted, along with the rows and columns count. Below are the basic code for the same and a screenshot of the terminal showing many "puts" writing the variables.

*Code*

```tcl
# Constraints csv file data processing for convertion to format[1] and SDC
# ------------------------------------------------------------------------
puts "\nInfo: Dumping SDC constraints for $Design_Name"
::struct::matrix m1
set f1 [open $Constraints_File]
csv::read2matrix $f1 m1 , auto
close $f1
set n_rows_concsv [m1 rows]
set n_columns_concsv [m1 columns]
# Finding row number starting for CLOCKS section
set clocks_start_row [lindex [lindex [m1 search all CLOCKS] 0] 1]
# Finding column number starting for CLOCKS section
set clocks_start_column [lindex [lindex [m1 search all CLOCKS] 0] 0]
# Finding row number starting for INPUTS section
set inputs_start [lindex [lindex [m1 search all INPUTS] 0] 1]
# Finding row number starting for OUTPUTS section
set outputs_start [lindex [lindex [m1 search all OUTPUTS] 0] 1]

puts "\nInfo: Listing value of variables for user debug"
puts "Number of rows in CSV file = $n_rows_concsv"
puts "Number of columns in CSV file = $n_columns_concsv"
puts "CLOCKS starting row in CSV file = $clocks_start_row"
puts "CLOCKS starting column in CSV file = $clocks_start_column"
puts "INPUTS starting row in CSV file = $inputs_start "
puts "OUTPUTS starting row in CSV file = $outputs_start "

```

*Screenshot*

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/27c7bbc2898276942cd24a2fda07c5f60b68a23e/day30/p16.PNG)

</details>

<details>
 <summary> Processing Clock and Input Constraints from CSV and dumping SDC</summary>

The assignment is to essentially to analyze clock and input constraints in a CSV file and output SDC commands into a .sdc file with the actual processed data. In addition to a number of matrix search algorithms, it also uses an algorithm to distinguish between inputs that are buses and bits.

**Review of input file - openMSP430_design_constraints.csv**

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/27c7bbc2898276942cd24a2fda07c5f60b68a23e/day30/p17.PNG)

### Implementation
Tasks are succesfully complete i.e. To process constraints in a csv file for clocks and inputs and dump SDC commands into a .sdc file with actual processed data.

#### Processing of the constraints .csv file for CLOCKS and dumping SDC commands to .sdc

The csv file containing the CLOCKS data has been successfully processed, and clock-based SDC commands (*with distinct clock names by appending "_synyui" to the SDC create_clock command*) have been dumped into the.sdc file. Below are screenshots of the terminal with many "puts" spitting out the variables, user debug information, and output.sdc, along with the basic code for the same.

*Code*

```tcl
##############################################################################################
################### Day 3 ###################################################################
# Conversion of constraints csv file to SDC
# -----------------------------------------
# CLOCKS section
# Finding column number starting for clock latency in CLOCKS section
#
#puts "$n_columns_concsv"
set clk_erd_st_col [lindex [lindex [m1 search rect $clocks_start_column $clocks_start_row [expr { $n_columns_concsv - 1}] [expr {$inputs_start-1}] early_rise_delay] 0 ] 0 ]
set clk_efd_st_col [lindex [lindex [m1 search rect $clocks_start_column $clocks_start_row [expr { $n_columns_concsv - 1}] [expr {$inputs_start-1}] early_fall_delay] 0 ] 0 ]
set clk_lrd_st_col [lindex [lindex [m1 search rect $clocks_start_column $clocks_start_row [expr { $n_columns_concsv - 1}] [expr {$inputs_start-1}] late_rise_delay] 0 ] 0 ]
set clk_lfd_st_col [lindex [lindex [m1 search rect $clocks_start_column $clocks_start_row [expr { $n_columns_concsv - 1}] [expr {$inputs_start-1}] late_fall_delay] 0 ] 0 ]

# Finding column number starting for clock transition in CLOCKS section
#

set clk_ers_st_col [lindex [lindex [m1 search rect $clocks_start_column $clocks_start_row [expr { $n_columns_concsv - 1}] [expr {$inputs_start-1}] early_rise_slew] 0 ] 0 ]
set clk_efs_st_col [lindex [lindex [m1 search rect $clocks_start_column $clocks_start_row [expr { $n_columns_concsv - 1}] [expr {$inputs_start-1}] early_fall_slew] 0 ] 0 ]
set clk_lrs_st_col [lindex [lindex [m1 search rect $clocks_start_column $clocks_start_row [expr { $n_columns_concsv - 1}] [expr {$inputs_start-1}] late_rise_slew] 0 ] 0 ]
set clk_lfs_st_col [lindex [lindex [m1 search rect $clocks_start_column $clocks_start_row [expr { $n_columns_concsv - 1}] [expr {$inputs_start-1}] late_fall_slew] 0 ] 0 ]

# Finding column number starting for frequency and duty cycle in CLOCKS section only
set clk_freq_st_col [lindex [lindex [m1 search rect $clocks_start_column $clocks_start_row [expr { $n_columns_concsv - 1}] [expr {$inputs_start-1}] frequency] 0 ] 0 ]
set clk_dc_st_col [lindex [lindex [m1 search rect $clocks_start_column $clocks_start_row [expr { $n_columns_concsv - 1}] [expr {$inputs_start-1}] duty_cycle] 0 ] 0 ]

# Creating .sdc file with design name in output directory and opening it in write mode
#
set sdc_file [open $Output_Directory/$Design_Name.sdc "w"]

# Setting variables for actual clock row start and end
#
set i [expr {$clocks_start_row+1}]
set end_of_clocks [expr {$inputs_start-1}]

puts "\nInfo-SDC: Working on clock constraints and creating clocks. Please wait"

# while loop to write constraint commands to .sdc file
while { $i < $end_of_clocks } {
	#Create SDC command to create clocks.
	puts -nonewline $sdc_file "\ncreate_clock -name [concat [m1 get cell 0 $i]_synui] -period [m1 get cell $clk_freq_st_col $i] -waveform \{0 [expr {[m1 get cell $clk_freq_st_col $i]*[m1 get cell $clk_dc_st_col $i]/100}]\} \[get_ports [m1 get cell 0 $i]\]"

	# set_clock_transition SDC command to set clock transition values
	puts -nonewline $sdc_file "\nset_clock_transition -min -rise [m1 get cell $clk_ers_st_col $i] \[get_clocks [m1 get cell 0 $i]\]"
	puts -nonewline $sdc_file "\nset_clock_transition -min -fall [m1 get cell $clk_efs_st_col $i] \[get_clocks [m1 get cell 0 $i]\]"
	puts -nonewline $sdc_file "\nset_clock_transition -max -rise [m1 get cell $clk_lrs_st_col $i] \[get_clocks [m1 get cell 0 $i]\]"
	puts -nonewline $sdc_file "\nset_clock_transition -max -fall [m1 get cell $clk_lfs_st_col $i] \[get_clocks [m1 get cell 0 $i]\]"

	# set_clock_latency SDC command to set clock latency values
	puts -nonewline $sdc_file "\nset_clock_latency -source -early -rise [m1 get cell $clk_erd_st_col $i] \[get_clocks [m1 get cell 0 $i]\]"
	puts -nonewline $sdc_file "\nset_clock_latency -source -early -fall [m1 get cell $clk_efd_st_col $i] \[get_clocks [m1 get cell 0 $i]\]"
	puts -nonewline $sdc_file "\nset_clock_latency -source -late -rise [m1 get cell $clk_lrd_st_col $i] \[get_clocks [m1 get cell 0 $i]\]"
	puts -nonewline $sdc_file "\nset_clock_latency -source -late -fall [m1 get cell $clk_lfd_st_col $i] \[get_clocks [m1 get cell 0 $i]\]"

	set i [expr {$i+1}]
}
set clocks_start_row_actual [expr {$clocks_start_row+1}]
puts "\n Clocks created in .sdc file. Values for debugging: "
puts "\n Clock early rise delay start column in constraint file = $clk_erd_st_col"
puts "\n Clock early fall delay start column in constraint file = $clk_efd_st_col"
puts "\n Clock late rise delay start column in constraint file = $clk_lrd_st_col"
puts "\n Clock late fall delay start column in constraint file = $clk_lfd_st_col"
puts "\n Clock early rise slew start column in constraint file = $clk_ers_st_col"
puts "\n Clock early fall slew start column in constraint file = $clk_efs_st_col"
puts "\n Clock late rise slew start column in constraint file = $clk_lrs_st_col"
puts "\n Clock late fall slew start column in constraint file = $clk_lfs_st_col"
puts "\n Clock frequency start column in constraint file = $clk_freq_st_col"
puts "\n Clock duty cycle start column in constraint file = $clk_dc_st_col"
puts "\n Clock actual starting row = $clocks_start_row_actual"
puts "\n Clock actual ending row = $end_of_clocks"
```

*Screenshots*

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/27c7bbc2898276942cd24a2fda07c5f60b68a23e/day30/p18.PNG)

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/27c7bbc2898276942cd24a2fda07c5f60b68a23e/day30/p19.PNG)

*openMSP430.sdc*

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/27c7bbc2898276942cd24a2fda07c5f60b68a23e/day30/p20.PNG)

#### Processing of the constraints .csv file for INPUTS and dumping SDC commands to .sdc

I've processed the inputs data csv file, separated bit and bus inputs, and dumped input-based SDC commands into a.sdc file correctly. Below are screenshots of the terminal with many "puts" spitting out the variables, user debug information, and output.sdc, along with the basic code for the same.

*Code*

```tcl

# Finding the starting column number for input clock latency in INPUTS section
set ip_erd_st_col [lindex [lindex [m1 search rect $clocks_start_column $inputs_start [expr {$n_columns_concsv-1}] [expr {$outputs_start-1}] early_rise_delay] 0 ] 0 ]
set ip_efd_st_col [lindex [lindex [m1 search rect $clocks_start_column $inputs_start [expr {$n_columns_concsv-1}] [expr {$outputs_start-1}] early_fall_delay] 0 ] 0 ]
set ip_lrd_st_col [lindex [lindex [m1 search rect $clocks_start_column $inputs_start [expr {$n_columns_concsv-1}] [expr {$outputs_start-1}] late_rise_delay] 0 ] 0 ]
set ip_lfd_st_col [lindex [lindex [m1 search rect $clocks_start_column $inputs_start [expr {$n_columns_concsv-1}] [expr {$outputs_start-1}] late_fall_delay] 0 ] 0 ]

# Finding column number starting for input clock transition in INPUTS section only
set ip_ers_st_col [lindex [lindex [m1 search rect $clocks_start_column $inputs_start [expr {$n_columns_concsv-1}] [expr {$outputs_start-1}] early_rise_slew] 0 ] 0 ]
set ip_efs_st_col [lindex [lindex [m1 search rect $clocks_start_column $inputs_start [expr {$n_columns_concsv-1}] [expr {$outputs_start-1}] early_fall_slew] 0 ] 0 ]
set ip_lrs_st_col [lindex [lindex [m1 search rect $clocks_start_column $inputs_start [expr {$n_columns_concsv-1}] [expr {$outputs_start-1}] late_rise_slew] 0 ] 0 ]
set ip_lfs_st_col [lindex [lindex [m1 search rect $clocks_start_column $inputs_start [expr {$n_columns_concsv-1}] [expr {$outputs_start-1}] late_fall_slew] 0 ] 0 ]

# Finding column number starting for input related clock in INPUTS section only
set ip_rc_st_col [lindex [lindex [m1 search rect $clocks_start_column $inputs_start [expr {$n_columns_concsv-1}] [expr {$outputs_start-1}] clocks] 0 ] 0 ]

# Setting variables for actual input row start and end
set i [expr {$inputs_start+1}]
set end_of_inputs [expr {$outputs_start-1}]

puts "\nInfo-SDC: Working on input constraints.."
puts "\nInfo-SDC: Categorizing input ports as bits and busses"

# while loop to write constraint commands to .sdc file
while { $i < $end_of_inputs } {
# Checking if input is bussed or not
	set netlist [glob -dir $Netlist_Directory *.v]
	set tmp_file [open /tmp/1 w]
	foreach f $netlist {
		set fd [open $f]
		while { [gets $fd line] != -1 } {
			set pattern1 " [m1 get cell 0 $i];"
			if { [regexp -all -- $pattern1 $line] } {
				set pattern2 [lindex [split $line ";"] 0]
				if { [regexp -all {input} [lindex [split $pattern2 "\S+"] 0]] } {
					set s1 "[lindex [split $pattern2 "\S+"] 0] [lindex [split $pattern2 "\S+"] 1] [lindex [split $pattern2 "\S+"] 2]"
					puts -nonewline $tmp_file "\n[regsub -all {\s+} $s1 " "]"
				
				}
			}
		}
		close $fd
	}
	close $tmp_file
	set tmp_file [open /tmp/1 r]
	set tmp2_file [open /tmp/2 w]
	puts -nonewline $tmp2_file "[join [lsort -unique [split [read $tmp_file] \n]] \n]"
	close $tmp_file
	close $tmp2_file
	set tmp2_file [open /tmp/2 r]
	set count [llength [read $tmp2_file]]
	close $tmp2_file
	if {$count > 2} {
		set inp_ports [concat [m1 get cell 0 $i]*]
	} else {
		set inp_ports [m1 get cell 0 $i]
	}
		# set_input_transition SDC command to set input transition values
	puts -nonewline $sdc_file "\nset_input_transition -clock \[get_clocks [m1 get cell $ip_rc_st_col $i]\] -min -rise -source_latency_included [m1 get cell $ip_ers_st_col $i] \[get_ports $inp_ports\]"
	puts -nonewline $sdc_file "\nset_input_transition -clock \[get_clocks [m1 get cell $ip_rc_st_col $i]\] -min -fall -source_latency_included [m1 get cell $ip_efs_st_col $i] \[get_ports $inp_ports\]"
	puts -nonewline $sdc_file "\nset_input_transition -clock \[get_clocks [m1 get cell $ip_rc_st_col $i]\] -max -rise -source_latency_included [m1 get cell $ip_lrs_st_col $i] \[get_ports $inp_ports\]"
	puts -nonewline $sdc_file "\nset_input_transition -clock \[get_clocks [m1 get cell $ip_rc_st_col $i]\] -max -fall -source_latency_included [m1 get cell $ip_lfs_st_col $i] \[get_ports $inp_ports\]"
# set_input_delay SDC command to set input latency values
	puts -nonewline $sdc_file "\nset_input_delay -clock \[get_clocks [m1 get cell $ip_rc_st_col $i]\] -min -rise -source_latency_included [m1 get cell $ip_erd_st_col $i] \[get_ports $inp_ports\]"
	puts -nonewline $sdc_file "\nset_input_delay -clock \[get_clocks [m1 get cell $ip_rc_st_col $i]\] -min -fall -source_latency_included [m1 get cell $ip_efd_st_col $i] \[get_ports $inp_ports\]"
	puts -nonewline $sdc_file "\nset_input_delay -clock \[get_clocks [m1 get cell $ip_rc_st_col $i]\] -max -rise -source_latency_included [m1 get cell $ip_lrd_st_col $i] \[get_ports $inp_ports\]"
	puts -nonewline $sdc_file "\nset_input_delay -clock \[get_clocks [m1 get cell $ip_rc_st_col $i]\] -max -fall -source_latency_included [m1 get cell $ip_lfd_st_col $i] \[get_ports $inp_ports\]"
	set i [expr {$i+1}]

}
```

*Screenshots*

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/27c7bbc2898276942cd24a2fda07c5f60b68a23e/day30/p21.PNG)


*openMSP430.sdc*

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/27c7bbc2898276942cd24a2fda07c5f60b68a23e/day30/p22.PNG)

</details>

<details>
	<summary>Complete Scripting and Yosys Synthesis Introduction</summary>

The remaining activities are processing the output section and dumping the SDC file, checking the Yosys hierarchy, resolving errors, and doing a sample Yosys synthesis using example memory and explanation.

**Review of input file - openMSP430_design_constraints.csv**

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/27c7bbc2898276942cd24a2fda07c5f60b68a23e/day30/p23.PNG)


### Implementation

I've successfully finished the tasks assigned : writing code to handle errors in hierarchy check, learning about sample memory synthesis and its memory write and read processes, processing constraints csv files for outputs, and dumping SDC commands to.sdc files with actual processed data.

#### Processing of the constraints .csv file for OUTPUTS and dumping SDC commands to .sdc

I've processed the csv file for the outputs data, separated the bit and bus outputs, then dumped the output-based SDC instructions into a.sdc file successfully. Below are images of the terminal with many "puts" spitting out the variables, user debug information, and output.sdc, along with the basic code for the same.

*Code*

```tcl
#################################################################################################
######################################## Day 4 ##################################################
#################################################################################################
#
#Output constraint
#

# Finding column number starting for output clock latency in OUTPUTS section only
set op_erd_st_col [lindex [lindex [m1 search rect $clocks_start_column $outputs_start [expr {$n_columns_concsv-1}] [expr {$n_rows_concsv-1}] early_rise_delay] 0 ] 0 ]
set op_efd_st_col [lindex [lindex [m1 search rect $clocks_start_column $outputs_start [expr {$n_columns_concsv-1}] [expr {$n_rows_concsv-1}] early_fall_delay] 0 ] 0 ]
set op_lrd_st_col [lindex [lindex [m1 search rect $clocks_start_column $outputs_start [expr {$n_columns_concsv-1}] [expr {$n_rows_concsv-1}] late_rise_delay] 0 ] 0 ]
set op_lfd_st_col [lindex [lindex [m1 search rect $clocks_start_column $outputs_start [expr {$n_columns_concsv-1}] [expr {$n_rows_concsv-1}] late_fall_delay] 0 ] 0 ]

# Finding column number starting for output related clock in OUTPUTS section only
set op_rc_st_col [lindex [lindex [m1 search rect $clocks_start_column $outputs_start [expr {$n_columns_concsv-1}] [expr {$n_rows_concsv-1}] clocks] 0 ] 0 ]

# Finding column number starting for output load in OUTPUTS section only
set op_load_st_col [lindex [lindex [m1 search rect $clocks_start_column $outputs_start [expr {$n_columns_concsv-1}] [expr {$n_rows_concsv-1}] load] 0 ] 0 ]

# Setting variables for actual input row start and end
set i [expr {$outputs_start+1}]
set end_of_outputs [expr {$n_rows_concsv-1}]

puts "\nInfo-SDC: Working on output constraints.."
puts "\nInfo-SDC: Categorizing output ports as bits and busses"

# while loop to write constraint commands to .sdc file
while { $i < $end_of_outputs } {
	# Checking if input is bussed or not
	set netlist [glob -dir $Netlist_Directory *.v]
	set tmp_file [open /tmp/1 w]
	foreach f $netlist {
		set fd [open $f]
		while { [gets $fd line] != -1 } {
			set pattern1 " [m1 get cell 0 $i];"
			if { [regexp -all -- $pattern1 $line] } {
				set pattern2 [lindex [split $line ";"] 0]
				if { [regexp -all {output} [lindex [split $pattern2 "\S+"] 0]] } {
					set s1 "[lindex [split $pattern2 "\S+"] 0] [lindex [split $pattern2 "\S+"] 1] [lindex [split $pattern2 "\S+"] 2]"
					puts -nonewline $tmp_file "\n[regsub -all {\s+} $s1 " "]"
				}
			}
		}
	close $fd
	}
	close $tmp_file
	set tmp_file [open /tmp/1 r]
	set tmp2_file [open /tmp/2 w]
	puts -nonewline $tmp2_file "[join [lsort -unique [split [read $tmp_file] \n]] \n]"
	close $tmp_file
	close $tmp2_file
	set tmp2_file [open /tmp/2 r]
	set count [llength [read $tmp2_file]]
	close $tmp2_file
	if {$count > 2} {
		set op_ports [concat [m1 get cell 0 $i]*]
	} else {
		set op_ports [m1 get cell 0 $i]
	}

	# set_output_delay SDC command to set output latency values
	puts -nonewline $sdc_file "\nset_output_delay -clock \[get_clocks [m1 get cell $op_rc_st_col $i]\] -min -rise -source_latency_included [m1 get cell $op_erd_st_col $i] \[get_ports $op_ports\]"
	puts -nonewline $sdc_file "\nset_output_delay -clock \[get_clocks [m1 get cell $op_rc_st_col $i]\] -min -fall -source_latency_included [m1 get cell $op_efd_st_col $i] \[get_ports $op_ports\]"
	puts -nonewline $sdc_file "\nset_output_delay -clock \[get_clocks [m1 get cell $op_rc_st_col $i]\] -max -rise -source_latency_included [m1 get cell $op_lrd_st_col $i] \[get_ports $op_ports\]"
	puts -nonewline $sdc_file "\nset_output_delay -clock \[get_clocks [m1 get cell $op_rc_st_col $i]\] -max -fall -source_latency_included [m1 get cell $op_lfd_st_col $i] \[get_ports $op_ports\]"

	# set_load SDC command to set load values
	puts -nonewline $sdc_file "\nset_load [m1 get cell $op_load_st_col $i] \[get_ports $op_ports\]"

	set i [expr {$i+1}]
}

close $sdc_file
puts "\nInfo-SDC: SDC created. Please use constraints in path $Output_Directory/$Design_Name.sdc"
```

*Screenshots*

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/27c7bbc2898276942cd24a2fda07c5f60b68a23e/day30/p24.PNG)

*openMSP430.sdc*

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/27c7bbc2898276942cd24a2fda07c5f60b68a23e/day30/p25.PNG)

#### Memory module yosys synthesis and explanation

The verilog code *memory.v* for a single-bit address and single-bit data memory unit is given below.

*Code*

```verilog
module memory (CLK, ADDR, DIN, DOUT);

parameter wordSize = 1;
parameter addressSize = 1;

input ADDR, CLK;
input [wordSize-1:0] DIN;
output reg [wordSize-1:0] DOUT;
reg [wordSize:0] mem [0:(1<<addressSize)-1];

always @(posedge CLK) begin
	mem[ADDR] <= DIN;
	DOUT <= mem[ADDR];
	end

endmodule
```

The basic Yosys script *memory.ys* to run this and obtain a gate-level netlist and 2D representation of the memory module in gate components is provided below.

*Script*

```tcl
# Reading the library
read_liberty -lib -ignore_miss_dir -setattr blackbox /home/kunalg/Desktop/work/openmsp430/openmsp430/osu018_stdcells.lib
# Reading the verilog
read_verilog verilog/memory.v
synth top memory
splitnets -ports -format ___
dfflibmap -liberty /home/kunalg/Desktop/work/openmsp430/openmsp430/osu018_stdcells.lib
opt
abc -liberty /home/kunalg/Desktop/work/openmsp430/openmsp430/osu018_stdcells.lib
flatten
clean -purge
opt
clean
# Writing the netlist
write_verilog memory_synth.v
# Representation of netlist with it's components
show
~     
```

The output view of netlist from the code is shown below.

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/27c7bbc2898276942cd24a2fda07c5f60b68a23e/day30/p26.PNG)


*Memory write process explained in following images using truth table*

Basic illustration of the write process

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/27c7bbc2898276942cd24a2fda07c5f60b68a23e/day30/p27.PNG)


Before first rising edge of the clock

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/27c7bbc2898276942cd24a2fda07c5f60b68a23e/day30/p28.PNG)

After first rising edge of the clock - write process done

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/27c7bbc2898276942cd24a2fda07c5f60b68a23e/day30/p29.PNG)

#### Hierarchy check script dumping

I have successfully written the code for dumping the hierarchy check script. The basic code of the same and screenshots of the terminal with several "puts" printing out the variables and user debug information as well as output .hier.ys are shown below.

*Code*

```tcl
###############################################################################
# Hierarchy Check
#############################################################################################
puts "\nInfo: Creating hierarchy check script to be used by Yosys"
set data "read_liberty -lib -ignore_miss_dir -setattr blackbox ${Late_Library_Path}"
set filename "$Design_Name.hier.ys"
set fileId [open $Output_Directory/$filename "w"]
puts -nonewline $fileId $data
set netlist [glob -dir $Netlist_Directory *.v]
foreach f $netlist {
	set data $f
	puts -nonewline $fileId "\nread_verilog $f"
	puts "\nInfo: Netlist being read for user debug: $f" 
}
puts -nonewline $fileId "\nhierarchy -check"
close $fileId


```

*Screenshots*

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/27c7bbc2898276942cd24a2fda07c5f60b68a23e/day30/p30.PNG)

*openMSP430.hier.ys*

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/27c7bbc2898276942cd24a2fda07c5f60b68a23e/day30/p31.PNG)


#### Hierarchy Check Run & Error Handling

I have successfully written the code for hierarchy check error handling in case any error pops up during hierarchy check run in Yosys and *exits if hierarchy check fails*. The basic code of the same and screenshots of the terminal with several "puts" printing out the variables and user debug information are shown below.

*Code*

```tcl
# Hierarchy check error handling
# Hierarchy check error handling done to see any errors popping up in above script.
# Running hierarchy check in yosys by dumping log to log file and catching execution message
set error_flag [catch {exec yosys -s $Output_Directory/$Design_Name.hier.ys >& $Output_Directory/$Design_Name.hierarchy_check.log} msg]
puts "Errfor flag value for user debug: $error_flag"
if { $error_flag } {
	set filename "$Output_Directory/$Design_Name.hierarchy_check.log"
	# EDA tool specific hierarchy error search pattern
	set pattern {referenced in module}
	set count 0
	set fid [open $filename r]
	while { [gets $fid line] != -1 } {
		incr count [regexp -all -- $pattern $line]
		if { [regexp -all -- $pattern $line] } {
			puts "\nError: Module [lindex $line 2] is not part of design $Design_Name. Please correct RTL in the path '$Netlist_Directory'"
			puts "\nInfo: Hierarchy check FAIL"
		}
	}
	close $fid
	puts "\nInfo: Please find hierarchy check details in '[file normalize $Output_Directory/$Design_Name.hierarchy_check.log]' for more info. Exiting..."
	
} else {
	puts "\nInfo: Hierarchy check PASS"
	puts "\nInfo: Please find hierarchy check details in '[file normalize $Output_Directory/$Design_Name.hierarchy_check.log]' for more info"
}

```

*Screenshots*

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/27c7bbc2898276942cd24a2fda07c5f60b68a23e/day30/p32.PNG)

*openMSP430.hierarchy_check.log*

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/27c7bbc2898276942cd24a2fda07c5f60b68a23e/day30/p33.PNG)

*Change module name by adding _vsd to check error is coming or not.*

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/27c7bbc2898276942cd24a2fda07c5f60b68a23e/day30/p34.PNG)


![image](https://github.com/Sidv005/Samsung-PD-Training/blob/27c7bbc2898276942cd24a2fda07c5f60b68a23e/day30/p35.PNG)

*openMSP430.hierarchy_check.log*

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/27c7bbc2898276942cd24a2fda07c5f60b68a23e/day30/p36.PNG)
</details>

<details>
	<summary>Advanced Scripting Techniques and Quality of Results (QoR) Generation </summary>

The remaining activities include running Yosys' main synthesis, learning about and using procedures at the application level, creating commands, and writing the files needed for the OpenTimer tool, like .conf,.spef, and timing Create an OpenTimer script, launch an OpenTimer STA, and gather the information needed to create a QoR.final step is to print the gathered data in a tool-standard QoR output format using the results file that was created during the OpenTimer STA run.

### Implementation

I have successfully coded all the required elements to achieve left over tasks, and all the details of the sub-tasks achieved are shown below.

#### Main Yosys synthesis script dumping

I have successfully written the code for the main Yosys synthesis script .ys file and dumped the script. The basic code of the same and screenshots of the terminal with several "puts" printing out the variables and user debug information are shown below.

*Code*

```tcl
##################################################################################################################################################

# Main Synthesis Script for yosys
# ---------------------
puts "\nInfo: Creating main synthesis script to be used by Yosys"
set data "read_liberty -lib -ignore_miss_dir -setattr blackbox ${Late_Library_Path}"
set filename "$Design_Name.ys"
set fileId [open $Output_Directory/$filename "w"]
puts -nonewline $fileId $data
set netlist [glob -dir $Netlist_Directory *.v]
foreach f $netlist {
	puts -nonewline $fileId "\nread_verilog $f"
}
puts -nonewline $fileId "\nhierarchy -top $Design_Name"
puts -nonewline $fileId "\nsynth -top $Design_Name"
puts -nonewline $fileId "\nsplitnets -ports -format ___\ndfflibmap -liberty ${Late_Library_Path} \nopt"
puts -nonewline $fileId "\nabc -liberty ${Late_Library_Path}"
puts -nonewline $fileId "\nflatten"
puts -nonewline $fileId "\nclean -purge\niopadmap -outpad BUFX2 A:Y -bits\nopt\nclean"
puts -nonewline $fileId "\nwrite_verilog $Output_Directory/$Design_Name.synth.v"
close $fileId
puts "\nInfo: Synthesis script created and can be accessed from path $Output_Directory/$Design_Name.ys"

```

*Screenshots*

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/9dce68881f2263913db3a03a59e7b183e91056d7/day30/p37.PNG)


*openMSP430.ys*

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/9dce68881f2263913db3a03a59e7b183e91056d7/day30/p38.PNG)

#### Running main synthesis script & error handling

I have successfully written the code for running the main Yosys synthesis script and exiting if errors are found. The basic code and screenshots of the terminal are shown below.

*Code*

```tcl
puts "\nInfo: Running synthesis......."
# Main synthesis error handling
# Running main synthesis in yosys by dumping logs to the log directory and catching execution message
if { [catch {exec yosys -s $Output_Directory/$Design_Name.ys >& $Output_Directory/$Design_Name.synthesis.log} msg] } {
	puts "\nError: Synthesis failed due to errors. Please refer to log $Output_Directory/$Design_Name.synthesis.log for errors. Exiting...."
	exit
} else {
	puts "\nInfo: Synthesis finished successfully"
}
puts "\nInfo: Please refer to log $Output_Directory/$Design_Name.synthesis.log"

```

*Screenshots*

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/9dce68881f2263913db3a03a59e7b183e91056d7/day30/p39.PNG)


*openMSP430.synthesis.log*

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/9dce68881f2263913db3a03a59e7b183e91056d7/day30/p40.PNG)

*openMSP430.synth.v*

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/9dce68881f2263913db3a03a59e7b183e91056d7/day30/p41.PNG)

*Error handling*

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/9dce68881f2263913db3a03a59e7b183e91056d7/day30/p42.PNG)

*Log file for error handling*

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/9dce68881f2263913db3a03a59e7b183e91056d7/day30/p43.PNG)

#### Editing .synth.v to be usable by OpenTimer

I have successfully written the code to edit the main synthesis output netlist .synth.v to make it usable for OpenTimer and other STA and PnR needs by replacing lines with "*" as a word and by removing "\" from any and all lines that have it. The basic code of the same and screenshots of the terminal with several "puts" printing out the variables and user debug information are shown below.

*Code*

```tcl
############################################## Editing .synth.v to be usable by Opentimer #######################################################

puts "\nInfo: Removing '*' and '\\' from netlist"
set fileId [open /tmp/1 "w"]
puts -nonewline $fileId [exec grep -v -w "*" $Output_Directory/$Design_Name.synth.v]
close $fileId
set output [open $Output_Directory/$Design_Name.final.synth.v "w"]
set filename "/tmp/1"
set fid [open $filename r]
while { [gets $fid line] != -1 } {
	puts -nonewline $output [string map {"\\" ""} $line]
	puts -nonewline $output "\n"
}
close $fid
close $output
puts "\nInfo: Please find the synthesized netlist for $Design_Name at below path. You can use this netlist for STA or PNR"
puts "\nPath: $Output_Directory/$Design_Name.final.synth.v"
```

*Screenshots*

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/9dce68881f2263913db3a03a59e7b183e91056d7/day30/p44.PNG)


*openMSP430.synth.v*

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/9dce68881f2263913db3a03a59e7b183e91056d7/day30/p45.PNG)


*/tmp/1*

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/9dce68881f2263913db3a03a59e7b183e91056d7/day30/p46.PNG)

*openMSP430.final.synth.v*

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/9dce68881f2263913db3a03a59e7b183e91056d7/day30/p47.PNG)

#### World of Procs (TCL Procedure)

Procs can be used to create user-defined commands, as shown below. I have successfully written the code for all the procs. The basic codes of all the procs and screenshots of the terminal with several "puts" printing out the variables and user debug information for the 'set_multi_cpu_usage' and the 'read_sdc' procs are shown below.

##### reopenStdout.proc

This proc redirects the 'stdout' screen log to the file in the proc's argument.

*Code*

```tcl
#!/bin/tclsh
# proc to redirect screen log to file
proc reopenStdout {file} {
    close stdout
    open $file w       
}
```

##### set_multi_cpu_usage.proc

This proc outputs multiple threads of the CPU usage command required for the OpenTimer tool.

*Code*

```tcl
#!/bin/tclsh

proc set_multi_cpu_usage {args} {
        array set options {-localCpu <num_of_threads> -help "" }
        foreach {switch value} [array get options] {
       # puts "Option $switch is $value"
        }
        while {[llength $args]} {
       # puts "llength is [llength $args]"
       # puts "lindex 0 of \"$args\" is [lindex $args 0]"
                switch -glob -- [lindex $args 0] {
                -localCpu {
                           #puts "old args is $args"
                           set args [lassign $args - options(-localCpu)]
                           #puts "new args is \"$args\""
                           puts "set_num_threads $options(-localCpu)"
                          }
                -help {
                           #puts "old args is $args"
                           set args [lassign $args - options(-help) ]
                           #puts "new args is \"$args\""
                           puts "Usage: set_multi_cpu_usage -localCpu <num_of_threads> -help"
                           puts "\t-localCpu - To limit number of threads used"
                           puts "\t-help - To print details of proc"
                      }
                }
        }
}

#set_multi_cpu_usage -localCpu 5 -help
```

*Screenshots*

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/9dce68881f2263913db3a03a59e7b183e91056d7/day30/p48.PNG)

##### read_lib.proc

This proc outputs commands to read early and late libraries required for the OpenTimer tool.

*Code*

```tcl
#!/bin/tclsh
proc read_lib args {
	# Setting command parameter options and its values
	array set options {-late <late_lib_path> -early <early_lib_path> -help ""}
	while {[llength $args]} {
		switch -glob -- [lindex $args 0] {
		-late {
			set args [lassign $args - options(-late) ]
			puts "set_late_celllib_fpath $options(-late)"
		      }
		-early {
			set args [lassign $args - options(-early) ]
			puts "set_early_celllib_fpath $options(-early)"
		       }
		-help {
			set args [lassign $args - options(-help) ]
			puts "Usage: read_lib -late <late_lib_path> -early <early_lib_path>"
			puts "-late <provide late library path>"
			puts "-early <provide early library path>"
			puts "-help - Provides user deatails on how to use the command"
		      }	
		default break
		}
	}
}
```

##### read_verilog.proc

This proc outputs commands to read the synthesised netlist required for the OpenTimer tool.

*Code*

```tcl
#!/bin/tclsh

# Proc to convert read_verilog to OpenTimer format
proc read_verilog {arg1} {
	puts "set_verilog_fpath $arg1"
}
```

##### read_sdc.proc

This proc outputs commands to read constraints .timing file required for the OpenTimer tool. This procs converts SDC file contents to .timing file format for use by the OpenTimer tool, and the conversion code is explained stage by stage with sufficient screenshots.

###### Converting 'create_clock' constraints

Initially, the proc takes the SDC file as an input argument or parameter and processes the 'create_clock' constraints part of SDC.

*Code*

```tcl
#!/bin/tclsh
proc read_sdc {arg1} {

# 'file dirname <>' to get directory path only from full path
set sdc_dirname [file dirname $arg1]
# 'file tail <>' to get last element
set sdc_filename [lindex [split [file tail $arg1] .] 0 ]
set sdc [open $arg1 r]
set tmp_file [open /tmp/1 w]

# Removing "[" & "]" from SDC for further processing the data with 'lindex'
# 'read <>' to read entire file
puts -nonewline $tmp_file [string map {"\[" "" "\]" " "} [read $sdc]]     
close $tmp_file

# Opening tmp file to write constraints converted from generated SDC
set timing_file [open /tmp/3 w]

# Converting create_clock constraints
# -----------------------------------
set tmp_file [open /tmp/1 r]
set lines [split [read $tmp_file] "\n"]
# 'lsearch -all -inline' to search list for pattern and retain elementas with pattern only
set find_clocks [lsearch -all -inline $lines "create_clock*"]
foreach elem $find_clocks {
	set clock_port_name [lindex $elem [expr {[lsearch $elem "get_ports"]+1}]]
	set clock_period [lindex $elem [expr {[lsearch $elem "-period"]+1}]]
	set duty_cycle [expr {100 - [expr {[lindex [lindex $elem [expr {[lsearch $elem "-waveform"]+1}]] 1]*100/$clock_period}]}]
	puts $timing_file "\nclock $clock_port_name $clock_period $duty_cycle"
}
close $tmp_file
```

*Screenshots*

*openMSP430.sdc*

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/9dce68881f2263913db3a03a59e7b183e91056d7/day30/p49.PNG)

*/tmp/1*

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/9dce68881f2263913db3a03a59e7b183e91056d7/day30/p50.PNG)

*/tmp/3*

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/9dce68881f2263913db3a03a59e7b183e91056d7/day30/p51.PNG)

###### Converting 'set_clock_latency' constraints

Processes 'set_clock_latency' constraints part of SDC.

*Code*

```tcl
# Converting set_clock_latency constraints
# ----------------------------------------
set find_keyword [lsearch -all -inline $lines "set_clock_latency*"]
set tmp2_file [open /tmp/2 w]
set new_port_name ""
foreach elem $find_keyword {
        set port_name [lindex $elem [expr {[lsearch $elem "get_clocks"]+1}]]
	if {![string match $new_port_name $port_name]} {
        	set new_port_name $port_name
        	set delays_list [lsearch -all -inline $find_keyword [join [list "*" " " $port_name " " "*"] ""]]
        	set delay_value ""
        	foreach new_elem $delays_list {
        		set port_index [lsearch $new_elem "get_clocks"]
        		lappend delay_value [lindex $new_elem [expr {$port_index-1}]]
        	}
		puts -nonewline $tmp2_file "\nat $port_name $delay_value"
	}
}

close $tmp2_file
set tmp2_file [open /tmp/2 r]
puts -nonewline $timing_file [read $tmp2_file]
close $tmp2_file
```

*Screenshots*

*/tmp/2*

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/9dce68881f2263913db3a03a59e7b183e91056d7/day30/p52.PNG)

*/tmp/3*

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/9dce68881f2263913db3a03a59e7b183e91056d7/day30/p53.PNG)

###### Converting 'set_clock_transition' constraints

Processes 'set_clock_transition' constraints part of SDC.

*Code*

```tcl
# Converting set_clock_transition constraints
# -------------------------------------------
set find_keyword [lsearch -all -inline $lines "set_clock_transition*"]
set tmp2_file [open /tmp/2 w]
set new_port_name ""
foreach elem $find_keyword {
        set port_name [lindex $elem [expr {[lsearch $elem "get_clocks"]+1}]]
        if {![string match $new_port_name $port_name]} {
		set new_port_name $port_name
		set delays_list [lsearch -all -inline $find_keyword [join [list "*" " " $port_name " " "*"] ""]]
        	set delay_value ""
        	foreach new_elem $delays_list {
        		set port_index [lsearch $new_elem "get_clocks"]
        		lappend delay_value [lindex $new_elem [expr {$port_index-1}]]
        	}
        	puts -nonewline $tmp2_file "\nslew $port_name $delay_value"
	}
}

close $tmp2_file
set tmp2_file [open /tmp/2 r]
puts -nonewline $timing_file [read $tmp2_file]
close $tmp2_file
```

*Screenshots*

*/tmp/2*

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/9dce68881f2263913db3a03a59e7b183e91056d7/day30/p54.PNG)

*/tmp/3*

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/9dce68881f2263913db3a03a59e7b183e91056d7/day30/p55.PNG)


###### Converting 'set_input_delay' constraints

Processes 'set_input_delay' constraints part of SDC.

*Code*

```tcl
# Converting set_input_delay constraints
# --------------------------------------
set find_keyword [lsearch -all -inline $lines "set_input_delay*"]
set tmp2_file [open /tmp/2 w]
set new_port_name ""
foreach elem $find_keyword {
        set port_name [lindex $elem [expr {[lsearch $elem "get_ports"]+1}]]
        if {![string match $new_port_name $port_name]} {
                set new_port_name $port_name
        	set delays_list [lsearch -all -inline $find_keyword [join [list "*" " " $port_name " " "*"] ""]]
		set delay_value ""
        	foreach new_elem $delays_list {
        		set port_index [lsearch $new_elem "get_ports"]
        		lappend delay_value [lindex $new_elem [expr {$port_index-1}]]
        	}
        	puts -nonewline $tmp2_file "\nat $port_name $delay_value"
	}
}
close $tmp2_file
set tmp2_file [open /tmp/2 r]
puts -nonewline $timing_file [read $tmp2_file]
close $tmp2_file
```

*Screenshots*

*/tmp/2*

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/9dce68881f2263913db3a03a59e7b183e91056d7/day30/p56.PNG)

*/tmp/3*

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/9dce68881f2263913db3a03a59e7b183e91056d7/day30/p57.PNG)

###### Converting 'set_input_transition' constraints

Processes 'set_input_transition' constraints part of SDC.

*Code*

```tcl
# Converting set_input_transition constraints
# -------------------------------------------
set find_keyword [lsearch -all -inline $lines "set_input_transition*"]
set tmp2_file [open /tmp/2 w]
set new_port_name ""
foreach elem $find_keyword {
        set port_name [lindex $elem [expr {[lsearch $elem "get_ports"]+1}]]
        if {![string match $new_port_name $port_name]} {
                set new_port_name $port_name
        	set delays_list [lsearch -all -inline $find_keyword [join [list "*" " " $port_name " " "*"] ""]]
        	set delay_value ""
        	foreach new_elem $delays_list {
        		set port_index [lsearch $new_elem "get_ports"]
        		lappend delay_value [lindex $new_elem [expr {$port_index-1}]]
        	}
        	puts -nonewline $tmp2_file "\nslew $port_name $delay_value"
	}
}

close $tmp2_file
set tmp2_file [open /tmp/2 r]
puts -nonewline $timing_file [read $tmp2_file]
close $tmp2_file
```

*Screenshots*

*/tmp/2*

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/9dce68881f2263913db3a03a59e7b183e91056d7/day30/p58.PNG)

*/tmp/3*

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/9dce68881f2263913db3a03a59e7b183e91056d7/day30/p59.PNG)

###### Converting 'set_output_delay' constraints

Processes 'set_output_delay' constraints part of SDC.

*Code*

```tcl
# Converting set_output_delay constraints
# ---------------------------------------
set find_keyword [lsearch -all -inline $lines "set_output_delay*"]
set tmp2_file [open /tmp/2 w]
set new_port_name ""
foreach elem $find_keyword {
        set port_name [lindex $elem [expr {[lsearch $elem "get_ports"]+1}]]
        if {![string match $new_port_name $port_name]} {
                set new_port_name $port_name
        	set delays_list [lsearch -all -inline $find_keyword [join [list "*" " " $port_name " " "*"] ""]]
        	set delay_value ""
        	foreach new_elem $delays_list {
        		set port_index [lsearch $new_elem "get_ports"]
        		lappend delay_value [lindex $new_elem [expr {$port_index-1}]]
        	}
        	puts -nonewline $tmp2_file "\nrat $port_name $delay_value"
	}
}

close $tmp2_file
set tmp2_file [open /tmp/2 r]
puts -nonewline $timing_file [read $tmp2_file]
close $tmp2_file
```

*Screenshots*

*/tmp/2*

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/9dce68881f2263913db3a03a59e7b183e91056d7/day30/p60.PNG)

*/tmp/3*

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/9dce68881f2263913db3a03a59e7b183e91056d7/day30/p61.PNG)

###### Converting 'set_load' constraints

Processes 'set_load' constraints part of SDC. And with that, all SDC constarints are processed, so we close the /tmp/3 file containing all processed data for now.

*Code*

```tcl
# Converting set_load constraints
# -------------------------------
set find_keyword [lsearch -all -inline $lines "set_load*"]
set tmp2_file [open /tmp/2 w]
set new_port_name ""
foreach elem $find_keyword {
        set port_name [lindex $elem [expr {[lsearch $elem "get_ports"]+1}]]
        if {![string match $new_port_name $port_name]} {
                set new_port_name $port_name
        	set delays_list [lsearch -all -inline $find_keyword [join [list "*" " " $port_name " " "*" ] ""]]
        	set delay_value ""
        	foreach new_elem $delays_list {
        	set port_index [lsearch $new_elem "get_ports"]
        	lappend delay_value [lindex $new_elem [expr {$port_index-1}]]
        	}
        	puts -nonewline $timing_file "\nload $port_name $delay_value"
	}
}
close $tmp2_file
set tmp2_file [open /tmp/2 r]
puts -nonewline $timing_file  [read $tmp2_file]
close $tmp2_file

# Closing tmp file after writing constraints converted from generated SDC
close $timing_file
```

*Screenshots*

*/tmp/3*

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/9dce68881f2263913db3a03a59e7b183e91056d7/day30/p62.PNG)

#### QoR (Quality of Results) Generation

I have successfully written the code for QoR generation. The basic code and screenshots of the terminal are shown below.

*Code*

```tcl
# Quality of Results (QoR) generation
puts "\n"
puts "                                                           ****PRELAYOUT TIMING RESULTS_SYNUI****\n"
set formatStr {%15s%14s%21s%16s%16s%15s%15s%15s%15s}
puts [format $formatStr "-----------" "-------" "--------------" "---------" "---------" "--------" "--------" "-------" "-------"]
puts [format $formatStr "Design Name" "Runtime" "Instance Count" "WNS Setup" "FEP Setup" "WNS Hold" "FEP Hold" "WNS RAT" "FEP RAT"]
puts [format $formatStr "-----------" "-------" "--------------" "---------" "---------" "--------" "--------" "-------" "-------"]
foreach design_name $Design_Name runtime $time_elapsed_in_sec instance_count $Instance_count wns_setup $worst_negative_setup_slack fep_setup $Number_of_setup_violations wns_hold $worst_negative_hold_slack fep_hold $Number_of_hold_violations wns_rat $worst_RAT_slack fep_rat $Number_output_violations {
	puts [format $formatStr $design_name $runtime $instance_count $wns_setup $fep_setup $wns_hold $fep_hold $wns_rat $fep_rat]
}
puts [format $formatStr "-----------" "-------" "--------------" "---------" "---------" "--------" "--------" "-------" "-------"]
puts "\n"

```

*Screenshots*

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/9dce68881f2263913db3a03a59e7b183e91056d7/day30/p_63.PNG)

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/9dce68881f2263913db3a03a59e7b183e91056d7/day30/p_64.PNG)

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/9dce68881f2263913db3a03a59e7b183e91056d7/day30/p_65.PNG)
![image](https://github.com/Sidv005/Samsung-PD-Training/blob/9dce68881f2263913db3a03a59e7b183e91056d7/day30/p_66.PNG)
![image](https://github.com/Sidv005/Samsung-PD-Training/blob/9dce68881f2263913db3a03a59e7b183e91056d7/day30/p_67.PNG)

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/9dce68881f2263913db3a03a59e7b183e91056d7/day30/p_68.PNG)

</details>

## Day 31 Low power Design ##
<details>
	<summary> Module 1</summary>

Low power Design:-

- Low-power design in Very Large Scale Integration (VLSI) is a critical aspect in modern semiconductor design, especially as portable devices and battery-powered systems become increasingly prevalent.
- Reducing power consumption in VLSI circuits is essential for extending battery life, minimizing heat dissipation, and meeting energy efficiency goals.

Why low power design ?

- Differentiating between Power and Energy

- Power

Power is the rate at which energy is transferred or converted. It is the amount of energy transferred or converted per unit of time.

In electrical terms, power ((P)) is calculated as the product of voltage ((V)) and current ((I)): [ P = V \times I ]

Observations as Power Increases

1. Heat Dissipation:

Increases with higher power.

2. Cooling Cost:

Increases with the rise in power consumption.

3. Frequency Limitations:

Higher power may limit achievable frequencies in electronic circuits.

4. Material Degradation:

Overall material degradation accelerates with increased power.

- Energy

   - Definition: Energy represents the ability to perform work or generate heat and manifests in diverse forms like electrical, mechanical, and thermal energy.

   - Formula: In electrical terms, energy (E) can be calculated by multiplying power (P) by time (t): E=Pxt or E=VxIxt

Economics of power and energy

1. Performance.

2. Cost.

Packaging

Battery capacity

Shipping

3. Weight.

4. Form factor

5. Functionality.

6. Context of use.

Low power designs are essential for various electronic devices and systems for several reasons:

- Extended Battery Life: In portable devices like smartphones, laptops, and wearables, low power designs help extend battery life. This is crucial for ensuring longer usage between charges, improving the overall convenience and usability of these devices.
- Energy Efficiency: Lower power consumption contributes to overall energy efficiency, reducing the environmental impact of electronic devices. Energy-efficient designs align with sustainability goals and regulatory requirements.
- Heat Dissipation: High-power consumption leads to increased heat generation. Low power designs help mitigate heat dissipation challenges, preventing devices from overheating. This is particularly important for compact and densely packed electronic systems.
- Form Factor and Size: Low power designs often allow for more compact and lightweight devices. This is especially critical in applications where space is limited, such as in IoT devices, medical implants, and other miniaturized electronic systems.
- Cost Savings: Lower power consumption can lead to cost savings in terms of smaller batteries, reduced cooling requirements, and lower electricity bills. This is important for both manufacturers and end-users.
- Reliability and Longevity: Reduced power usage can contribute to the longevity and reliability of electronic components. Lower temperatures and less stress on materials can result in longer lifespans for integrated circuits and other electronic components.
</details>

<details>
	<summary> Module 2</summary>

Low power fundamentals

- Creating low-power designs involves a combination of strategies, methodologies, and techniques across various levels of IC and system design.Here are the essential aspects and practices in low-power design:
1. Design Goals and Requirements Analysis
- Power Budgeting: Determine acceptable power consumption limits for different system components.
- Use Case Analysis : Understand various usage scenarios to optimize power usage during different modes of operation.

2. Architecture-Level Strategies
- Power-Aware Architectures : Design with power efficiency in mind, incorporating techniques like clock gating, power gating, and voltage/frequency scaling.
- Partitioning and Power Domains : Divide the system into power domains, allowing selective activation/deactivation of parts to conserve power.

3. Architecture-Level Strategies
- Power-Aware Architectures : Design with power efficiency in mind, incorporating techniques like clock gating, power gating, and voltage/frequency scaling.
- Partitioning and Power Domains : Divide the system into power domains, allowing selective activation/deactivation of parts to conserve power.

4. Circuit-Level Techniques

- Transistor Level Optimization : Utilize low-leakage transistors, sub-threshold operation, and other techniques to minimize leakage currents.
- Clock and Data Management : Implement clock gating, data encoding, and other logic techniques to reduce dynamic power consumption.

5. System-Level Strategies

- Dynamic Power Management : Employ techniques like DVFS (Dynamic Voltage and Frequency Scaling) and AVS (Adaptive Voltage Scaling) to adjust power based on workload.
- Low-Power Modes : Utilize sleep, idle, or power-down modes during periods of inactivity.

6. Verification and Validation

- Power-Aware Simulation and Verification : Use specialized tools and methodologies to validate power consumption estimates and optimize power-critical paths.
- Hardware/Software Co-Design : Collaborate on power optimization between hardware and software for maximum efficiency.

7. Hardware/Software Co-Design

- Collaborate on power optimization between hardware and software for maximum efficiency.

8. Technological Innovations

- Advanced Process Nodes : Benefit from newer process technologies that inherently offer better power efficiency.

- Emerging Design Methodologies : Explore novel design approaches like approximate computing, probabilistic computing, or energy harvesting for specific applications.

9. Tools and Methodologies

- Power Analysis Tools : Utilize simulation tools providing accurate power estimates at different design stages.

- Power-Aware Synthesis Tools : Employ tools optimizing circuits and architectures for reduced power consumption.

10. Standard Compliance and Optimization

- Compliance with Power Standards : Ensure designs meet regulatory standards for power consumption.

- Trade-off Analysis : Balance performance, area, and power to achieve optimal design results.

11. Documentation and Knowledge Sharing
- Document Power Considerations : Maintain comprehensive documentation detailing power design decisions, methodologies, and trade-offs.

- Knowledge Sharing : Encourage knowledge sharing among design teams to propagate best practices and lessons learned.

Power Consumption view of SOC

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/20ee8a926517109770884511e9fe4962e5d92f4b/day31/p1.PNG)

Balance between power management and low power design.

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/20ee8a926517109770884511e9fe4962e5d92f4b/day31/p2.PNG)

i. Density : Density is the ratio of power and area.Heat is a primary consequence of density.Power consumed is a function of current junction temperature.

ii. Delivery : Delivery is managing I and dI/dt.Power supply must supply Imax within Vmin and Vmax. Power supply must withstand Imax-Imin scenario within Vmin-Vmax.

iii. Leakage : Leakage = tax paid by transistors when they are powered on.Leakage power can be enormous.Leakage increses with gate size and temperature.Leakage can heat up the chip.Turning off is the best way to arrest leakage power.

iv. Reliabilty : Current degrades material.High current drawn fuses material.

**How does power gating works**

- Power gating involves the use of special power gating transistors, also known as power switches or isolation transistors. These transistors act as switches to control the flow of power to a specific block or module.
- A control logic unit is responsible for determining when a particular block or module can be powered down and when it needs to be powered up. This control logic is often based on the activity or inactivity of the corresponding functional block.
- When the control logic decides to power down a specific block, the power gating transistors are turned off, isolating the block from the power supply. This isolation prevents current flow and reduces static power consumption.
- Before powering down, critical state information (such as register contents) from the block being powered down is often stored in retention registers. This ensures that when power is restored, the block can resume operation seamlessly without loss of critical data.
- When the block needs to become active again, the control logic triggers the power gating transistors to turn on, allowing power to flow back into the block. The retention registers are then used to restore the state of the block.
- Careful consideration must be given to the timing of power-up and power-down operations to avoid glitches or timing violations. Ensuring proper sequencing is crucial to maintain correct functionality.

**Challenges and Consideration**

- Implementing power gating adds complexity to the design, requiring additional control logic and ensuring proper synchronization to avoid issues such as glitches or improper power-up sequences.
- Switching power gates on and off introduces some overhead in terms of delay and power consumption associated with the control logic.
- Proper verification and testing are crucial to ensure correct functionality of power gating to prevent issues like data loss or corruption during power transitions.

Retention

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/20ee8a926517109770884511e9fe4962e5d92f4b/day31/p3.PNG)

**Dynamic Voltage Scaling**

- Dynamic Voltage Scaling (DVS), also known as Dynamic Voltage and Frequency Scaling (DVFS), is a power management technique used in electronic systems to adjust the operating voltage and frequency of a processor or a system dynamically.
- The goal is to optimize the performance of the system while minimizing power consumption, allowing for better energy efficiency. Dynamic voltage scaling is commonly employed in scenarios where the computational workload varies, and maximum performance is not required at all times.

**Working of DVS**

- There is a direct relationship between the operating voltage and the clock frequency of a processor. Generally, increasing the voltage allows for higher clock frequencies, resulting in increased performance.
- The system continuously monitors the workload or processing requirements. This can be done through hardware performance counters, software profiling, or other mechanisms that provide information about the current computational demands.
- Based on the workload information, the system dynamically adjusts the operating voltage and frequency. When the workload is high, the voltage and frequency may be increased to achieve higher performance. Conversely, during periods of lower activity, the voltage and frequency can be decreased to conserve power.
- Dynamic voltage scaling involves a trade-off between power consumption and performance. Higher voltage and frequency settings lead to increased power consumption but provide higher performance, while lower settings reduce power consumption at the expense of performance.
- Dynamic voltage scaling is often implemented using real-time control mechanisms. These mechanisms continuously monitor the system's workload and adjust the voltage and frequency settings accordingly.
- Dynamic voltage scaling also plays a role in thermal management. As power consumption decreases with lower voltage and frequency settings, the generation of heat is reduced, contributing to better thermal efficiency.
- Dynamic voltage scaling is typically implemented in discrete steps. The system can transition between these steps based on the changing workload, allowing for a gradual adjustment of performance and power consumption.

**Challenges and Considerations** 

- Trade-off between Power and Performance:There might be trade-offs between power savings and performance. Aggressive voltage scaling might impact performance, causing slowdowns during high-demand tasks.
- Complexity and Overhead: Implementing DVS requires complex control mechanisms and algorithms, adding overhead in terms of design complexity and validation.
- Voltage-Reliability Trade-offs: Extreme voltage scaling might compromise reliability due to potential issues such as timing violations or transient faults.

**Low VDD Standby**

- Low VDD standby" typically refers to a low standby or idle power state achieved by reducing the supply voltage (VDD) of a device during periods of inactivity.
- This is a power-saving technique commonly employed in integrated circuits and electronic systems to minimize energy consumption during standby modes.

**Key Aspects**

- The supply voltage (VDD) is adjusted to a lower level during standby or idle periods. This reduces the dynamic and static power consumption of the circuit.
- Electronic devices often have different power modes, including active, idle, and standby. During standby, certain components or functions may be temporarily powered down or placed in a low-power state.
- Power gating involves selectively turning off power to specific blocks or components when they are not in use. This can be part of the strategy to achieve low VDD standby.
- Critical data or state information from the active mode may be stored in retention registers before transitioning to low VDD standby. These registers preserve important information during low-power states.
- A mechanism is usually in place to wake up the device from the low VDD standby state when it needs to become active again. This involves restoring the voltage and reactivating the necessary components.
- Achieving low VDD standby contributes to overall energy efficiency, extending battery life in portable devices and reducing power consumption in applications where energy conservation is critical.
- Low VDD standby is particularly important in embedded systems and Internet of Things (IoT) devices, where power constraints are common, and maximizing energy efficiency is a key design consideration.

**State Retention**

- State retention refers to the preservation of critical data or state information within an integrated circuit during power-down or low-power modes. When a portion of a chip enters a low-power state or is powered off, it's crucial to retain specific data in certain memory elements or registers to ensure that the device can quickly resume operation without losing essential information.
- For example, in low-power design, certain registers might store critical system configurations, context information, or data that needs to be retained during standby or power-off modes. Retention elements or specialized memory cells are employed to preserve this critical data while consuming minimal power.

**Unified Power Format (UPF)**

- Unified Power Format (UPF) is a standardized format or language used to specify low-power design intent and methodologies in electronic designs, especially for describing power intent in digital designs and ICs. UPF provides a standardized way to define power management techniques, power domains, power modes, and power control strategies within a design.
- UPF facilitates the description of power intent at various levels of abstraction, allowing designers to specify power domains, isolation strategies, retention strategies, power states, power switches, and more. It enables the representation of the design's power architecture and how the different elements of the chip interact during different power modes.
</details>

<details>
	<summary> Module 3 </summary>
Deep dive into state space

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/20ee8a926517109770884511e9fe4962e5d92f4b/day31/p4.PNG)

Power State space

The term "power state space" refers to the collection or set of possible power states that a system or device can exist in.
In the context of electronic systems, especially those with power management features, the power state space represents the different levels of power consumption and operational modes that the system can transition between.
Key components of the power state space include:

Active State: This is the operational mode where the system is fully active and performing its primary functions. It typically corresponds to the highest power consumption state.

Idle State:In the idle state, the system is operational but not actively performing tasks. Power consumption is lower than in the active state, but the system is ready to quickly resume normal operation.

Standby State : Standby is a low-power mode where certain components or subsystems are powered down, but the system remains in a state of readiness to quickly return to full operation.

Sleep State : The sleep state is a deeper power-saving mode where more components are powered down compared to standby. The system may take longer to resume normal operation from the sleep state.

Hibernation state : Hibernation is an even lower power state where the system saves its current state to non-volatile memory (such as a hard drive or flash memory) and powers down almost entirely. Resuming from hibernation involves reloading the saved state.

Off State: The off state represents the state where the system is completely powered down. This is the lowest power consumption state, and the system needs to be fully restarted to resume normal operation.

Key points

Techniques such as power gating (isolating parts of the chip when not in use), voltage scaling (adjusting voltage levels for lower power), clock gating (stopping clock signals to inactive parts), and various design methodologies help manage the power state space effectively.

Designers use power management units (PMUs) or power management integrated circuits (PMICs) to control and regulate the power delivery to different sections of the chip, enabling efficient utilization of power states based on the device's requirements at any given time. Balancing performance with power consumption is crucial in low-power IC design to prolong battery life, reduce heat dissipation, and enhance overall energy efficiency.

Low power DUT

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/20ee8a926517109770884511e9fe4962e5d92f4b/day31/p5.PNG)

A "Low power DUT" refers to a Device Under Test that is designed or configured to operate with minimal power consumption.
This can be important for various reasons, including energy efficiency, battery life, and heat dissipation considerations.
Key Aspects

A Low Power DUT is designed to consume minimal electrical power while still performing its intended functions. This is crucial for devices that operate on batteries or have strict energy efficiency requirements.
Many portable devices, such as smartphones, wearables, and IoT devices, aim to be low power to extend battery life. A Low Power DUT in this context ensures that the device can operate for longer durations on a single battery charge.
Devices that consume less power generally generate less heat. This is important for both user comfort and the longevity of electronic components. A Low Power DUT helps minimize heat dissipation issues.
A Low Power DUT may implement various power management techniques, such as dynamic voltage and frequency scaling (DVFS), power gating, and sleep modes, to optimize power consumption based on the operational state.
When testing and verifying the functionality of a Low Power DUT, it's important to consider power-related aspects, such as standby power, active power, and transitions between power states.
Low Power VMM

![image](https://github.com/Sidv005/Samsung-PD-Training/blob/20ee8a926517109770884511e9fe4962e5d92f4b/day31/p6.PNG)

A "Low Power VMM" refers to a Verification Methodology Manual designed specifically for verifying low-power aspects of digital designs.
This involves creating an effective methodology for validating and ensuring the correct functionality of circuits and systems that incorporate low-power design techniques.
Key Aspects

A Low Power VMM includes guidelines and practices for creating power-aware testbenches. These testbenches are designed to exercise and verify the low-power features of the design.
The VMM provides guidelines for setting up simulation environments that accurately model the power behavior of the design. This includes incorporating power-aware models and stimuli into the simulation.
Verification of different power states and transitions is a crucial aspect. The Low Power VMM defines strategies for checking that the design correctly enters and exits low-power states as intended.
Coverage metrics are established to ensure that the verification process adequately exercises and checks the low-power features of the design. This includes coverage of power domains, transitions, and various power management states.
If the design incorporates DVFS techniques, the Low Power VMM addresses the verification challenges associated with dynamically adjusting voltage and frequency levels during simulation.
Verification methodologies for power gating scenarios, where certain blocks or sections of the design are powered down during inactive periods, are outlined in the Low Power VMM.
Clock gating is a common low-power technique. The VMM defines strategies for verifying that clock gating is functioning correctly and that it doesn't introduce timing or functional issues.
The Low Power VMM provides guidelines for analyzing simulation results related to power consumption. This includes identifying areas of potential improvement and ensuring that the design meets power specifications.
If there are industry or internal standards related to low-power design, the VMM may include directives for ensuring compliance during the verification process.
Basic Multivoltage Terminology

In most ICs, various parts of the chip require different voltage levels for their proper operation. These voltage supply lines are commonly referred to as "rails." They provide the necessary voltages to specific sections of the chip, such as the core logic, input/output (I/O) interfaces, memory blocks, or other functional units.

Some common types of rails in IC design include:

Core Voltage Rail: This supplies power to the core logic of the chip, which includes the computational units and processing elements. It is crucial for the fundamental operation of the IC.

I/O Voltage Rail: Provides power to the input/output interfaces of the chip, enabling communication with external devices or other integrated circuits.

Memory Voltage Rail: Supplies power to the memory components (e.g., SRAM, DRAM) within the chip.

Analog/Digital Voltage Rails: Some ICs might have separate voltage rails for analog and digital circuits to ensure proper operation and avoid interference between these components.

"Multi Vdd" is a design technique used in low power design where different sections or blocks of a chip are powered by independent and separate voltage supplies. Each voltage domain, or Vdd, operates at its designated voltage level, which may differ from other parts of the chip.

The rationale behind employing multiple voltage domains in IC design is to optimize power consumption, improve performance, and address specific design requirements for different sections of the chip.

MTCMOS

MTCMOS (Multi-Threshold CMOS) power gating is a power-saving technique commonly used in low power design to reduce static power consumption in modern semiconductor devices. Static power, also known as leakage power, refers to the power dissipation that occurs even when the chip is in a standby or idle state.

MTCMOS power gating involves selectively shutting down power to specific sections or blocks of a chip when they are not in use, thereby reducing leakage current and overall power consumption. This technique is particularly effective in scenarios where certain parts of the chip are inactive for extended periods.

Working of MTCMOS

Isolation of Power Domains: The chip is divided into multiple power domains. Each domain represents a specific section or block of the chip that can be independently powered on or off. Controlled Power Switches: Within each power domain, there are dedicated power switches or transistors (often high threshold voltage transistors) known as power gates or isolation cells. These gates act as switches to control the flow of power to the domain.

Power State Transition: When a specific section of the chip is not actively in use (during idle periods or when certain functionalities are not required), the associated power gate is activated to cut off power supply to that domain. This action effectively isolates the inactive section from the rest of the chip, minimizing leakage current and reducing power consumption.

Power-Up and Power-Down Sequencing: Before activating or deactivating a power domain, careful sequencing of power-up and power-down operations is essential to prevent glitches, maintain data integrity, and ensure proper functionality when transitioning between power states.

Control and Management Logic: A power management unit (PMU) or control logic oversees the activation and deactivation of power gates based on the chip's operational requirements. It coordinates the transitions between different power states to manage power consumption effectively.

Level Shifting

Level shifting is a technique used in electronic design to convert signals from one voltage level to another. This is often necessary when connecting components or subsystems that operate at different voltage levels within the same overall system.
Level shifting ensures proper signal integrity and functionality when interfacing between devices with different voltage requirements.
Key Aspects

Different components in a system may operate at different voltage levels. For example, a microcontroller might operate at 3.3V, while a sensor or peripheral device might use a different voltage level such as 5V.
There are various methods for level shifting, and the choice depends on the specific application and requirements. Common types include resistive dividers, voltage level translators, and specialized level-shifting ICs.
In some cases, bidirectional level shifting is needed, allowing for communication in both directions. Level-shifting techniques need to accommodate bidirectional data flow while maintaining signal integrity.
Level shifting is often required for communication buses like I2C (Inter-Integrated Circuit) and SPI (Serial Peripheral Interface) where multiple devices share the same communication lines.
Dedicated level-shifting ICs are available for various voltage level conversion needs. These ICs can provide bidirectional shifting and are designed to minimize signal distortion and delay.
Level shifting is sometimes referred to as voltage translation since it involves translating signals from one voltage domain to another while preserving logical relationships.
Level shifting for buses like I2C often involves the use of open-drain or open-collector outputs. This allows for easy level translation when connecting devices with different voltage levels.
While level shifting is commonly associated with digital signals, it is also relevant for analog signals. Operational amplifiers or dedicated analog level-shifting circuits may be used for this purpose.

</details>

<details>
	<summary> Module 4 </summary>
ARM Based SOC

An ARM-based System-on-Chip (SoC) refers to a type of integrated circuit that incorporates an ARM processor as its central processing unit (CPU) along with various other components, such as memory, input/output interfaces, and peripherals, all integrated onto a single chip.
ARM (Advanced RISC Machines) is a family of reduced instruction set computing (RISC) architectures, and it is widely used in a variety of electronic devices due to its energy efficiency and performance.
Power Management Techniques

Several common power management schemes are implemented in ARM-based System-on-Chips (SoCs):

Dynamic Voltage and Frequency Scaling (DVFS): DVFS adjusts the voltage and frequency of the CPU dynamically based on the workload. This technique scales the CPU frequency and voltage to match processing demands, lowering them during low workload periods to save power and increasing them during higher workload periods to enhance performance.
CPU Power Modes (Idle States):ARM-based SoCs often incorporate multiple power states for CPUs, including idle or sleep states (e.g., C-states in ARM's terminology). These modes allow parts of the CPU to enter low-power states when not actively processing tasks. During idle times, specific CPU components are powered down or operate at reduced frequencies to conserve power.
Heterogeneous Multi-Processing (HMP):HMP architectures in ARM SoCs utilize multiple types of CPU cores with varying performance and power characteristics. This approach dynamically assigns tasks to different cores based on their power-performance trade-offs. Lower-power cores handle less demanding tasks, while higher-performance cores manage more intensive tasks, optimizing power usage.
Peripheral Power Management:ARM-based SoCs include various peripherals, such as GPUs, DSPs, and I/O controllers. Power management techniques like clock gating, power gating, and dynamic power scaling are applied to these peripherals. By selectively enabling or disabling peripherals and adjusting their operating voltages or frequencies, power consumption can be reduced.
Adaptive Voltage Scaling (AVS):AVS adjusts the voltage levels supplied to different components based on required performance. It dynamically scales the voltage to the lowest level that still maintains stable operation, reducing power consumption without sacrificing performance.
Temperature and Thermal Management:ARM SoCs often incorporate thermal management schemes to monitor and regulate temperature. Dynamic thermal management techniques, such as throttling or reducing processor speed in response to elevated temperatures, help prevent overheating while maintaining operational stability.
Software-Based Power Governors:Power governors within the operating system or firmware of ARM-based devices manage and control power states. They determine when to transition between different power modes based on system demands and user settings, contributing to efficient power management.
Conflicting events due to power management

Conflicting events in low-power design power management refer to scenarios or situations where different power-saving mechanisms or requirements clash, causing conflicts or challenges in managing power efficiently.

Voltage-Frequency Conflicts: While dynamic voltage and frequency scaling (DVFS) aim to reduce power consumption by lowering voltage and frequency during low activity, high-performance demands may conflict with this strategy. For instance, an application requiring high performance might clash with the goal of reducing voltage and frequency to save power, creating a conflict between performance and power efficiency.

Clock Gating vs. Timing Requirements:Clock gating is a strategy employed to halt clock signals to inactive blocks, aiming to conserve power. However, challenges arise when certain blocks have stringent timing requirements or dependencies that clash with the concept of clock gating. Striking a balance between power savings and meeting timing constraints can lead to conflicts.

Power Gating and Wake-up Time:Power gating involves cutting off power to inactive blocks. Nevertheless, the duration it takes to power up these blocks and return to full operation, known as wake-up time, may conflict with the need for instantaneous responsiveness in some applications. This conflict arises as a trade-off between achieving power savings and maintaining responsiveness.

Multiple Power Domains Coordination:Effectively managing multiple voltage or power domains within a chip can introduce conflicts during transitions between power states. The timing and sequencing requirements for activating or deactivating different domains may clash with overall system operation, potentially resulting in glitches or errors during transitions.

Trade-offs between Power and Functionality:Certain power-saving techniques may introduce compromises to the functionality or performance of the system. For example, overly aggressive power-saving methods might lead to degraded system performance, creating a conflict between the pursuit of power efficiency and meeting functional requirements.

Resolving conflicting events in low-power design power management involves careful trade-offs, optimizations, and compromises. Designers need to consider the specific requirements of the system, application use cases, and the balance between power-saving strategies and the overall functionality or performance goals to mitigate these conflicts and achieve an optimal balance between power efficiency and system operation.

Power Management Verification

Power management verification is a crucial aspect of the design and verification process for electronic systems, ensuring that power-saving features are correctly implemented and do not compromise the functionality or reliability of the device.
key Aspects

Utilize power-aware simulation tools to simulate the behavior of the design under different power scenarios. This involves considering dynamic voltage and frequency scaling (DVFS), power gating, and other power management techniques.
Define power intent specifications using standardized formats like UPF (Unified Power Format) or CPF (Common Power Format). These specifications describe power domains, power states, and the expected behavior of power management features.
Establish coverage metrics to ensure that the power management features are thoroughly exercised during the verification process. This includes coverage of power state transitions, power domains, and other relevant aspects.
Apply formal verification techniques to formally verify the correctness of power management features. This involves mathematical proof methods to ensure that the design meets specified power requirements.
Use emulation or FPGA prototyping to validate power management features in a hardware-like environment. This allows for more accurate assessment of power behavior and potential issues related to power domains and transitions.
Verify the proper isolation of power domains to prevent unintended interactions between different parts of the system. Incorrect power domain isolation can lead to functional and power integrity issues.
Specifically focus on verifying low-power modes, such as sleep or idle states. Ensure that the device correctly enters and exits these modes, and that critical data is retained during transitions.
Validate power gating techniques by verifying that inactive blocks are correctly powered down and brought back to full operation during wake-up. Assess the impact of power gating on wake-up time and overall system responsiveness.
Integrate power management verification into the overall regression testing framework to continuously validate power-related functionality as the design evolves.
Incorporate power-aware models during simulation to accurately model the power consumption behavior of the design. This enhances the reliability of power management verification results.
</details>

<details>
	<summary> Module 5 </summary>

Island Ordering

Island ordering, in the context of power management and design for low power, typically refers to the arrangement or sequencing of power islands within a chip or system-on-chip (SoC).

Power islands are regions of a chip that can be independently powered on or off to conserve energy when specific components are not in use. Island ordering involves determining the sequence or priority in which these power islands are activated or deactivated.

Voltage islands consist of groups of logic blocks that operate at distinct supply voltages. Strategically placing voltage islands with similar voltage levels in close proximity allows designers to minimize the length of power supply wires. This reduction in wire length diminishes voltage drop across the wires, consequently lowering power consumption.

Two primary approaches exist for island ordering: top-down and bottom-up.

In the top-down approach, the chip is partitioned into voltage islands based on a high-level power analysis. While relatively simple to implement, this method may not be as effective as the bottom-up approach. Bottom-up island ordering involves a more detailed power analysis to optimize the placement of individual logic blocks. This intricate approach has the potential for greater power savings.

The bottom-up method utilizes a power grid analysis tool to identify the optimal placement of individual logic blocks. This tool considers the power consumption of each logic block, as well as the resistance and capacitance of the power supply wires. After determining the optimal placement, the designer arranges the voltage islands on the chip, aiming to group islands with similar voltage levels closely and minimize the length of power supply wires.

Island ordering serves as a valuable technique in low-power design, enabling designers to reduce power consumption by optimizing the placement of voltage islands. The focus on minimizing power supply wire length contributes to overall power efficiency in electronic systems.

Power Formats

Power formats are standardized representations that facilitate the description, analysis, and optimization of power-related aspects in electronic designs, particularly in the context of low-power integrated circuit (IC) design.
These formats provide a common language for design tools and methodologies to understand and implement power management strategies.
Some commonly used power formats:

Unified Power Format (UPF):

Definition: UPF is an industry-standard power format defined by the IEEE 1801 standard.
Purpose: UPF provides a comprehensive framework for expressing power intent, including specifications for supply voltages, power domains, leakage models, and power-aware design constraints.
Features: Supports hierarchical power management, allowing designers to specify power intent at different levels of abstraction.
Power Analysis Markup Language (PAM-XML):

Definition: PAM-XML is an XML-based power format developed by Mentor Graphics.
Purpose: Designed for early-stage power analysis and estimation, PAM-XML is lightweight and user-friendly.
Features: While less comprehensive than UPF, it offers a simpler and more intuitive syntax, making it suitable for quick power assessments.
Common Power Format (CPF):

Definition: CPF is a power format developed by Synopsys.
Purpose: Similar to UPF, CPF provides features for power-aware synthesis and optimization.
Features: Supports power-aware clock tree synthesis, power-aware scan insertion, and other power-saving techniques.
PowerIntent (PI):

Definition: PowerIntent is a power format developed by Cadence Design Systems.
Purpose: Gaining popularity for its support of power-aware design in advanced process technologies.
Features: Offers advanced features for power modeling, including considerations for leakage currents, crosstalk effects, and power grid analysis.
Note

Choosing the appropriate power format depends on various factors, including the design methodology, tools in use, and the level of detail required for power analysis. Each format has its own strengths and may be better suited to specific stages of the design process or certain design goals.
UPF

UPF, or Unified Power Format, is an industry-standard power format defined by the IEEE 1801 standard. It plays a crucial role in low-power integrated circuit (IC) design by providing a standardized framework for expressing power intent.
Power intent refers to the designer's specifications and intentions related to power management strategies within the electronic design.
Key Aspects

UPF allows designers to describe various power-related aspects, including supply voltages, power domains, and power modes. It provides a comprehensive language for specifying the behavior of the design concerning power consumption.
Designers can use UPF to define different supply voltages within the design. This includes specifying voltage levels for various power domains or sections of the circuit.
UPF supports the definition of power domains, which are groups of elements within the design that can be powered on or off independently. This allows for efficient power management by selectively activating or deactivating specific parts of the circuit.
Different power modes represent the operational states of the design with varying power requirements. UPF enables designers to articulate the conditions under which the design transitions between these power modes.
UPF supports hierarchical power management, allowing designers to specify power intent at different levels of abstraction. This hierarchical approach is valuable in managing complex designs with multiple levels of hierarchy.
Designers can use UPF to model and specify leakage currents, which are currents that flow through a transistor even when it is supposed to be in a non-operational state. Managing leakage is crucial for optimizing power consumption in low-power designs.
Various EDA tools provide support for UPF, allowing designers to seamlessly integrate power management strategies into their design flows.
Application of UPF

UPF allows designers to define power domains, which are groups of logic elements that can be powered on or off independently. This is crucial for managing power consumption by selectively activating or deactivating specific parts of the circuit.
Designers use UPF to specify different supply voltages within the design. This includes defining voltage levels for various power domains or sections of the circuit, contributing to efficient power management.
UPF enables the description of different power modes representing distinct operational states of the design with varying power requirements. Designers can specify the conditions for transitions between these power modes.
UPF supports the modeling of leakage currents, which are currents that flow through transistors when they are in a non-operational state. Managing leakage power is essential for optimizing power consumption in low-power designs.
UPF facilitates hierarchical power management, allowing designers to specify power intent at different levels of abstraction. This hierarchical approach is particularly valuable for complex designs with multiple levels of hierarchy
Power gating involves selectively shutting down power to certain portions of the circuit when they are not in use. UPF provides a standardized way to describe power gating strategies, specifying when and how power can be gated to save energy.
Clock gating is a technique where clock signals to inactive blocks are stopped to save power. UPF allows designers to describe clock gating strategies, specifying when and how clock signals can be gated.
Impact of UPF on low power design

Facilitating Standardization: UPF has introduced a standardized approach for expressing power intent, fostering smooth communication across design teams and Electronic Design Automation (EDA) tools.

Boosting Power Efficiency: Techniques derived from UPF-based power optimization have resulted in notable reductions in power consumption, contributing to the creation of smaller and more energy-efficient designs.

Optimizing Design Flow: UPF has streamlined the design flow by automating power management tasks and seamlessly integrating power-related information throughout the design process.

Enhancing Design Productivity: The adoption of UPF has enhanced design productivity by minimizing the time and effort required for managing and optimizing power consumption in electronic designs.
</details>
