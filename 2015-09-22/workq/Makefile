.PHONY: test

test: workq
	./workq 4

workq: workq.o 
	$(CC) -o $@ $^ -lpthread -lm

%.o: %.c
	$(CC) -std=c99 -c -O3 $<

clean:
	rm -f *.o workq
