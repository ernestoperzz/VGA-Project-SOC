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

The ColourStripes example was basically different assigned RGB values that were continuosly displayed on an horizontal pixel position. Then, the ColourCycle template switches between different RGB values where each of them was displayed as a backgound (one by one).  
### **Simulation**
Simulation is a technique for applying different inputs to the design at different times to check if the RTL code behaves in an intended way by running a testbench that drives a clock that it is generated on the testbench. It also allows throwing design and testbench signals into a waveform that can be graphically represented to analyze and debug the RTL design if it works. 
### **Synthesis**
Describe the synthesis and implementation processes. Consider including 1/2 useful screenshot(s). Guideline: 1/2 short paragraphs.
### **Demonstration**


<img source = "https://github.com/ernestoperzz/VGA-Project-SOC/ImagesSOC/"416209b7-a9a6-4e23-9c80-35b563bd8397.jpg">




## **My VGA Design Edit**
Introduce your own design idea. Consider how complex/achievabble this might be or otherwise. Reference any research you do online (use hyperlinks).

![efa70bcc-660f-447d-a1d0-031b6a06237b](https://github.com/user-attachments/assets/75bc34c2-1d74-4f4f-a9b8-b5939ab986f9)

![618144d1-36cd-4dc7-995a-2d424248926b](https://github.com/user-attachments/assets/0b16bd5b-5e3b-4565-b947-4a4366efedc0)

![8b234de8-838a-46d0-b9ab-ee1ae2d3162c](https://github.com/user-attachments/assets/ccc94681-bc4c-4cdf-8558-265b15270062)

### **Code Adaptation**
Briefly show how you changed the template code to display a different image. Demonstrate your understanding. Guideline: 1-2 short paragraphs.
### **Simulation**
Show how you simulated your own design. Are there any things to note? Demonstrate your understanding. Add a screenshot. Guideline: 1-2 short paragraphs.
### **Synthesis**
Describe the synthesis & implementation outputs for your design, are there any differences to that of the original design? Guideline 1-2 short paragraphs.
### **Demonstration**
If you get your own design working on the Basys3 board, take a picture! Guideline: 1-2 sentences.

https://github.com/user-attachments/assets/7262f9b6-c441-4661-b860-63886d0990d4

## **More Markdown Basics**
This is a paragraph. Add an empty line to start a new paragraph.

Font can be emphasised as *Italic* or **Bold**.

Code can be highlighted by using `backticks`.

Hyperlinks look like this: [GitHub Help](https://help.github.com/).

A bullet list can be rendered as follows:
- vectors
- algorithms
- iterators

Images can be added by uploading them to the repository in a /docs/assets/images folder, and then rendering using HTML via githubusercontent.com as shown in the example below.

<img src="https://raw.githubusercontent.com/melgineer/fpga-vga-verilog/main/docs/assets/images/VGAPrjSrcs.png">
