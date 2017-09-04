CC = gcc
INC_DIR = .
LIB_DIR = .
CFLAGS  = -c -Wall -I$(INC_DIR)
#LFLAGS  = -L$(LIB_DIR) -lFunction

hello: hello.o printmovie.o
	$(CC) $^ -o $@
hello.o: hello.c $(INC_DIR)/printmovie.h
	$(CC) $(CFLAGS) hello.c 
printmovie.o: printmovie.c
	$(CC) $(CFLAGS) $^
clean:
	rm -f *.o hello
