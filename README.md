#Flight simulator control integration PCB
This project was to make a simple, expandable, Hardware to USB input control board. This is so that additional, non-standard controls or switch panels can be added to an existing flight simulator setup.
This was accomplished by using an existing Arduino program called FreeJoy with a custom Interfase board. 

This custom PCB was designed with 40 inputs for switches and pads for up to 4 potentiometers. Due to signal noise in most potentiometers, each pad was designed to have a 3rd order filter built in.
This proved to be unnecessary due to filters built into the Arduino program. This was not unexpected, so a filter bypass was built into the PCB so that the physical filter doesn't need to not be populated during board assembly.
Later iterations will leave off this filter entirely. 
