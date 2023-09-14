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



