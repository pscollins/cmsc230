CFLAGS=-ggdb -pthread -Wall -O3 -std=c11
CC=gcc 
CHK_SOURCES = *.c
DEPS = graph.c tsgraph.c ../../utilities/stopwatch.c

check-syntax:
	$(CC) $(CFLAGS) -S $(CHK_SOURCES)

%: 
	$(CC) $(CFLAGS) -o $@.out $@.c $(DEPS)

# test: *.c *.h
# 	gcc tests

.PHONY: clean

clean:
	rm *.out
