
all: build

build:
	mkdir -p build && cp -r configure.ac Makefile.am src/ build/  && cd build/ \
	&& autoreconf --force --install \
	&& ./configure && make


clean:
	rm -rf build
