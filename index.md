---
layout: home
title: FPGA VGA Driver Project
tags: fpga vga verilog
categories: demo
---

Welcome to my SOC project where I will walk through my FPGA VGA Driver project. In this project, I will document from the initial concept and design choices all the way to implementation, testing, final results and everything I learned during this project!

## **Template VGA Design**
### **Project Set-Up**
In this project, I used the VGA template given to start with and adjusted it to make my own landscape. I started by creating a new vivado project, added the files and constraint given and modifying some parameters before getting the stripes template output desired. Then, I coded on my own in order to get the landscape I was looking for and with spare time I was able to switch between two different images on a VGA monitor after synthesising, implementing and simulated the design in Vivado.

<img src="https://raw.githubusercontent.com/melgineer/fpga-vga-verilog/main/docs/assets/images/VGAPrjSum.png">
## **Template Code**
The template verilog files provided by Michelle define the basics in VGA design where we can generate 3 RGB signals(red, gree, blue) using VGA timers. I personally found them handy and gave me a better understanding on
VGA design code before adapting the given one.

The ColourStripes example was basically different assigned RGB values that were continuosly displayed on an horizontal pixel position. Then, the ColourCycle template switches between different RGB values where each of them was displayed as a background (one by one).  
### **Simulation**
Simulation is a technique for applying different inputs to the design at different times to check if the RTL code behaves in an intended way by running a testbench that drives a clock that it is generated on the testbench. It also allows throwing design and testbench signals into a waveform that can be graphically represented to analyze and debug the RTL design if it works. 
### **Synthesis**
The synthesis proccess beasically translates the RTL code into a generic netlist representing the designs logic. Then, the implementation process takes the synthesized netlist and constraints and makes a bitstream file that programs the FPGA.
### **Demonstration**


<img src="https://raw.githubusercontent.com/ernestoperzz/VGA-Project-SOC/main/ImagesSOC/416209b7-a9a6-4e23-9c80-35b563bd8397.jpeg">



## **My VGA Design Edit**
At the start my main idea was working on just a complex image where there would be a cowboy standing in the grass full of flowers. However, I decided to change my design idea into a landscape where we could switch into a saturated version of the landscape as it will proof my deeper understanding into my FPGA VGA Driver Project. I personally found more challenging to be able to switch between different images than making a complex image as it will just require a longer code to make a harder image and I would learn how to initialize and configure any type of switches for future projects.  

<img src="https://raw.githubusercontent.com/ernestoperzz/VGA-Project-SOC/main/ImagesSOC/efa70bcc-660f-447d-a1d0-031b6a06237b.jpeg">

<img src="https://raw.githubusercontent.com/ernestoperzz/VGA-Project-SOC/main/ImagesSOC/618144d1-36cd-4dc7-995a-2d424248926b.jpeg">

<img src="https://raw.githubusercontent.com/ernestoperzz/VGA-Project-SOC/main/ImagesSOC/8b234de8-838a-46d0-b9ab-ee1ae2d3162c.jpeg">

### **Code Adaptation**
Briefly show how you changed the template code to display a different image. Demonstrate your understanding. Guideline: 1-2 short paragraphs.

<img src="https://raw.githubusercontent.com/ernestoperzz/VGA-Project-SOC/main/ImagesSOC/Code.png">
<img src="https://raw.githubusercontent.com/ernestoperzz/VGA-Project-SOC/main/ImagesSOC/Code2.png">
<img src="https://raw.githubusercontent.com/ernestoperzz/VGA-Project-SOC/main/ImagesSOC/Constraintfile.png">
### **Simulation**
Show how you simulated your own design. Are there any things to note? Demonstrate your understanding. Add a screenshot. Guideline: 1-2 short paragraphs.

<img src="https://raw.githubusercontent.com/ernestoperzz/VGA-Project-SOC/main/ImagesSOC/Simulation.png">
### **Synthesis**
Describe the synthesis & implementation outputs for your design, are there any differences to that of the original design? Guideline 1-2 short paragraphs.

<img src="https://raw.githubusercontent.com/ernestoperzz/VGA-Project-SOC/main/ImagesSOC/Synthesis.png">
### **Demonstration**
Here is the final desing of my SOC project. I did not manage to generate a saturatedThis is an optimized version of the video demonstration turned into a gift as in Github you are only allowed to upload files under 25mb. Below there is a link to download the original version of the mp4 file.

<img src = "https://raw.githubusercontent.com/ernestoperzz/VGA-Project-SOC/main/SmallOptimizedVideo.gif">

![Please download video demo here.](https://raw.githubusercontent.com/ernestoperzz/VGA-Project-SOC/main/FinalProjVideo.mp4)

## **References**

