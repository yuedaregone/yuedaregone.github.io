LFLAGS+=-lpng
LFLAGS+=-lz

PNG_PATH= 
ZLIB_PATH = 

CORE_O= MImage.o export.o
EXECUTE= export

$(EXECUTE): export.o MImage.o
	g++ $(CORE_O) -o $(EXECUTE) $(LFLAGS)

clean:
	rm -f $(CORE_O) $(EXECUTE)

.cpp.o:
	$(CC) -c -o $@ $<

MImage.o: MImage.cpp MImage.h	
export.o: export.cpp MImage.h

