.PHONY: clean run

vpath %.sh src
vpath % build

build/hello-world: hello-world.sh | build
	install $^ build/hello-world

build:
	mkdir -v build

run: hello-world
	@$^

clean:
	rm -rvf build/*
