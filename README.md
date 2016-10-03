# baser

Convert numbers from a javascript base10 number to other bases.  Can either run 
in "pure" mode (which runs into issues with mantissa and divisibility) or 
"accurate" mode which is certain to always keep the digits the same when going 
back to original base but does not give you the right numbers to use in 
mathematical operations.

Why the two modes?  Often we are using this library to compress quite long 
numbers where we don't want to lose precision after the decimal.  Accurate is
much more useful, as we don't have to worry about loss of data when converting
back to base 10.

Currently this only works in "accurate" mode for research sake.