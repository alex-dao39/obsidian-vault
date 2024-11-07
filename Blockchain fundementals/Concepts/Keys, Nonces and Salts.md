***
### Cryptographic Keys
- is an [[Technical Terms#^arbitrary|arbitrary secret]].
- If the key is compromised, the cryptographic does nothing.
- A good cryptographic key should:
	- be generated with an unbiased random number generator or trustworthy hardware.
	- large enough that it can not be guessed in a reasonable time frame.
	- stored securely
***
### Public values
- Everything else is considered public.
- Any user-generated content is public.
- [[Technical Terms#^cryptographic-primitive|Crypto primitives]] are designed to ensure that even if user-generated content is known, they still provide the same security guarantee.
***
### Salts
- **Definition**: Unpredictable values that are not treated as secrets.
- **Purpose**: "flavoring" a hash function, or to anchor cryptographic primitives to a particular use case.
- **Examples**: password

***
### Nonces
- [[Technical Terms#^nonce|Definition]]
- **Example**: simple counter.