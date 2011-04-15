A python package to calculate cosmological distances in a FRW metric.

Description
-----------

A package to calculate cosmological distances.  The workhorse is a class Cosmo
that wraps and the underlying C code.  The geometry can be non-flat.

In order to take advantage of the speed of the underlying C code, you should,
if at all possible, send numpy arrays to the methods rather than repeatedly
call the python methods.

Installation
------------

    python setup.py install --prefix=/some/path

If you want to use UPS to manage your code install with the with_ups command

    python setup.py with_ups install --prefix=/some/path


Unit Tests
----------
import cosmology
cosmology.test()

TODO
----
    - Add equation of state
    - Add *evolving* equation of state.
