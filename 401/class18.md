# Cryptography

## Encryption, Decryption, and Hacking

### Encrypting a message

* One way of encrypting a message is called the Caeser cypher. It it done by shifting the order of the letters in the alphabet up or down by a set number of letters. To put a string of words into a cypher is to encrypt a message, while making it readable to human eyes is the act of decrypting a message

Cryptography is used in computers to keep information secure and to keep packages able to be sent with some amount of privacy on the internet. There is a tradeoff to all secure communication though, and that tradeoff is time. While it is possible to make every interaction online wildly secure, the process of encrypting and decrytping a message gets longer and shorter based on how complex those processes are.

### Key Exchange

Key exchange is a type of encryption and allows servers to send information through the internet to a website more securely than it would if it it would use no kind of encryption. Specifically, the Diffie-Hellman key exchange uses modular exponents form of encryption. It uses a combination of public and private values to encrypt.

Public values: Exponent base, modulus
Private values: exponents

By sending the public values between user and server, and then combining the exponents together on each respective machine, the resulting huge secret value would be only known to the two parties on either end of the transaction. This style of encryption where the key for decryption is the same at either end is known as symmetric encryption.

Asymmetric encryption is the method where there is a public key that allows anyone to encrypt a message, but the decrypting key is private.
