# PRANCE: Phage-and-Robotics Assisted Near-Continuous Evolution

PRANCE is a new method for phage-assisted evolution of biomolecules.

For a Hamilton robot to be PRANCE-compatible, certain equipment must be installed.

## How to enable PRANCE on a Hamilton Microlab STAR

The most general requirements for running PRANCE are a way to load multiple
sources of constant OD bacteria culture onto the robot deck, a way to wash and
sterilize tips for reuse, and a way to automatically obtain real-time spectrophotometric 
measurements from phage-inoculated bacteria culture on the deck.

This guide outlines certain equipment, configurations, and practices that
the authors have found to be the easiest and most widely accessible means
of running PRANCE on a Hamilton Microlab STAR.

https://www.biorxiv.org/content/10.1101/2020.04.01.021022v1

### P&ID for Liquid Flow-paths
![alt text](https://github.com/Golaszewski/PRANCE/blob/main/Extras/pid.png)

### Deck Layout Diagram
![alt text](https://github.com/Golaszewski/PRANCE/blob/main/Extras/decklayout.svg)


### Pumps
Agrowtek AD6i dosing pump is recommended for the custom pump array.

https://www.agrowtek.com/index.php/products/dosing_systems/dosing-pumps/agrowdose-adi-digital-persitaltic-dosing-pumps-detail

For installation refer to the perma_pump folder.

### Orbital Shaker

The orbital shaker is fitted to the waffle. Refer to the perma_shaker folder for installation.

http://www.bigbearautomation.com/HT91108.htm

### Waffle

The waffle is a 3D printed part designed by the authors which is used as a staging point for bacteria culture loaded onto the deck. The 3D printing (.stl) file can be obtained from the Waffle folder.

### Scripts

Ready-made scripts for running PRANCE and other methods are in PyHamilton_Methods. To run one of these, open a CMD shell, navigate to the folder
containing the desired script, and run with py. For example:
```bat
cd PRANCE\PyHamilton_Methods\210210_PRANCE_w_errorrecovery\reusable-pace
py robot_method.py
```
