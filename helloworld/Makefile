.PHONEY: all clean install

all: helloworld

clean:
	rm -f helloworld

install: helloworld
	install -D helloworld $(DESTDIR)/usr/local/bin/helloworld

helloworld: main.c
	$(CROSS)gcc $^ -o $@
