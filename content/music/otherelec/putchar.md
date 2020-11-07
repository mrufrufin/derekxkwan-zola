+++
title = "putchar"
date = 2015-01-01
description = "c code to aplay"

[extra]
author = "Derek Kwan"
keywords = "putchar, noisy, c, aplay"
+++

Applying a technique I learned from countercomplex's [blog post](http://countercomplex.blogspot.com/2011/10/algorithmic-symphonies-from-one-line-of.html), this series of algorithmic compositions pipes the output of compiled C code to the soundcard via the aplay command. The actual C code consists of the declaration of the main function passed a variable automatically typecasted to an integer. In the body, you iterate over the variable in a for loop and use putchar to write a statement involving the variable to stdout. The code looks something like this: `main(t){ for(t=0;;t++){putchar(t * ((t>>10)&54));};}`
