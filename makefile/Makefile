CC = g++
CXXFLAGS = -Wall -O2
OBJECTS = bar.o foo.o main.o

bar.o : bar.cc bar.h
	$(CC) $(CXXFLAGS) -c $<
foo.o : foo.cc foo.h
	$(CC) $(CXXFLAGS) -c $<
main.o : main.cc bar.h foo.h
	$(CC) $(CXXFLAGS) -c $<
main: main.o foo.o bar.o
	$(CC) $(CXXFLAGS) $(OBJECTS) -o main

clean:
	rm -f ./*o main