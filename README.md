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
