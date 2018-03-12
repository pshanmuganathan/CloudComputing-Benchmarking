# CloudComputing-Benchmarking
Benchmarking of CPU,Memory and Disk
## BENCHMARKING
This project aims at Benchmarking the performance of CPU, Memory and Disk of KVM virtual machine m1.medium (2 virtual processors with 4GB RAM and 40GB disk), CentOS 7 Linux for the OS in a private Cloued testbed called Chameleon
## CPU
For CPU Benchmarking, we used strong scaling experiment and design a source code in C language.
* This program will measure the processor speed, in terms of double precision floating point operations per second (GFLOPS) and integer operations per second (GIOPS).
* This program has 16 instruction which include addition operation on both integer and floating point numbers which will run for 1 billion times to measure the speed.
* Main aim of this is to utilize the complete CPU cycle by performing diverse types of instructions and measure the speed.
* There is a performance evaluation which evaluates IOPS and FLOPS executed per second using different levels of concurrency (1 thread, 2 threads, 4 threads, 8 threads)
* Also ran this code with AVX instruction and adequate evaluation using bare metal provisioning.
* Ran the Linpack benchmark (http://en.wikipedia.org/wiki/LINPACK) and compare the performance achieved using double precision floating point.
## Memory
For Memory Benchmarking, we used strong scaling experiment and design a source code in C language.
* This program will measure the memory speed of host which will include parameters like read + write operations, sequential write access, random write access.
* This experiment used different block sizes (8B, 8KB, 8MB, 80MB), and varying the concurrency (1 thread, 2 threads, 4 threads, and 8 threads).
* We allocate 1 GB of memory to perform read + write operations in both sequential and random write access.
* The program also measures the throughput (Megabytes per second, MB/sec) and latency (microseconds, us). 8B block case used to measure latency, and the 8KB, 8MB, and 80MB cases used to measure throughput.
* Computed the theoretical memory bandwidth of your memory, based on the type of memory and the speed.
* Ran the Stream benchmark (http://www.cs.virginia.edu/stream/) and compared both the performance to see weather benchmarking is running properly.
## Disk
For Disk Benchmarking, we used strong scaling experiment and design a source code in C language.
* This program will measure the memory speed of host which will include parameters like read + write operations, sequential write access, random write access.
* This experiment used different block sizes (8B, 8KB, 8MB, 80MB), and varying the concurrency (1 thread, 2 threads, 4 threads, and 8 threads).
* It implements 4 methods, sequential read and write, random read and write.
* Allocated a large piece file of 1GB, and perform read + write or read operations on either sequential or random access within this 1GB file.
* Ran the IOZone benchmark (http://www.iozone.org/) and compared the performance achieved with theoretical performance.
