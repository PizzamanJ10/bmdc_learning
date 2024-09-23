# Src of Knowledge
Author: PizzamanJ10

## Requirements
- A partner (or a second computer)
- Python libraries: Scapy, OS
- A local network you can both be connected to

## The exercise
In this exercise, there are 2 computers. 
We'll refer to one as the commander, and one as the victim.

### Part 1
Write a python script, that will run on the `victim computer`, that listens for UDP packets on port `18613`.
If it recieves a packet with the source port `1337`, it should take the data from the packet, and run it as a CMD command.
(If you are not familiar with CMD, take 20 min online to read about it)

To run a cmd command, you can use the following code as an example:
```python
import os

command = 'shutdown /s'

os.system(command)
```

### Part 2
Now, add a feature to the python script on the `victim_computer`, that will send the output of the command back to the IP that sent it the command, the `commander computer`, at port `9247`, in UDP.
Now add a feature to the `commander_computer`, that listens on port `9247`, and prints the output of the commands that are coming back from the `victim_computer`~

Try making it nice, so that you can easily write commands on the `attacker_computer` and see the output that the `victim_computer` is sending back.

Good luck!

