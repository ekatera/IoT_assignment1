CC = gcc
bin = ../bin
include = ../include
lib = ../lib

$(bin)/program: main.c $(include)/mathhelpfunction.h $(lib)/mathhelpfunction.o | $(bin) $(lib)
	$(CC) -o $(bin)/program main.c $(lib)/mathhelpfunction.o -I$(include)

$(lib)/mathhelpfunction.o: mathhelpfunction.c | $(lib)
	$(CC) -o $(lib)/mathhelpfunction.o -c mathhelpfunction.c -I$(include)

clean:
	rm -f $(lib)/*.o
	rm -f $(bin)/program