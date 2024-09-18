# Src of Knowledge
Author: PizzamanJ10

## Requirements
- A partner
- Python libraries: Scapy, OS
- A local network you can both be connected to

## The exercise

### Part 1
Write a python script, that listens for UDP packets on port `18613`.
If it recieves a packet from the source port `1337`, it should take the data from the packet, and run it as a CMD command.
(If you are not familiar with CMD, take 20 min online to read about it)

To run a cmd command, you can use the following code as an example:
```python
import os

command = 'shutdown /s'

os.system(command)
```

### Part 2
Now, add a feature to the python script, that will send the output of the command back to the IP that sent it the command, at port `9247`, in UDP.
If you listen now on the machine that's sending the commands, on port `9247`, you should be able to see the outputs of the commands you run!

Try making it nice, so that you can easily write commands and see the output from the computer thats sending them :)

Good luck!

