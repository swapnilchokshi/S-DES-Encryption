# S-DES Encryption
## Simplified Data Encryption Standard Algorithm in C Language

Until the introduction of Advanced Encryption Standard (AES) in 2001, the Data Encryption Standard (DES) was the most widely used encryption schemes.
DES was issued in 1977 by NIST, as FIPS-46.

DES encrypts 64-bit blocks using a 56-bit key and produces 64-bit ciphertext through a series of steps.

S-DES or Simplified Data Encryption Standard is a simplified version of DES algorithm which is a block cipher that inputs 8-bit plaintext or ciphertext and uses 10-bit key for encryption and decryption.
S-DES was designed for educational purposes only, to help students learn about modern cryptanalytic techniques. SDES has similar properties and structure as DES, but has been simplified to make it much easier to perform encryption and decryption by hand with pencil and paper.

The Encryption Processing of plaintext proceeds in 3 phases:-

1) First, the plaintext passes through an initial permutation (IP) that rearranges the bits to produce permutted output.

2) The permutted output is then passed through 16 rounds of both Permutation and Substitution functions. The left and right halves of output are swapped to produce the preoutput.

3) Finally, preoutput is passed through a permutation (IP-1) that is inverse of initial permutation function, to produce ciphertext.

The key is passed through a permutation function. Then a subkey is produced for each 16 rounds by combination of left circular swift and a permutation. The permutation function is the same for every round, but a different subkey is produced because of the repeated shifts of key bits.

![DES ENCRYPTION AND DECRYPTION PROCESS](https://www.brainkart.com/media/extra/0QHPefM.jpg)

![KEY GENERATION](https://www.brainkart.com/media/extra/ZaaYJhs.jpg)

![WHOLE PROCESS](https://sandilands.info/sgordon/images/sdes-encrypt-1-r123.png)

