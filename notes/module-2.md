# Module 2

Chapters to read: 

* Ch2: Cryptographic Tools - in the Computer Security Principles and Practice Book
* Ch3: User Authentication - in the Computer Security Principles and Practice Book
* Ch 4: The Crown Jewels - Project Zero Trust
* Ch 5: The Identity Cornerstone - Project Zero Trust

## Chapter 2 - Cryptographic Tools

### Symmetric Encryption

Encryption scheme using a secret key shared by the sender and recipient along with an encryption/decryption algorithm to transmit encrypted ciphertext.

Even if someone knows the algorithm but doesn't have the key, there is no way of decypting the ciphertext.

#### Attacks

* Cryptanalysis
  * Exploits the characteristics of the algorithm to attemp to deduce a specific plaintext or to deduce the key being used.
* Brute-Force
  * try every possible key on a piece of ciphertext until intelligible plaintext is obtained.

#### Algorithms

* DES
  * 56-bit key is too small for modern brute force attacks
* Triple DES
  * Repeats DES three times with two or three unique keys, key size of 112 or 168 bits
  * DES is very well researched so that's a plus
  * Sluggish in practice
* AES
  * ECB (Electronic codebook mode) does multi-block encryption, originally, but different modes of operation have been developed to overcome weaknesses of ECB.


#### Ciphers

* Block Cipher
  * Processes the input one block of elements at a time
  * Produces an output block for each input block
  * More common
  * Can reuse keys
* Stream Cipher
  * Processes the input elements continuously
  * Produces output one element at a time
  * Encrypts plaintext one byte at a time
  * Pseudorandom stream is one that is unpredictable without
knowledge of the input key
  * Primary advantage is that they are almost always faster
and use far less code
