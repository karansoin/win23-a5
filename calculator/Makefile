CC = gcc
CFLAGS = -Wall -Wextra -pedantic -std=c99 -Wno-unused-parameter
SRC = main.c addition.c subtraction.c multiplication.c division.c
OBJ = $(SRC:.c=.o)

calculator: $(OBJ)
	$(CC) $(CFLAGS) -o calculator $(OBJ)

%.o: %.c operations.h
	$(CC) $(CFLAGS) -c $< -o $@

.PHONY: clean
clean:
	rm -f calculator $(OBJ)


