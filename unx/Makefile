libnndc.a: nndclib.f
	gfortran -c nndclib.f
	ar cr libnndc.a nndclib.o

pandora: libnndc.a pandora.f
	gfortran -static pandora.f  -L. -lnndc -o pandora

clean:
	rm -f *.o
	rm -f *.a
	rm -f pandora
