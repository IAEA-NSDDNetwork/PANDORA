libnndc.a: nndclib.f
	gfortran -c nndclib.f
	ar cr libnndc.a nndclib.o

pandora: libnndc.a pandora.f
	gfortran -o pandora -L. -lnndc pandora.f

clean:
	rm -f *.o
	rm -f *.a
	rm -f pandora
	
