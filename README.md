# Activity-3---Operating-Overloading-Part-2

#### Set up a CPU class
##### Attributes
manufacturer - string<br />
processor type - string<br />
processor speed - float<br />
processsor cache - int<br />
cores - int<br />
rating - 1-10<br />

##### Operators
str - print some nice output.<br />
lt - Compare the cores first, if the number of cores of self is less than the number of cores of other then lt is true. If the number of cores are equal then the compare the processor speed and then the cache in the same way.<br />
eq - compare all of the attributes.<br />
gt - opposite of lt.<br />
in - check if the keyword is in any of the string attributes.<br />
int - return the rating<br />

#### Set up a hard drive class
##### Attributes
manufacturer - string<br />
hard drive size - int<br />
transfer rate - int<br />
cache - string, with units<br />
rating - 1-10<br />

##### Operators
str - print some nice output.<br />
lt - compare size,  then transfer rate, and finally latency.<br />
eq - compare all of the attributes.<br />
gt - opposite of lt.<br />
in - check if the keyword is in any of the string attributes.<br />
int - return the rating<br />

#### Set up a ram class
##### Attributes
manufacturer - string<br />
type - string, can be SDRAM, DDR, Rambus, or GDDR. GDDR is used for graphics cards<br />
size - string, with units<br />
rating - 1-10<br />

##### Operators
str - print some nice output.<br />
lt - compare size then type. GDDR > Rambus > DDR > SDRAM, although in theory GDDR should never be compared with other types.<br />
Each type is followed by a number, bigger is better, so GDDR5 > GDDR4.<br />
eq - compare all of the attributes.<br />
gt - opposite of lt.<br />
in - check if the keyword is in any of the string attributes.<br />
int - return the rating<br />

#### Set up a graphics card class
##### Attributes
card manufacturer - string<br />
graphics coprocessor - CPU class<br />
graphics ram - ram class<br />
rating - 1-10<br />

##### Operators
str - print some nice output.<br />
lt - compare ram and then compare processors.<br />
eq - compare all of the attributes.<br />
gt - opposite of lt.<br />
in - check if the keyword is in any of the string attributes for this class and the composed class.<br />
int - return the rating<br />

#### Set up a computer class
cpu - CPU class<br />
ram - ram class<br />
hard drive - hard drive class<br />
graphics card - graphics card class<br />
rating - 1-10<br />

str - print some nice output using the composed classes str operators<br />
int - return .4*cpu rating + .2*ram rating + .2*hard drive rating + .2*graphics card rating  <br />
lt - compare the int value for the computer<br />
eq - compare all of the attributes.<br />
gt - opposite of lt.<br />
in - check if the keyword is in any of the composed classes.<br />
 
#### More on __in__
If you have instatiated a computer, a use should be able to look for components of the computer using the in operator. So "Intel" in computer should list all of the computers that have intel as a manufacturer somewhere. Similarly "Rambus" in computer should list all of the computer that are using Rambus.


__init__ - all init methods are going to come through the command line, no inputs.

#### Instantiate
Processors: 
* Intel Core i5-6600K<br />
* Intel Core i3-6100<br />
* AMD-FX_8250<br />
* Intel Core 2 

Hard Drives: 
* Western Digital, 4TB, data transfer 6Gbps, cache 32MB<br />
* Seagate, 4TB, data transfer 4Gbps, cache 64MB<br />

Graphics Cards: 
* EVGA GeForce GTX 1050 Ti SC GAMING, 4GB GDDR5 with Intel core 2 processor - 3GHz with 8Gb ram<br />
* Gigabyte Radeon Rx 460 Windforce, 4GB GDDR4, with Intel core 2 processor - 4GHz with 16Gb ram<br />

Ram: 
* 32Gb of Rambus<br />
* 64Gb of DDR<br />

Two computers using these components.<br />

