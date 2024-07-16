CC=gcc
CFLAGS=-std=c99 -g

all: string atom 
clean:
	rm -f *.exe *.o *~ .*.un~

string: main.o String.o new.o
	$(CC) $^ -o $@ 

atom: main.o Atom.o new.o
	$(CC) $^ -o $@

new.o: new.h new.r 
String.o: String.h new.h new.r
Atom.o: atom.h new.h new.r
