CC=g++
LIBS=-lIrrlicht
CFLAGS=$(LIBS)
DEPS =
OBJ = main.o

%.o: %.c $(DEPS)
	$(CC) -c -o $@ $< $(CFLAGS)

game: $(OBJ)
	$(CC) -o $@ $^ $(CFLAGS)

all: game

.PHONY: clean

run: game
	./game

clean:
	rm -f *.o game
