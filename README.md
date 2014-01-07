# varifuzz

Use [zzuf][] to corrupt an increasing percentage of a file's bits.

    Usage: ./varifuzz inputfile outputdir/ ERRPCT_MIN ERRPCT_INCREMENT ERRPCT_MAX
      where 0.0 <= ERRPCT_MIN < ERRPCT_MAX <= 100.0
        and 0.0 < ERRPCT_INCREMENT < 100.0

E.g., to generate 51 versions of a file with 0% to 5% of the bits flipped,

    ./varifuzz examples/baboon640.jpg baboon 0.0 0.1 5.0

[zzuf]: http://caca.zoy.org/wiki/zzuf
