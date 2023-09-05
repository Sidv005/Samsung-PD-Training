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
*.lib* : A design library housing standard cells.
*.db* : Similar to .lib, but in an alternate format that DC (Design Compiler) can comprehend, libraries are provided in .db format.
*.ddc* : Synopsys uses its own exclusive format called DDC for storing design data, and DC (Design Compiler) has the ability to both produce and interpret this format.
*Design* : RTL files which has the behavioral model of the design.
</details>

***SDC : Synopsys Design Constraints***
The SDC format defines design intentions regarding timing, power, and area constraints, with power described using UPF. SDC commands can extract UPF information. This format is compatible with various EDA tools in the semiconductor industry and is built upon the Tool Command Language (Tcl).

***DC Setup:***
The DC setup process involves taking RTL files, .lib files (similar to Yosys), and SDC files as inputs to produce gate-level netlists, DDC format files, and synthesis reports as outputs.
The ASIC flow is the steps involved in converting RTL to the Graphical Data set(GDS). The Application Specific IC flow is shown in figure below:
<img width="1085" alt="ASICflow" src="https://github.com/Sidv005/Samsung-PD-Training/blob/23a9599941c49214a1e3a55031833afe2746c3db/SamsungPD%23day6/ASICflow.jpeg">
- The DC Synthesis process can be described in the following manner: In this scenario, the "Design.lib" is a specific design library, distinct from the standard .lib or technology library, and it may represent third-party intellectual property (IP) or pre-designed modules. The Design Compiler ensures that the connections of inputs and outputs from this module are correctly integrated into the overall design and optimizes the logic accordingly.

- The Design Compiler reads the Verilog files of the design, along with the standard library files and constraints, and generates reports as it links and synthesizes the design. Eventually, it produces a netlist as its final output. The DC Synthesis flow is given below in the figure.
<img width="1085" alt="dc_synth" src="https://github.com/Sidv005/Samsung-PD-Training/blob/7662963a9a31c04b318faed24f35b77eb406fb9e/SamsungPD%23day6/dc_synth.png">

***Invoking dc basic setup***
- We understand that the library name contains crucial information regarding the PVT (Process, Voltage, Temperature) conditions under which a design operates. The performance of any electronic circuit is influenced by factors like voltage, temperature, and manufacturing process. Therefore, a unique .lib file is defined for each PVT corner, with this particular PVT corner representing typical conditions at 25°C temperature and 1.8V voltage.

- Within the .lib file, you can find valuable data such as the units for resistance (R), inductance (L), capacitance (C), time measurements, technology specifications, and the various versions or flavors of each cell.

- To initiate the DC (Design Compiler) shell, the following commands are executed:

```ruby
$ csh
$ dc_shell
dc_shell> 
```
To initiate the process, we must activate the C shell and subsequently launch the DC shell. Within the DC shell, a series of license checks are performed for various compilers, including the VHDL compiler, HDL compiler (used for interpreting Verilog or other Hardware Description Languages), DFT compiler (for enabling scan stitching), Design Vision (the graphical version of DC), and Power Compiler (essential for power-aware synthesis).

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
module lab1_flop_with_en
endmodule
```
The dc shell reads lib files in .db format.

```ruby
dc_shell> read_db ~/DC_WORKSHOP/lib/sky130_fd_sc_hd_tt_025c_1v80.db
dc_shell> sh gvim lab1_net.v &
```
The resulting netlist appears as follows: The cells are within SEQGEN, but they are not in the sky130 cell format. This situation arises because no file has been designated for the target and link library. "gtech" serves as the virtual library within DC's memory, used to interpret the design.

```ruby
dc_shell> set target_library /home/usha.m/DC_WORKSHOP/lib/sky130_fd_sc_hd_tt_025c_1v80.db
dc_shell> set link_library {* <path to standardcell library> }
dc_shell> link
dc_shell> compile
dc_shell> write -f verilog -out lab1_net_with_sky130.v
```
Upon assigning files to the libraries, the design is linked and compiled in the following manner. In this process, the link_library is specified to append data to the existing list without replacing it. Consequently, the resulting outnetlist is as follows:
</details>

<details>
<summary>Labs on Tcl Scripting</summary>
The Tool Command Language (Tcl) is employed for crafting SDCs.
	
**Set**
- It is utilized for generating and assigning variables.
- For example, set a 5 --> a=5
- set a [expr $a+$b] --> a=a+b
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

**foreach_in_collection**
The command "foreach_in_collection" is specific to DC (Design Compiler).
```ruby
foreach_in_collection var collection {
   statements
 }
```
</details>
