# Cyclic-Redudancy-Checker
This is a communication system designed with LEDs for communication and CRC to detect errors. 

There are two files in this project. 
1. crc.cpp :
    This is the sender side code by which calculates the CRC bits after polynomial division. 
    Inputs: > Length of the bit string need to be sent.
            > Bit string
            > Length of the generator
            > Generator

    Outputs: > Number of 0's to be appended.
             > Message after appending 0's.
             > CRC bits.
             > Transmitted Frame.
         
2. crc.oy :
This is the receiver side code which determines whether the bit string received is correct or not with help of predecided generator.
This does not asks for any input. The bit string and the generator can be edited in code which are there at the end of the code. It outputs the remainder after the polynomial division. If the remainder id equal to 0, then the message is correct and accepetable. If it is not equal to 0, the message is wrong and needs retransmission.

