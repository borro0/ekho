all:
	make emulate

Vector.o: Vector.cpp Vector.h
	g++ -g -c Vector.cpp

emulate: Vector.o
	g++ emulate_render.cpp Vector.o -g -Wall -pedantic -L/usr/local/Cellar/gsl/1.16/lib -lGL -lGLU -lglut -lgsl -lgslcblas -lm  -o emulate_render

# -framework Foundation -framework glut -framework opengl 

clean:
	rm -rf emulate_render emulate_render.dSYM Vector.o

