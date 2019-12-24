.PHONY: clean run

vpath %.rs src
vpath %.o build
vpath hello-world build

build/hello-world: hello-world.rs | build
	rustc -o build/hello-world $^

build:
	mkdir -v build

run: hello-world
	@$^

clean:
	rm -rvf build/*
