# How to Simulate Siemens S7-200 PLC with PC-Simu Software
 
Siemens S7-200 PLC is a popular and widely used programmable logic controller that can be used for various industrial applications. However, sometimes it is not possible or convenient to test the PLC program on a real hardware. In such cases, simulation software can be very helpful to verify the logic and functionality of the program without connecting to a physical device.
 
**Download Zip ››› [https://searchdisvipas.blogspot.com/?download=2uLv3U](https://searchdisvipas.blogspot.com/?download=2uLv3U)**


 
One of the simulation software that can be used with Siemens S7-200 PLC is PC-Simu. PC-Simu is a free and easy-to-use software that can simulate the inputs and outputs of the PLC and display them on a graphical interface. PC-Simu can also communicate with another software called S7-200 Simulator, which can emulate the CPU and memory of the PLC and run the program written in Step 7 MicroWin software.
 
In this article, we will show you how to use PC-Simu and S7-200 Simulator to simulate a Siemens S7-200 PLC program. We will also demonstrate a simple example of a bottle filling project that uses some basic instructions such as memory bits, counters, timers, and positive edge detection.
 
## Step 1: Download and Install PC-Simu and S7-200 Simulator
 
The first step is to download and install PC-Simu and S7-200 Simulator software on your computer. You can find the download links below:
 
- PC-Simu: [http://www.mediafire.com/file/hihe724...](http://www.mediafire.com/file/hihe724...)
- S7-200 Simulator: [http://www.mediafire.com/file/o06so56...](http://www.mediafire.com/file/o06so56...)

Note that you also need to have Step 7 MicroWin software installed on your computer to write and compile the PLC program. You can download it from here: [https://www.youtube.com/watch?v=dvduZ...](https://www.youtube.com/watch?v=dvduZ...)
 
siemens s7200 simulation with s7200 simulator and pc simu,  how to connect pc simu with siemens s7200 simulator,  bottle filling project with siemens s7200 and pc simu,  s7 200 simulator v4.0 full download,  how to use s7 200 simulator v4.0,  dotnet 3.5 for s7 200 simulator,  palamela/siematic-s7-200-pc-simu docker hub,  how to simulate automatic processes with pc simu,  plc programming and simulation with siematic s7 200 pc simu,  cable pc-ppi for communication with s7 200 simulator,  siematic s7 200 pc simu pdf,  how to run s7200 simulator on win 10,  animation not shown in s7200 simulator,  siematic s7 200 pc simu tutorial video,  siematic s7 200 pc simu youtube,  siematic s7 200 pc simu crack,  siematic s7 200 pc simu free download,  siematic s7 200 pc simu software,  siematic s7 200 pc simu online,  siematic s7 200 pc simu manual,  siematic s7 200 pc simu serial key,  siematic s7 200 pc simu license code,  siematic s7 200 pc simu activation key,  siematic s7 200 pc simu registration key,  siematic s7 200 pc simu keygen,  siematic s7 200 pc simu review,  siematic s7 200 pc simu features,  siematic s7 200 pc simu system requirements,  siematic s7 200 pc simu installation guide,  siematic s7 200 pc simu user guide,  siematic s7 200 pc simu troubleshooting tips,  siematic s7 200 pc simu support forum,  siematic s7 200 pc simu latest version,  siematic s7 200 pc simu update download,  siematic s7 200 pc simu patch download,  siematic s7 200 pc simu alternative software,  siematic s7 200 pc simu comparison with other plc simulators,  siematic s7 200 pc simu benefits and drawbacks,  siematic s7 200 pc simu pros and cons,  siematic s7 200 pc simu best practices and tips,  siematic s7 200 pc simu case studies and examples,  siematic s7 200 pc simu testimonials and feedbacks,  siematic s7 200 pc simu ratings and reviews,  siematic s7 200 pc simu pricing and plans,  siematic s7 200 pc simu discount and coupon codes,  siematic s7 200 pc simu affiliate program and commission rates,  siematic s7 200 pc simu reseller program and benefits,  siematic s7 200 pc simu partner program and perks,  how to buy or order siematic s7 200 pc simu online
 
## Step 2: Write and Compile the PLC Program in Step 7 MicroWin
 
The next step is to write and compile the PLC program in Step 7 MicroWin software. You can use any programming language that is supported by the software, such as ladder logic, statement list, or function block diagram. For this example, we will use ladder logic to implement a simple bottle filling project.
 
The logic of the project is as follows:

1. When the start button (I0.0) is pressed, the conveyor motor (Q0.0) starts running and moves the bottles towards the filling station.
2. When a bottle reaches the filling station, a sensor (I0.1) detects it and triggers a positive edge detection instruction (M0.0).
3. The positive edge detection instruction activates a counter (C0) that counts how many bottles have been filled.
4. The counter output (C0.Q) activates a timer (T0) that controls how long the filling valve (Q0.1) should be opened for each bottle.
5. The timer output (T0.Q) deactivates the filling valve (Q0.1) and resets the counter (C0) for the next bottle.
6. The process repeats until the stop button (I0.2) is pressed or the maximum number of bottles (10) is reached.

The ladder logic diagram of the program is shown below:

    +----[ ]----+----[ ]----+----( )----+
    | I0.0      | I0.2      | Q0.0      |
    +-----------+-----------+-----------+
    | Start     | Stop      | Conveyor  |
    +----[ ]----+----[P]----+----( )----+
    | I0.1      | M0.0      | C0        |
    +-----------+-----------+-----------+
    | Sensor    | Posedge   | Counter   |
    +----[ ]----+----( )----+
    | C0.Q      | T0        |
    +-----------+-----------+
    | Counter 8cf37b1e13

    
