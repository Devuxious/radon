# Reference Obfuscation

## Overview
Reference obfuscation obscures method invocation and/or field gets/sets. This often done via reflection, MethodHandles,
proxies, and invokedynamic. Most obfuscators sport some kind of derivation of this (Zelix KlassMaster and Stringer in
particular).

Depending on how well said transformation is (and how much information an attacker has access to), reference obfuscation
is sometimes very tricky to deal with even for more experienced attackers. However, any type of reference obfuscation
often carries a considerable overhead as a side effect (performance and size) so it should be used sparingly.

Like string encryption, reference obfuscation is weak at its internal resolver subroutines as it must produce a
semantically equivalent behavior to the unobfuscation version of the program. Because of this, the obfuscator used
must inject the code to resolve the correct references which ultimately can be intercepted or manipulated. 
