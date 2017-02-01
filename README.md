# Activity-3---Operating-Overloading-Part-3

#### Set up a CPU class
##### Attributes
manufacturer - string
processor type - string
processor speed - float
processsor cache - int
cores - int
rating - 1-10

##### Operators
str - print some nice output.
lt - compare the cores first, if the number of cores is equal then the compare the processor speed and then the cache.
eq - compare all of the attributes.
gt - opposite of lt.
in - check if the keyword is in any of the string attributes.
int - return the rating

#### Set up a hard drive class
##### Attributes
manufacturer - string
hard drive size - int
transfer rate - int
cache - string, with units
rating - 1-10

##### Operators
str - print some nice output.
lt - compare size,  then transfer rate, and finally latency.
eq - compare all of the attributes.
gt - opposite of lt.
in - check if the keyword is in any of the string attributes.
int - return the rating

#### Set up a ram class
##### Attributes
manufacturer - string
type - string, can be SDRAM, DDR, Rambus, or GDDR. GDDR is used for graphics cards
size - string, with units
rating - 1-10

##### Operators
str - print some nice output.
lt - compare size then type. GDDR > Rambus > DDR > SDRAM, although in theory GDDR should never be compared with other types. Each type is followed by a number, bigger is better, so GDDR5 > GDDR4.
eq - compare all of the attributes.
gt - opposite of lt.
in - check if the keyword is in any of the string attributes.
int - return the rating

#### Set up a graphics card class
##### Attributes
card manufacturer - string
graphics coprocessor - CPU class
graphics ram - ram class
rating - 1-10

##### Operators
str - print some nice output.
lt - compare ram and then compare processors.
eq - compare all of the attributes.
gt - opposite of lt.
in - check if the keyword is in any of the string attributes for this class and the composed class.
int - return the rating

#### Set up a computer class
cpu - CPU class
ram - ram class
hard drive - hard drive class
graphics card - graphics card class
rating - 1-10

str - print some nice output using the composed classes str operators
int - return .4*cpu rating + .2*ram rating + .2*hard drive rating + .2*graphics card rating  
lt - compare the int value for the computer
eq - compare all of the attributes.
gt - opposite of lt.
in - check if the keyword is in any of the composed classes.
 
#### More on in
If you have instatiated a computer, a use should be able to look for components of the computer using the in operator. So "Intel" in computer should list all of the computers that have intel as a manufacturer somewhere. Similarly "Rambus" in computer should list all of the computer that are using Rambus.

#### Instantiate
Processors: Intel Core i5-6600K, Intel Core i3-6100, and an AMD-FX_8250
Hard Drives: Western Digital, 4TB, data transfer 6Gbps, cache 32MB
             Seagate, 4TB, data transfer 4Gbps, cache 64MB
Graphics Cards: EVGA GeForce GTX 1050 Ti SC GAMING, 4GB GDDR5 with Intel core 2 processor - 3GHz with 8Gb ram
                Gigabyte Radeon Rx 460 Windforce, 4GB GDDR4, with Intel core 2 processor - 4GHz with 16Gb ram
Ram: 32Gb of Rambus
     64Gb of DDR

Two computers using these components.

