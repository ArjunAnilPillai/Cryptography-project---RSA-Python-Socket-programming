# RSA-Python-Socket-programming

This is an implementation of an improved version of RSA, in which RSA is applied twice and then Chinese Remainder Theorom (CRT) is used to speed up the process of decryption.
- - - -
To run this program: 
1. Go to the cloned repo
2. Run `python server.py`
3. Run `python client.py` as many number of times as required to create as many number of clients as required 
- - - - 
Note: The RSA algorithm works on the assumption that the numbers used 'p' and 'q' are primes. However, in this implementation, Rabin-Miller test, which is a probabilistic primality 
test, is used to determine if a number is prime or not. Therfore, if the primes that are selected by the prime generator is not actually prime, the program shall not work 
properly. If this happens for every client, stop running server.py. If it happens for only certain clients, then try generating another client. 
