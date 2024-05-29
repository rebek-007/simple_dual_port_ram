
# Simple Dual Port RAM 

Simple Dual Port RAM has 2 ports; one for read port and the other for write port. 

 To initialise all the signals, we take a delay of 20 seconds.
 
We enable wr_en(write enable) for 150ns. With that , we can clearly see the write operation.

We disable wr_en(write enable) for 150ns. With that , we can clearly see the read operation.  

## Deployment

To deploy this project clone this github repository and extract the files to VS Code. 

If you wish to simulate the timing diagram of simple dual port ram, enter 
```
iverilog -o sim simple_dual_port_ram_testbench.v
```
A simulation output of sim is created as the output file . To generate the timing diagram of sim , enter 
```
vvp sim
```

If we wish to simulate simple_dual_port_ram , then following command is given
```
gtkwave simple_dual_port_ram.vcd
```
A timing diagram will be generated by GTKwave Analyser. We can analyse the output signals as per our requirement. 


![timing diagram]([relative%20path/to/img.jpg](https://github.com/rebek-007/simple_dual_port_ram/blob/master/simple_dual_port_ram_timing_diagram.png)?raw=true "Title")
