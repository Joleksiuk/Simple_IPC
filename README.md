# Simple_IPC
Simple inter process communicatiom. The program synchronizes work of threads with linux mechanisms such as pipes, queues. shared memory and signals.

![so_projekt](https://user-images.githubusercontent.com/26255190/136761402-3d7571fe-2a0c-4746-8793-65846793a92f.jpg)

This scheme ilustrates the producer - consumer problem implemented with mechanisms:
  - pipes
  - shared memory
  - signals
  - FIFO files
  - 
There are 3 newly created processes:

  - Process 1: Reads signle lines from standard input file or user input, and transmits the data into process 2 
  - Process 2: Reads the data from process 1, counts the number of characters in every line, and transmits the results to process 3
  - Process 3: Reads the results from Process 2 and writes it out on the output stream. 
