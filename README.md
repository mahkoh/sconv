sconv
=====

Simple frontend for convert

`sconv` is a small script to concatenate images with `convert`.

Usage
-----

    $ ls
    a.png b.png c.png d.png
    $ sconv ++/++ * out.png
    $ ls
    a.png b.png c.png d.png out.png
    
`out.png` now contains the concatenation of the four images in a 2x2 matrix.
`a` and `b` are in the top row, `c` and `d` in the bottom row.

    $ rm out.png
    $ sconv +++/+ * out.png
    
Now `a`, `b`, and `c` are in the top row and `d` in the bottom row.
