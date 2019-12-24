.PHONY: clean run

vpath %.js src
vpath % build

build/hello-world: hello-world.js | build
	install $^ build/hello-world

build:
	mkdir -v build

run: hello-world
	@$^

clean:
	rm -rvf build/*
