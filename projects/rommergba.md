---
layout: page
title: RommerGBA
permalink: /projects/rommergba/
---

![RommerGBA](/assets/images/rommer-gba-001.png)

## Overview
RommerGBA is a locally deployed web application designed to assist in reverse engineering of Game Boy Advance ROMS using machine learning and AI-based approaches.  This project is an R&D tool which aids in reverse engineering.

## Technologies Used
- **JavaScript React w/ Typescript**: web application frontend
- **Python REST Flask**: APIs for web application
- **Python PyTorch**: CNN training and LLM training
- **BizHawk**: GBA emulator
- **Lua**: scripts that run in BizHawk
- **Ghidra**: disassembly of GBA ROM

## Description
The core goal of RommerGBA is to create a multi-AI system used for reverse-engineering of GBA ROMs. The intended workflow is as follows:

1. User opens BizHawk emulator and loads in Lua script
2. Every n frames, WRAM and IRAM are exported to log files
3. Scripts in the backend are used to organize the data for use in the web app
4. User annotates many frames in the web application and trains a CNN to classify game scenes

It is noted that we are able to create CNN classifiers with > 90% accuracy classifying various scenes from the tested GBA ROM "Medabots: Rokusho Version."  

Once the classifier has been created, the intention is to complete development to test the following strategies for AI-driven reverse engineering:

1. Next train an LLM on IRAM and WRAM deltas
2. Combine CNN classifier and LLM to provide high level details on game events while user is playing
3. Train another LLM to produce patch files in the assembly code
4. User tests patch files, annotates results and feeds back to the LLM

Eventually with enough iterations the patch file generation LLM is intended to learn the context and meaning of the underlying assembly code.  This second set of steps are not implemented yet, but were ideas that are eventually intended to be tested in a multi-agent system.

Lastly, the eventual goal was to see if it is possible to pull this integrated system into a single web application where a user could do the following:

1. Upload a GBA ROM, and a set of changes the user would like to make to the underlying game
2. Trained patch generator generates a "hacked" ROM

## Key Features
- Web application for annotating frame data exported from BizHawk
- Backend scripts for data analysis and machine learning
- Lua script for exporting WRAM and IRAM from live game

## What I Learned
This project tackled a lot of areas. I revisited REST Flask which I haven't used in a long time and additionally explored some new technologies. The most notable being the Ghidra disassembly and decompiler tool, which was originally developed by the NSA and later released for public use. It is an extremely powerful tool. Additionally, I worked with Lua a bit and learned how to load custom scripts into BizHawk to pull data out of a running emulated game. I also learned a bit about training CNNs and LLMs using PyTorch.

## Links
- [GitHub Repository](https://github.com/dtand/rommer-gba)

[← Back to Projects](/projects/)
