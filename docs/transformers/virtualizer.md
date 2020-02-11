# Virtualizer
*a.k.a. VM obfuscation*

## Overview
Virtualization is the process of converting a range of instructions into a custom instruction set which can
(theoretically) only be interpreted by a special virtual machine. Very few public Java bytecode obfuscators include this
feature (possibly including Stringer Enterprise).

Virtualization is often among the most difficult transformations to analyze and attack as a successful attack often
requires the attacker to understand the implementation of the custom VM and reconstruct a semantically equivalent set of
instructions from the custom instruction set.

Notably, virtualization is also one of the heaviest (performance and size) possible transformations possible as it
requires several extra computational cycles to interpret just one of the instructions from the custom instruction set.
