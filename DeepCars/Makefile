#CC=clang++
CC=g++

all:
	$(CC) main.cpp -I../pig -I/usr/include/SDL2 -I. \
	-lSDL2 -lSDL2_ttf -lSDL2_image -lpthread -lwebp  \
	-I/usr/include/gsl -lgsl -lgslcblas -lm \
	-o main

png-fix:
	find imagens -type f -iname '*.png' -exec pngcrush -ow -rem allb -reduce {} \; 

run:
	./main

dep:
	sudo apt install libgsl-dev

clean:
	rm -f main
