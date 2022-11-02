# live-audio-encryption-and-decryption

There are two types of encryptions, **Symmetric** and **Asymmetric** Encryption.

Here we are implementing **RSA Asymmetric algorithm** and **AES Symmetric algorithm**, so that we can conclude which algorithm is better and easy to encrypt and decrypt the speech/audio. 

_**RSA Algorithm**_

Let us learn the mechanism behind RSA algorithm : **>> Generating Public Key : **

Select two prime no's. Suppose P = 53 and Q = 59.

Now First part of the Public key  : n = P*Q = 3127.

 We also need a small exponent say e : 
But e Must be An integer, Not be a factor of n. 

1 < e < Φ(n) [Φ(n) is discussed below], 

Let us now consider it to be equal to 3.

    Our Public Key is made of n and e
    
**>> Generating Private Key : **

We need to calculate Φ(n) :

Such that Φ(n) = (P-1)(Q-1)     
      so,  Φ(n) = 3016
      
    Now calculate Private Key, d : 
d = (k*Φ(n) + 1) / e for some integer k

For k = 2, value of d is 2011.

_**AES Algorithm**_

The encryption process consists of various sub-processes such as sub bytes, shift rows, mix columns, and add round keys.
