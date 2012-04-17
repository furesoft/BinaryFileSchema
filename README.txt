Binary File Schema
==================

http://www.andersriggelsen.dk/binaryfileschema.php

Binary File Schemas is a project of mine that will allow you to define the structure of various binary files.
There are quite a lot of uses for this:

* Easy to explain the structure of binary files to other people
* Create programs that can inspect any binary file given a schema
* Automatically generate a parser directly from a schema
* Extend application functionality (eg. allow Google Desktop Search to search virtually any file if you have schemas for them)
* Make compression/diff programs content-aware to maximize speed and accuracy.
* Binary File Schemas' syntax include basic validation and computation functionality.

Features so far
---------------
* Structures - ordered list of data
* Offset structures - data stored at other places at either relative or absolute offsets to the read value
* Enums - limited set of possible values
* Bitfields - fields containing a bunch of flags
* Arrays - of both constant, calculated and unknown lengths (with multiple stop clauses)
* Compression - Automatically handles compressed structures of data (C# generator supports GZip and Deflate)

The aim is not to be able to express all kinds of binary files but at least attempt to express most types of formats in a simple syntax.