# ECE298-HomeSecurity
Software side of our Instruments and Prototyping Lab home security system prototype. Gave handy experience and practice with regards to embedded programming, PCB design, soldering, and using common electronics lab instrumentation to test and debug systems. 

Implemented with a Texas Instruments MSP430FR4133 MCU. Decided to use four reed switches to represent "different zones" in a "household".
Detection of anything magnetic closes the local circuit and sends an output signal accordingly to our audio transduscer (our alarm system). Statuses of each zone are displayed on the MCU LCD display - specific characters represent whether a zone is in danger, unarmed, or currently 'watching'/'monitoring'. Additionally, used LEDs on our custom manufactured PCB to represent zone status as well (different colour for a different state). One zone was set up to also detect sound - if the detected sound through the Analog-to-Digital converter was above a certain threshold, this would also trigger the alarm. 

Used tight-polling to continually monitor our zones, interrupts to interact with components such as our sound sensor / mic. 

# Top down view: 

![ece2981](https://user-images.githubusercontent.com/31193217/71362363-d1331f80-2563-11ea-84c0-d6da71ccfaca.png)


# Board Close-up (Arming timer, LCD displaying statuses with characters, different LEDs on): 

![ece2982](https://user-images.githubusercontent.com/31193217/71362367-d42e1000-2563-11ea-84b5-b2a32f69fd24.png)
![ece2983](https://user-images.githubusercontent.com/31193217/71362370-d6906a00-2563-11ea-8276-061610c0c8b0.png)


# Design Schematics and PCB Layout: 
Used Diptrace to create these design schematics. 

![ece2984](https://user-images.githubusercontent.com/31193217/71362375-d85a2d80-2563-11ea-82d3-6bf5613a2e17.png)
![ece2985](https://user-images.githubusercontent.com/31193217/71362376-da23f100-2563-11ea-82bd-581a2cbd9d3c.png)
