# Radon Java Obfuscator [![Build Status](https://travis-ci.org/ItzSomebody/Radon.svg?branch=master)](https://travis-ci.org/ItzSomebody/Radon)

Radon is a Java bytecode obfuscator that I conceptualized in my freshman year of high school. I use Radon to experiment
with obfuscation and to learn about various parts of Java bytecode.

It's important to note that Radon is intended for __***experimentation only***__. If your software breaks in production
because you protected it with Radon, then just know you have been warned.

If you have a quick question about how something works, you can just join my [Discord](https://discord.gg/RfuxTea)
server and ask.

If you would like some pointers to production-safe (more or less) and less buggy Java bytecode obfuscators, I would
suggest one of these:
* [Zelix KlassMaster](http://www.zelix.com/)
* [Paramorphism](https://paramorphism.serenity.enterprises/) - [Discord](https://discordapp.com/invite/k9DPvEy)
* [Proguard](https://www.guardsquare.com/en/products/proguard)

Additionally, here are some other obfuscators for Java that you could check out
for fun:
* [Allatori](http://www.allatori.com/)
* [DashO](https://www.preemptive.com/products/dasho/overview)
* [JBCO](http://www.sable.mcgill.ca/JBCO/)
* [JObf](https://github.com/superblaubeere27/obfuscator)
* [NeonObf](https://github.com/MoofMonkey/NeonObf)
* [Obzcure](https://obzcu.re/) - [Discord](https://discordapp.com/invite/fUCPxq8)
* [Sandmark](http://sandmark.cs.arizona.edu)
* [Stringer](https://jfxstore.com/stringer/)
* [yGuard](https://www.yworks.com/products/yguard)

## FAQ

* **Q: Is this uncrackable/undeobfuscatable?**  
*A: No. Nothing is impossible to deobfuscate or reverse-engineer. Furthermore, Radon is far from being hard to
deobfuscate. On a scale of 1 to 10 on how hard Radon is to deobfuscate, I'd say 3 in the best possible scenario.*
* **Q: Why is this open-sourced?**  
*A: I made Radon as a way to experiment with obfuscation and to become familiar with the JVM bytecode instruction set
and as a codebase if anyone wants to mess around. Furthermore, I strongly support the FOSS ideology.*
* **Q: Doesn't Radon being open-sourced make it easier to deobfuscate?**  
*A: Probably.*
* **Q: Can Spring apps be obfuscated with this?**  
*A: Out of the box, no. Starting from Radon 3, I will never add support for Spring or multiversion JARs.*
* **Q: What does '... "org/somelib/TableFactoryBuilder" not found in classpath' mean?**  
*A: Radon internally determines how to construct certain entities in the classfile based on the class hierarchy of the
JAR being obfuscated. For this reason, Radon needs access to library classes used by the project. Make sure you add
the appropriate libraries so this doesn't show up.*
* **Q: Can I use all transformers for maximum protection?**  
*A: You could, but you should note that it's very likely that the program will break and/or there will be a large
overhead in file size or performance.*
* **Q: Why do certain combinations of transformers break the program?**  
*A: Radon is intended to be an experimental project, not a commercial product protector. Not all features are meant to
work together.*
* **Q: What version of Java is required to run Radon 3?**  
*A: Java 11 and above.*
* **Q: What version of Java is my software required to written in to work with Radon?**  
*A: Radon can theoretically obfuscate software written in any Java version.*
* **Q: Does Radon support Android?**  
*A: While the answer is yes, I will not provide support for issues pertaining to Android apps.*

## License

GNU General Public License v3.0
