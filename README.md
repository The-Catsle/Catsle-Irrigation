# Catsle Irrigation

A small creek runs through our back yard. A previous owner routed most of it through a buried pipe,
but left a small section of it accessible. In 2025 we leased water rights and wanted to use it for
watering our gardens. 

This project aims to let us pump the water into a couple barrels and then pump it out of the barrels
to our various gardens.

# The Result
## Overall Setup
I built a 24V relay-controlled system that runs from two 100W solar panels and two 12V deep-cycle
batteries in series. They fill two 55-gallon barrrels and we have a series of LEDs to tell us the
status of the system. 

In this photo you can see the solar panels, batteries, control box, and the tiny bit of creek
in the corner of the yard. 
![C667240E-9A41-42D4-8993-4457A6BCD76D_1_105_c](https://github.com/user-attachments/assets/2bec9ec9-c687-486e-a7d6-9767e18d9e6a)

## The Control Box
This photo is already slightly outdated but it gives you the gist of the layout. The only major
changes I've made since this photo have been to delete the left relay and clean up some of the
wiring. 

![E9624C94-3CB4-488F-B1D6-7A105D0BB151_1_105_c](https://github.com/user-attachments/assets/497fcb5f-9071-40cc-b3fc-92c2d330d6de)

The percentage lights are controlled by a series of float switches in one of the barrels and
tell us how much water we have.

![1F83D141-623B-432B-AB2E-2534BE3C1CF8_1_105_c](https://github.com/user-attachments/assets/ab1831cb-a418-4094-b2aa-79fcff070df4)

Additionally some switches will enable or disable the two pumps. The 100% full switch (when
high) will disable the pump that fills the system. The 25% full switch (when low) will disable
the drain pump. And we also have a float switch in the creek that will disable the fill pump
if the creek goes dry.

# The Schematic
I used KiCAD to create the schematic. The image should be all you need to understand it, but I have
added links to all the datasheets for every part if you're curious. 

![image](https://github.com/user-attachments/assets/6ba22fbe-a74a-45fe-b941-3be392edae55)
> May 17 Export

# Problems
So this project is a version 1 of the overall concept but we wanted to start somewhre. 
* The well/creek pump isn't very deep in the water and can run dry during some normal
flow states
* The hose connecting the barrels is too small which results in (slightly) inaccurate
fill readings
