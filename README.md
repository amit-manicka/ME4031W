# ME4031W
This Repo holds the LABVIEW VI file used by Amit Manicka, Calieb Prunty, and Huxley Nyabwari for experimentation in Summer 2023 of ME 4031W, Basic Measurements at the University of Minnesota Twin Cities

## How to use
The file assumes you have NI LABVIEW Packages installed in the Spring 2021 Version:
Link: https://www.ni.com/en/support/downloads/software-products/download.labview.html#487445
Additionally, You'll want an NI DAQ model USB-6002 (https://www.ni.com/docs/en-US/bundle/usb-6002-specs/resource/374371a.pdf). 

## Circuitry required.
Have the Solar Panel (https://www.amazon.com/SUNYIMA-Polycrystalline-Panels-50x50MM-1-96inch/dp/B087TK7T7T) in parallel with a 1 k-Ohm resistor.
Ensure the solar panel and the resistor are grounded, with ground being the AI0- port on the DAQ and the positive lead being the AI0+ port on the DAQ. 
There is also a GND port on the DAQ. Plug that into the ground. After setting up, plug into computer via USB.

## In the application
The app will prompt you for your resistor value, and a DAQ number. If set up correctly, you should be able to select your DAQ from the dropdown menu.
There also is a file path as the software will write the data to a csv file. Specify any path you desire. Once you enter a resistor value in, hit the run button.
The DAQ will collect voltage and power data for 30 seconds and output it to the CSV file specified. Additionally, it will show you a graph of what it read.
