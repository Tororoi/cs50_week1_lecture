# Makefile

# Compiler
CC = gcc

# Compiler flags
CFLAGS = -Wall -Wextra

# Linker flags
LDFLAGS = -lcs50

# Default target
all: $(patsubst %.c,%,$(wildcard *.c))

# Rule to build each program
%: %.c
	$(CC) $(CFLAGS) -o $@ $< $(LDFLAGS)

# Clean target
.PHONY: clean
clean:
	rm -f $(patsubst %.c,%,$(wildcard *.c)) *.o
