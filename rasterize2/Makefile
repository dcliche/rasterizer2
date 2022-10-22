CFLAGS= \
	-ffast-math \
	-O3 \
	-std=gnu11 \
	-mmmx -msse -msse2 -msse3 -msse4a -mssse3 -mfpmath=sse \
	-falign-functions \
	-finline-functions \
	-foptimize-sibling-calls \
	-funsafe-math-optimizations \
	-masm=intel -m3dnow -mtune=core2 \
	-g
	
OBJECTS=cityscape2.o \
	cityscape3.o \
	tower.o \
	livingroom.o \
	rasterize.o \
	fixedmath.o \
	enemy.o \
	core.o \
	ringworld.o \
	main.o
	
all: $(OBJECTS)
	gcc $(OBJECTS) -lm -lGL -lglut -lGLU -o raster
	
clean:
	rm -rf *.o
