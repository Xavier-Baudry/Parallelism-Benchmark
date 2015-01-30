# Parallelism-Benchmark
A simple benchmark test I've created for my Advanced Computer Architecture class.

The program simply calculates the product of two 1500x1500 matrix on a single thread, thereafter it splits the matrix
as evenly as possible and distributes it to threads where the produce will again be calculated.

The program will do the operations in interger arithmetic followed by a test using floating point arithmetic.

IMPORTANT NOTE: Due to the nature of the program, it may take up to 5 minutes to complete and will look like
it is idling, however it is not. Give it some time.

Also, due to some dependancies, the program will only run on Linux.


If you wish to compile it yourself:

g++  benchmark.cpp -o benchmark.out -pthread -std=c++11 -Wl,--no-as-needed
