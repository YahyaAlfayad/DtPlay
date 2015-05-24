Sometimes when compiling on Linux systems the following error occures:

<pre>
./DTAPI/DTAPI64.o: In function `Dtapi::XpThreadLinux::SetName(char const*)':
(.text+0x13df68): undefined reference to `dlsym'
collect2: error: ld returned 1 exit status
make: *** [DtPlay] Error 1
</pre>

In order to overcome that error, the <code>ldl</code> flag must be set in <code>Makefile</code>.
The code in this repository was tested on Ubuntu 14.04 - 64 bit. Please note that you have to follow the original instructions in <code>readme.txt</code> file.
