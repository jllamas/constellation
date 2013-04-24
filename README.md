Constellation
=============

Find the constellation name given RA and DEC.

This is a port of http://djm.cc/constellation.js into ruby.

http://djm.cc/constellation.html is a Javascript port of a C program found here http://cdsarc.u-strasbg.fr/viz-bin/Cat?VI/42

The 'new' method can take a simple string like the original or an array.

String Examples
-------------
Find with a simple string

20 34 55.56 -10 33 22.1
7 18.389 +41 32.17
13.2324 +33.91

```ruby
Constellation.new("6 43 49.5 -1 3 46.9")
 => #<Constellation:0x00000102744b60 @ra=6.730416666666667, @dec=-1.063027777777778, @abreviation="Mon", @name="Monoceros", @genitive="Monocerotis">
```

Array Examples
-------------
RA - in decimal hours
DEC - in decimal degrees

```ruby
Constellation.new([6.730408333333334, -1.063033])
  => #<Constellation:0x00000104536a88 @ra=6.730408333333334, @dec=-1.063033, @abreviation="Mon", @name="Monoceros", @genitive="Monocerotis">
```
