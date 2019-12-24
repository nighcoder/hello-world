.PHONY: clean run

vpath %.py src
vpath % build

build/hello-world: hello-world.py | build
	install $^ build/hello-world

build:
	mkdir -v build

run: hello-world
	@$^

clean:
	rm -rvf build/*
