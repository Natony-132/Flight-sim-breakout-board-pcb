# Flight simulator control integration PCB 

This project was to make a simple, expandable, Hardware to USB input control board. This is so that additional, non-standard controls or switch panels can be added to an existing flight simulator setup. 

This was accomplished by using an existing Arduino program called FreeJoy with a custom Interface board. The freeJoy program allows a series of Shift registers to expand the number of inputs that an arduino can normally except. 

![PCB layout](/flight%20sim%20board%20info/board.png) 
 

This custom PCB was designed with 40 inputs for switches and pads for up to 4 potentiometers.  

![other PCB layout](/flight%20sim%20board%20info/layout.png) 

Due to signal noise in most potentiometers, each pad was designed to have a 3rd order filter built in. 

![3rd order filter](/flight%20sim%20board%20info/filter.PNG) 

This proved to be unnecessary due to filters built into the Arduino program. This was not unexpected, so a filter bypass was built into the PCB so that the physical filter doesn't need to not be populated during board assembly. 

Later iterations will leave off this filter entirely.

 

These custom circuit boards were used in a UH-34 Sikorsky helicopter collective and a replica FA18 landing gear panel. 
![PCB in use](/Flight%20sim%20PCB%20in%20use%20images/flight%20sim%20lights%20on.jpg)
![PCB in use 2](/Flight%20sim%20PCB%20in%20use%20images/flight%20sim%20G.jpg)