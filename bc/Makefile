.PHONY: clean run

vpath %.bc src
vpath % build

build/hello-world: hello-world.bc | build
	install $^ build/hello-world

build:
	mkdir -v build

run: hello-world
	@$^

clean:
	rm -rvf build/*
