.PHONY: clean run

vpath %.java src
vpath %.class build


build/HelloWorld.class: HelloWorld.java | build
	javac -d build $^

build:
	mkdir -v build

run: HelloWorld.class
	cd build; java HelloWorld	

clean:
	rm -rvf build/*
