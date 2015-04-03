CXX=clang++
CXXFLAGS := -std=c++11 -O3 -DNDEBUG -I/usr/local/include/eigen3
VPATH = ../src

all: libcns.a
libcns.a : Meta.o ISolver.o GradientDescentSolver.o ConjugateGradientSolver.o NewtonDescentSolver.o BfgsSolver.o LbfgsSolver.o LbfgsbSolver.o
	ar rc libcns.a *.o
	ranlib libcns.a
clean:
	rm libcns.a *.o
