# Compiler
CC = cc
CFLAGS = -Wall
TARGET = main

INCLUDE =
LIBRARIES =

SRC = main.c
OBJ = $(SRC:.c=.o)

all: $(TARGET)

$(TARGET): $(SRC)
	$(CC) $< $(INCLUDE) $(LIBRARIES) $(shell pkg-config --libs --cflags raylib) -o $@

.PHONY: clean
clean:
	rm -f $(OBJ) $(TARGET)
