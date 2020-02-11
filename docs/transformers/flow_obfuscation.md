# Flow Obfuscation
*a.k.a. control-flow obfuscation*

## Overview
Flow obfuscation involves restructuring a function's code so that it's control flow is difficult to understand. Nearly
all Java bytecode obfuscators sport some kind of flow obfuscation feature.

When done well, flow obfuscation can be one of the more annoying transformation strategies to deal with as it hinders a
lot of effective decompiler usage. Depending on how the obfuscator implements the flow obfuscation, flow obfuscation can
sometimes lead to some negative performance and/or file sizes.
