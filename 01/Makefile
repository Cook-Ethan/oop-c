CC=gcc
CFLAGS=-std=c99 -g

all: set bag
clean:
	rm -f *.exe *.o

set: main.o Set.o
	$(CC) $^ -o $@ 
bag: main.o Bag.o
	$(CC) $^ -o $@ 

Set.o: new.h Set.h Object.h
Bag.o: new.h Set.h Object.h
