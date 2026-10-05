## Public Key Encryption

Public Key Encryption is the asymmetric encryption key that makes much of the digital world work in today's age. Given a trusted set of public keys, any two entities can communicate without a previously shared private key. In the world of the Internet, public key encryption is necessary for a side to prove who they are using the private key that matches their public key.

Let's go into more specifics about how it works. 

## Diffie-Hellman key exchange algorithm

The Diffie-Hellman key exchange algorithm is a key component of the TLS cryptographic protocol, which the world depends on for much of its encrypted internet traffic. TLS has other cryptographic components, like public key encryption, but the ability to securely share a secret without having ever communicated before is where the Diffie-Hellman algorithm is so crucial.

It begins with the TLS handshake where the sender includes half of a public key. The receiver then sends back the other half. They both do some modulo arithmetic to compute the private key, which can't be computed by an eavesdropper. This key can then be used in TLS to share subsequent keys to allow for simpler, less computationally expensive AES communication. Hopefully no one ever finds a solution to break the modulo arithmetic the algorithm depends on, but researchers have plans for methods to supersede the Diffie-Hellman algorithm to protect against quantum computation. 

