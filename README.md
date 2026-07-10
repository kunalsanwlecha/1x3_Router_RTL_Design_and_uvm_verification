RTL Design and Implementation of 1x3 Router
This RTL Design of the Project was completed in 2017 and verification testbench was added later in 2019. It contains RTL Implementation of a basic Router1x3 (Single Ingress, 3 Egress Ports). It is designed accepts data packets on a single 8-bit port and routes them to one of the three output ports.

Router 1x3 Block Diagram: 

<img width="843" height="453" alt="image" src="https://github.com/user-attachments/assets/6cfcfad7-9e67-45a4-9695-604cc98e6b91" />

<img width="1081" height="601" alt="router" src="https://github.com/user-attachments/assets/c5e16a68-906b-49fa-a5f6-321fd32dc3c6" />

FSM:- 

<img width="948" height="516" alt="image" src="https://github.com/user-attachments/assets/d84e5e08-d1a5-477f-bf68-25e8184582dc" />

FIFO:-

<img width="840" height="449" alt="image" src="https://github.com/user-attachments/assets/9105a8be-a9d9-4630-b903-078e0108c7ce" />




Functionality:

Input Register: This block is responsible for extracting the header, calculating and checking the parity.
Synchronizer: This block is responsible for decoding the header and determining the output portIt also provides synchronization between FSM and FIFO Modules. It allows faithful communication between the input port and the output port.
FSM: This block is basically a controller for the router. It generates necessary controls for FIFO, Synchroniser based on the values of status signals.
FIFO: This is an synchronous active low reset FIFO which allows simultaneous read and write operations.
Steps covered during the project:

Designed a the block level structure for the Router.
Implemented the RTL Design using Verilog HDL and verified using individual verilog testbenches.
Synthesized and Implemented the design to generate a bit file and tested on FPGA.
Developed the class based verification environment and verified the 1x3 Router RTL model in system verilog using UVM Methodology.
Generated functional and code coverage for the RTL verification sign-off.

KUNAL SANWLECHA
