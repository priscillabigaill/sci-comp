CC = gcc

all: main.out

main.out: myutils.o 2602109883.o main.o
	${CC} -o main.out main.o myutils.o 2602109883.o -lm

2602109883.o: 2602109883/2602109883.c
	${CC} -Wall -c 2602109883/2602109883.c -o 2602109883.o -I.

main.o: main.c
	${CC} -Wall -c main.c -o main.o

myutils.o: utils/myutils.c
	${CC} -Wall -c utils/myutils.c -o myutils.o 

clean:
	rm *.o 
	rm *.out