CC=g++
CFLAGS=-g -c -Wall -std=c++0x

kruskal_algo.o:  kruskal_algo.hpp graph.hpp disjoint_set.hpp kruskal_algo.cpp
	$(CC) $(CFLAGS) kruskal_algo.cpp

disjoint_set.o:  disjoint_set.hpp disjoint_set.cpp
	$(CC) $(CFLAGS) disjoint_set.cpp

graph.o: graph.hpp graph.cpp
	$(CC) $(CFLAGS) graph.cpp

main: main.o  kruskal_algo.o disjoint_set.o  graph.o 
	$(CC) kruskal_algo.o disjoint_set.o  graph.o  main.o -o main

main.o: kruskal_algo.hpp disjoint_set.hpp graph.hpp main.cpp
	$(CC) $(CFLAGS) main.cpp


clean:
	rm -rf *.o Main
