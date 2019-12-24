.PHONY: clean run

vpath %.c src
vpath %.o build
vpath hello-world build


build/hello-world: hello-world.o | build
	cc -o build/hello-world $^

build/hello-world.o: hello-world.c | build
	cc -o build/hello-world.o -c $^

build:
	mkdir -v build

run: hello-world
	@$^

clean:
	rm -rvf build/*
