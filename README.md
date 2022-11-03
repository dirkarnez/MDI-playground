MDI-playground
==============

### Makefile
```
# Project: Project3
# Makefile created by Embarcadero Dev-C++ 6.3

CPP      = g++.exe
CC       = gcc.exe
WINDRES  = windres.exe
RES      = Project3_private.res
OBJ      = main.o $(RES)
LINKOBJ  = main.o $(RES)
LIBS     = -L"C:/Users/Administrator/Downloads/Embarcadero_Dev-Cpp_6.3_TDM-GCC_9.2_Portable/TDM-GCC-64/lib" -L"C:/Users/Administrator/Downloads/Embarcadero_Dev-Cpp_6.3_TDM-GCC_9.2_Portable/TDM-GCC-64/x86_64-w64-mingw32/lib" -static-libgcc -mwindows
INCS     = -I"C:/Users/Administrator/Downloads/Embarcadero_Dev-Cpp_6.3_TDM-GCC_9.2_Portable/TDM-GCC-64/include" -I"C:/Users/Administrator/Downloads/Embarcadero_Dev-Cpp_6.3_TDM-GCC_9.2_Portable/TDM-GCC-64/x86_64-w64-mingw32/include" -I"C:/Users/Administrator/Downloads/Embarcadero_Dev-Cpp_6.3_TDM-GCC_9.2_Portable/TDM-GCC-64/lib/gcc/x86_64-w64-mingw32/9.2.0/include"
CXXINCS  = -I"C:/Users/Administrator/Downloads/Embarcadero_Dev-Cpp_6.3_TDM-GCC_9.2_Portable/TDM-GCC-64/include" -I"C:/Users/Administrator/Downloads/Embarcadero_Dev-Cpp_6.3_TDM-GCC_9.2_Portable/TDM-GCC-64/x86_64-w64-mingw32/include" -I"C:/Users/Administrator/Downloads/Embarcadero_Dev-Cpp_6.3_TDM-GCC_9.2_Portable/TDM-GCC-64/lib/gcc/x86_64-w64-mingw32/9.2.0/include" -I"C:/Users/Administrator/Downloads/Embarcadero_Dev-Cpp_6.3_TDM-GCC_9.2_Portable/TDM-GCC-64/lib/gcc/x86_64-w64-mingw32/9.2.0/include/c++"
BIN      = Project3.exe
CXXFLAGS = $(CXXINCS) 
CFLAGS   = $(INCS) 
DEL      = C:\Users\Administrator\Downloads\Embarcadero_Dev-Cpp_6.3_TDM-GCC_9.2_Portable\devcpp.exe INTERNAL_DEL

.PHONY: all all-before all-after clean clean-custom

all: all-before $(BIN) all-after

clean: clean-custom
	${DEL} $(OBJ) $(BIN)

$(BIN): $(OBJ)
	$(CPP) $(LINKOBJ) -o $(BIN) $(LIBS)

main.o: main.cpp
	$(CPP) -c main.cpp -o main.o $(CXXFLAGS)

Project3_private.res: Project3_private.rc resource.rc
	$(WINDRES) -i Project3_private.rc --input-format=rc -o Project3_private.res -O coff 

```
