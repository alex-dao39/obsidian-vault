***
### Purposes
Take in an [[Technical Terms#^arbitratry|arbitrary]] value (typically of any length) and return a fixed-length arbitrary value.
***
### Properties of a good hash function
- Fixed size output, not dependent on the input
- [[Radical Asymmetry]]
- [[Technical Terms#^collision-resistance|Collision Resistance]]
- [[Technical Terms#^ba84fb|Uniformity across degrees and range]].
	- E.g, the out put of SHA-256 is uniformly distributed across the whole 256 bits and is not dependent on the size, length or complexity of the input.
- [[Technical Terms#^determinism|Determinism]]
***
### Use cases
- passwords: storing the hash of actual password with a [[Keys, Nonces and Salts|salt]].
- [[Digital Signature]].
- [[IFPS|Digital Storage]].
- Pseudo-random number generator.
- Hash commitments