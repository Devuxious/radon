# Radon Java Obfuscator [![Build Status](https://travis-ci.org/ItzSomebody/Radon.svg?branch=master)](https://travis-ci.org/ItzSomebody/Radon)

Welcome to the documentation page for the Radon Java bytecode obfuscator! Here you can find the documentation and
various parts of research put into Radon's internals and transformers.

* [Exclusions](exclusions.md)
* Transformers
    * String encrypters
        * XOR encrypter
        * Base64 encrypter
        * Dynamic encrypter
        * Long Array encoder
        * String pooler
        * Complex encrypter
        * Anti-emulation encrypter
    * Flow obfuscators
        * Block splitter
        * CFG flattener
        * Dead branch injector
        * Dead switch injector
        * Dead trap injector
        * Null check mutilator  
        * Stack rearranger
    * Number obfuscators
        * Arithmetic obfuscator
        * Bitwise obfuscator
        * Casting obfuscator
        * Context obfuscator
        * Number pooler
    * Reference obfuscator
        * Invocation proxy obfuscator
        * Invokedynamic obfuscator
        * Reflection obfuscator
    * Watermarker
        * Todo
    * Virtualizer
        * Simple VM
        * TODO
    * Misc.
        * Anti-debugger injector
        * Anti-memory-dump injector
        * Anti-tamper injector
        * Name obfuscator
        * Expiration injector
        * Member shuffler
        * Packer
        * Shrinker
