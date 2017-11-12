CC = emcc
RUN = emrun
RUNFLAGS = --no_browser --port
RUNPORT = 8080
CFILES = print.c hello.c
OUTFILES = hello.wasm hello.js
TARGET = hello.html

build:
	$(CC) $(CFILES) -s WASM=1 -o $(TARGET)

clean:
	rm -f $(OUTFILES) $(TARGET) *~

run: 
	$(RUN) $(RUNFLAGS) $(RUNPORT) .