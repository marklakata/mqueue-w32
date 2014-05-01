mqueue-w32
==========

Win32s port of POSIX mqueues


History:

This code was originally written by Aurelio Medina in 2000. The original code can be found here

http://cygwin.com/ml/pthreads-win32/2000/msg00131.html

This version has the following improvements

* compiles without warning on VisualStudio 2012
* works around the pthreads issue of global Mutexes by using native Windows Mutexes and Events,
  instead of pthreads mutexes and signals.
* added support for `mq_timedreceive()`


Caveat: The demo code is multithreaded, so it does not demonstrate how to use this between different
processes.

Mark Lakata



