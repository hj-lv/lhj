# lhj

---
### Paper
__ Zhuo Li, Shuaijun Liu, Jindian Liua, Yu Zhang, Teng Liang, Kaihua Liu__
SIM：Afastreal-time graph stream summarization with improved memory efficiency and accuracy
__Computer Networks 248 (2024) 110502__

---
### Files
- main.cpp,main,hpp: the implementation of SIM
- hash.c,hash.h: the hash function
- SIM_heavy.hpp: store heavy flow
- SIM_light.hpp: store little flow
- SIM.hpp：the overall framework of data structure
- p4/mv\_32.p4: p4 implementation of MV-Sketch for 32-bit flow key
- p4/mv\_104.p4: p4 implementation of MV-Sketch for 5-tuple flow key
---

### Compile and Run the examples
MV-Sketch is implemented with C++. We show how to compile the examples on
Ubuntu with g++ and make.

#### Requirements
- Ensure __g++__ and __make__ are installed.  Our experimental platform is
  equipped with Ubuntu 20.0.

- Prepare the test files.
    - You can use pcap,caida,dplp and so on to test its performance.
      

#### Compile
- Compile examples with make

```
    $ make main
```

    - The g++ compiler should be suitable 


#### Run
- Run the examples, and the program will output some statistics about the detection accuracy. 

```
$ ./main
```

