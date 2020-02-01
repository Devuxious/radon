# String Encryption
*a.k.a. constant/string scrambling, string encoding, string hiding, constant (string) encryption*

## Overview
String encryption is the process of encrypting static strings present in the constant pool of a classfile and injecting
code to decrypt said strings on runtime. Almost every obfuscator sports this feature or at the very least, some kind of
derivation.

Against initial or inexperienced attackers, string encryption prevents potential attackers from making educated guess of
what a particular class or method does based purely upon strings. Often, strings for API endpoints and license server
IPs are encrypted or hidden for this purpose.

String encryption is very insecure because it relies on the fact that automatic obfuscators must inject code to decrypt
the encrypted string at runtime. This means the decryption method itself can be manipulated into decrypting the string
by an attacker. Obfuscators like Stringer attempt to make this difficult to by computing decryption keys based multiple
variables of the context at which the decrypter method is invoked.
