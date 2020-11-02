CC=gcc
CFLAGS=-g -Wall -pedantic
EXECS=lab3part1 lab3part2 lab3part3 lab3part4
OBJ=my_rand.o

all: $(EXECS)
debug: CFLAGS+=-DDEBUG=1
debug: all

lab3part1: lab3part1.c $(OBJ) timer.h
	$(CC) $(CFLAGS) -fopenmp  lab3part1.c  $(OBJ) -o lab3part1

lab3part2: lab3part2.c $(OBJ) timer.h
	$(CC) $(CFLAGS) -fopenmp  lab3part2.c  $(OBJ) -o lab3part2
	
lab3part3: lab3part3.c $(OBJ) timer.h
	$(CC) $(CFLAGS) -fopenmp  lab3part3.c  $(OBJ) -o lab3part3

lab3part4: lab3part4.c $(OBJ) timer.h
	$(CC) $(CFLAGS) -fopenmp  lab3part4.c  $(OBJ) -o lab3part4

lab3part5: lab3part5.c $(OBJ) timer.h
	$(CC) $(CFLAGS) -fopenmp  lab3part5.c  $(OBJ) -o lab3part5

my_rand.o: my_rand.c my_rand.h
	$(CC) $(CFLAGS) -c my_rand.c

clean:
	rm -rf $(EXECS) $(OBJ)