CFLAGS = -c
CC = gcc
LIBS = -lm 

all: main

main: main.o parser.o scanner.o reader.o charcode.o token.o error.o
	$(CC) main.o parser.o scanner.o reader.o charcode.o token.o error.o -o main $(LIBS)

main.o: main.c
	$(CC) $(CFLAGS) main.c -o main.o

scanner.o: scanner.c
	$(CC) $(CFLAGS) scanner.c -o scanner.o

parser.o: parser.c
	$(CC) $(CFLAGS) parser.c -o parser.o

reader.o: reader.c
	$(CC) $(CFLAGS) reader.c -o reader.o

charcode.o: charcode.c
	$(CC) $(CFLAGS) charcode.c -o charcode.o

token.o: token.c
	$(CC) $(CFLAGS) token.c -o token.o

error.o: error.c
	$(CC) $(CFLAGS) error.c -o error.o


clean:
	rm -f *.o main *~
