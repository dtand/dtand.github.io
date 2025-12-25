---
layout: page
title: CHIP-8 Emulator
permalink: /projects/chip8/
---

![Chip8](/assets/images/chip8.png)

## Overview
A CHIP-8 emulator written in C++ using SDL3 for graphics and input. This project allows you to run classic CHIP-8 ROMs and experiment with emulator development.

## Technologies Used
- **C++**: core programming language

## Description
This project implements a fully functional CHIP-8 emulator including all required opcodes.  The project uses SDL3 for the event looping and implements a logging system used for forwarding memory address changes to file-backed storage.  Eventually the goal was to experiment with training a model that could generate patch files using information output from the emulator.

## Key Features
- Fully working emulator compatible with CHIP-8 ROMs

## What I Learned
I learned about various instructions used for CHIP-8 as well as how to set up SDL3 for use with event handling.

## Links
- [GitHub Repository](https://github.com/dtand/chip8-emulator) 

[← Back to Projects](/projects/)
