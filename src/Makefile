## Makefile

TARGET		= galasm.js
SOURCES		= galasm.c support.c jedec.c localize.c
OUTPUTS     = galasm.js galasm.wasm
CC          = emcc

CFLAGS		= -Wall -O3
LDFLAGS		= -s EXPORTED_RUNTIME_METHODS='["callMain"]'


all: $(TARGET)

$(TARGET):
	$(CC) $(CFLAGS) $(SOURCES) $(LDFLAGS) -o $@ $(OBJS)

clean:
	-rm -f $(OUTPUTS)
 
