# Eurorack PSU

A simple linear adjustable power supply for modular synthesizers in the Eurorack format.  
It's easy to build and outputs more than $1A$ at $+12V$, $-12V$ and $+5V$ each.

![bus board assembled](/pictures/eurorack_psu_v010_assembled.jpg?raw=true "psu assembled")
*Eurorack_PSU v0.1.0*

## Motivation

I designed this power supply for use in my own modular synthesizer projects. Thought i'd share the board with other synth builders.
(Gerber files in the repo can be directly uploaded to your pcb manufacturer of choice. Interactive BOM for easy assembly included.)

## A few words of caution

**DANGER OF DEATH:** Do not attempt to build this project if you do not fully know what you are doing!!!  
The build requires wiring a transformer to mains voltage, which can easily end in a deadly accident if done incorrectly!  

![danger of death warning sign](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fupload.wikimedia.org%2Fwikipedia%2Fcommons%2Fthumb%2Ff%2Ffd%2FDANGERBOARD01.png%2F240px-DANGERBOARD01.png&f=1&nofb=1?raw=true "danger of death warning sign")

**CAUTION:** This project is not suited for beginners! Use the files in this repository at your own risk!  

<hr style="border:1px solid gray">

If you do know what you are doing and want to build the PSU:

I will do my best to test everything, but the occasional bug might still find its way into the project files. Don't hesitate to report found bugs or share ideas on how to improve the board.

## Project status

The *main* branch of this repository holds the current tested version of the board. All potentially breaking changes will be done on the *develop* branch and the build will be tested before merging. Images in this README do not necessarily show the most recent version of the board, though all images will have version numbers in their title.  

## Tech/framework used

- KiCad

## Features

- Designed for standard $+12V$, $-12V$, $+5V$ power ($\pm 15V$ should also be possible by adjusting the potentiometers).  
- $\approx 1.3A$ per rail (regulators are rated $1.5A$ abolute maximum)
- Three LEDs indicate the rails being powered.
- Little heat generation
- Fuses on both secondary windings

## Installation

M3 screws and PCB spacers can be used to mount the board to the back of a case.  
Regular 6.3mm flat connectors are used for connecting to both transformer and bus board.
Use a toroidal transformer with split secondaries at 15VAC (choose one capable of driving enough current to meet your needs! Both positive rails are powered by the same transformer winding.)

## How to use?

*(TODO!: Write usage instructions incuding calibration and setup)*

## How to build?

Upload the *.zip* in the `gerber_files/` folder to your PCB manufacturer's website to order.

An interactive HTML BOM is available in the `bom/` folder. Just open it in a browser and tick off sourced/placed components.  
Also shows where on the board components should be placed.  

**HINT:** Use good quality solder/flux and clean the board thoroughly after soldering!  

## Component availability/choices

No unobtainium in this project. All components should be easily sourced, at least in europe.  
Feel free to recommend more easily available parts if you can think of any worth replacing.

## Contact

Any questions?   

🡢 contact[at]butchwarns.de

## License

*(TODO: Find appropriate open-hardware license!)*

> Until otherwise stated here, the project is default licensed as proprietary.

Build as many of these boards as you want for personal use, but please make it obvious if your build has modified the project files in any way to avoid confusion!  

My name and any logo of mine that might me present on the board design are copyrighted and are not free to use.

You are free to share the images in the `pictures/` folder of this repository with correct attribution or a link to the project.  

Copr. 2021, Butch Warns
