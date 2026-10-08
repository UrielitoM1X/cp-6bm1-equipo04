CC = gcc

all: matmul_00 matmul_02 matmul_03 hello_omp

matmul_00: matmul.c
	$(CC) -O0 -std=c11 $< -o $@

matmul_02: matmul.c
	$(CC) -O2 -std=c11 $< -o $@

matmul_03: matmul.c
	$(CC) -O3 -march=native -std=c11 $< -o $@

hello_omp: hello_omp.c
	$(CC) -fopenmp $< -o $@

clean:
	rm -f matmul_00 matmul_02 matmul_03 hello_omp
