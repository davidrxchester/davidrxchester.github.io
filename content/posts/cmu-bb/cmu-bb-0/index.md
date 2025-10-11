+++
title = "cmu binary bomb lab introduction"
date = "2024-08-15T23:19:00-04:00"
draft = false
categories = ["cmu-binary-bomb"]
featured_image = "img/computer.jpg"
+++
<!--more-->


>This is a warning: This folder contains solutions and my personal walk through to this challenge. I do not want to spoil the fun for others, so only proceed if you have done the lab or do not plan to. Or read this and go do the lab after. Don't let me tell you how to live your life.
{: .prompt-warning}

## **Introduction** 

The CMU Binary Bomb lab is a reverse engineering challenge derived from the Carnegie Mellon University (CMU) Computer Architecture course. Here is a link to the [course](https://csapp.cs.cmu.edu/) and also a link to the [Official Binary Bomb lab](https://www.cs.cmu.edu/afs/cs/academic/class/15213-s02/www/applications/labs/lab2/bomblab.html). It is commonly used in computer security courses, such as [OpenSecurityTraining2](https://p.ost2.fyi/dashboard) Architecture 1001. The challenge presents itself as a binary executable that is known as a 'bomb'. The goal of the challenge is to 'defuse' the bomb by providing the correct input for each of the 6 phases of the challenge. Failure to input the correct answer results in the binary 'exploding', which is indicated by a message and metaphorically, a failure in the challenge. The purpose of this challenge is to be a 'weed out' for introductory reverse engineering courses, as it is the final challenge faced in Architecture 1001, which is the gateway to many other reverse engineering courses provided by OpenSecurityTraining2.



### Some background on the challenge

The Binary Bomb Lab is designed to reinforce knowledge of assembly language, the behavior of compiled code, and debugging techniques. Participants must use a combination of static and dynamic analysis tools, such as GDB (GNU Debugger) or other disassemblers, to dissect the binary, understand its logic, and discover the correct inputs for each phase.

The challenge comprises 6 phases, each increasing in complexity. Solvers must methodically analyze the code, identify critical instructions, and derive the correct inputs needed to progress to the next phase. This process not only sharpens reverse engineering skills but also deepens the understanding of how high-level programming constructs are translated into machine code.

The lab serves as a practical application of concepts learned in systems programming, including control flow, memory management, and data representation. By the end of the challenge, participants gain hands-on experience with debugging and reverse engineering techniques that are essential for careers in cybersecurity and software development.


#### Tools used

Since I am already quite familiar with x64Dbg, Ghidra, and a few other tools, I decided to use [WinDbg](https://learn.microsoft.com/en-us/windows-hardware/drivers/debugger/) to get familiar with a new debugger. 


I hope this introduction piqued your interest on this challenge. If you like complex challenges, I highly encourage you to go attempt the CMU Binary Bomb before reading through my walk through. With that being said, the next 6 posts in this category will be my appraoch and solution to each of the phases. 

Enjoy <3