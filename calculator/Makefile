objects = addition.o subtraction.o multiplication.o division.o main.o

calculator: main.o addition.o subtraction.o multiplication.o division.o operations.h
	cc -o calculator main.o addition.o subtraction.o multiplication.o division.o

main.o: main.c operations.h
	cc -c main.c -o main.o

addition.o: addition.c operations.h
	cc -c addition.c -o addition.o

subtraction.o: subtraction.c operations.h
	cc -c subtraction.c -o subtraction.o

multiplication.o: multiplication.c operations.h
	cc -c multiplication.c -o multiplication.o

division.o: division.c operations.h
	cc -c division.c -o division.o

clean:
	rm -f calculator $(objects)

.PHONY: clean
