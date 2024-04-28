# Project: Parallel and Serial Implementations of K-Shortest Path Algorithm

## 1. Introduction
This experiment compares the performance of parallel and serial implementations of the k-shortest path algorithm, which identifies the top k-shortest paths between a source and destination in a graph. The parallel version employs MPI for distributed memory parallelism and OpenMP for shared memory parallelism.

## 2. Experimental Setup

### Hardware Specifications
- **Processor:** Intel Core i7-8700K CPU @ 3.70GHz
- **Memory:** 16 GB RAM
- **Cores:** 6 cores, 12 threads

### Software Configuration
- **Operating System:** Ubuntu 20.04 LTS
- **Compiler:** GCC version 9.3.0
- **MPI:** Open MPI version 4.0.3
- **OpenMP:** OpenMP version 5.0
- **Code Editor:** Visual Studio Code

### Dependencies
- C Libraries: `stdio.h`, `stdlib.h`, `limits.h`
- MPI Library: `mpi.h`
- OpenMP Library: `omp.h`
- Time Library: `time.h`

## 3. Compile and Run Instructions
**Parallel:**
- mpicc -fopenmp -o parallel parallel.c priorityqueue.c 
- mpirun -n 3 ./parallel

**Serial:**
- gcc -o program serial.c priorityqueue.c
- ./program

