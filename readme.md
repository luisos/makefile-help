# Makefile brief help

## Format
	target: dependencies
	        commands

### Autovars
	$@ - target
	$^ - dependencies
	$< - first dependency

### Templates
	%.o: %.c
	        $(CC) $^ -o $@
		
	.c.o:
	        $(CC) $^ -o $@
	
	.PHONY: all clean install uninstall

### Links
* [Russian manual](http://rus-linux.net/nlib.php?name=/MyLDP/algol/gnu_make/gnu_make_3-79_russian_manual.html)
* [English manual](https://www.gnu.org/software/make/manual/make.html)
