libnndc.a: nndclib.f
	gfortran.exe -c nndclib.f
	ar.exe cr libnndc.a nndclib.o

pandora.exe: libnndc.a pandora.f
	gfortran.exe -static pandora.f  -L. -lnndc -o pandora.exe

clean:
	del *.o
	del *.o
	del pandora.exe
