# Python SHA-1

An implementation of the SHA-1 hashing algorithm in pure python. 

This library was designed to demonstrate a straight-forward implementation of
the algortihm, and is not designed for speed. The current implementation
matches the [hashlib](https://docs.python.org/3/library/hashlib.html) api. 
If you want to see the entire algorithm run in a single function, see 
[this commit](https://github.com/ajalt/python-sha1/blob/4f9306d271e39e354c695ca6fb66d3f598dab64b/sha1.py).

## Usage

The library may be called from the command line.
Message input may be piped in stdin:

    $ echo hello | python sha1.py
    sha1-digest: f572d396fae9206628714fb2ce00f72e94f2258f

A file may also be specified as arguments to the script:

    $ python sha1.py myfile
    sha1-digest: 3f786850e387550fdab836ed7e6dc881de23001b

A file may also be specified as many arguments to the script:
	
    $ python sha1.py file example main
    sha1-digest: 9f41a95cba557b2894771eed96e07a4ded82537f
    sha1-digest: 57a9901af6fe030198ef1737783e2048ee96da4a
    sha1-digest: 743803de635cbcc9001a61ab8498261b1acb3e83



