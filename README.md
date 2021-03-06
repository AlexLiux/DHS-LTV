# DHS-LTV Encryption Library

The library provides a homomorphic encryption scheme by Doroz, Hu and Sunar (DHS), along with several applications. The details of the scheme can be seen in : http://v.wpi.edu/wp-content/uploads/Papers/Publications/ntruaes.pdf. Our scheme is a single key variant of Lopez-Alt, Tromer and Vaikuntanathan (LTV) Homomorphic Encryption. The original construction can be found in : https://eprint.iacr.org/2013/094.pdf.

# Applications

Using the core homomorphic cryptosystem, we have built several applications. Examples include encrypted computation of cryptographic protocols such as AES, Prince Cipher, as well as more practical applications like PIR, Sorting Encrypted Data, Arithmetic over Encrypted Data and encrypted keyword search/completion. Sorting application is already available can be seen in applications folder, the other source codes will be avaliabe soon. All of these projects were developed for research purpose only, therefore although they provide maximum efficiency, some parts may lack a clean user interface for now. The "src" contains a more recent version of the library compared to the applications. The links for the mentioned applications:
  1. PIR      :https://eprint.iacr.org/2014/232.pdf
  2. PRINCE   :https://eprint.iacr.org/2014/233.pdf
  3. SORTING  :https://eprint.iacr.org/2015/274.pdf
  4. AUTOCOMPLETE :https://eprint.iacr.org/2015/1194.pdf

# Installation

This library uses NTL (v9.0.2 or later) with GMP support (with C++11 on). Tested on Linux environment. You can use the following commandline to compile the projects:

src: g++ main.cpp -o main -O3 fft_mult.cpp general.cpp ltv.cpp -lntl -lgmp

AES: g++ main.cpp -o main -O3 fft_mult.cpp fheaes.cpp general.cpp ltv.cpp -lntl -lgmp

PRINCE: g++ main.cpp -o main -O3 fft_mult.cpp fheprince.cpp general.cpp ltv.cpp -lntl -lgmp

# FLaSH

We are currently working on a clean and more functional version of our library (FLaSH). We do not continue supporting the current library. For your implementations we advise you to use FLaSH. The FLaSH library can be accessed using the link: https://github.com/vernamlab/FLaSH. 



