# Encryption and Steganography in Python #

The Key_Generator notebook uses Crypto and cryptography modules to create a public key and private key. 
The Source_Side notebook uses DNA and AES method to encrypt a secret message and then employ the private key to sign the encrypted message. At the end, the encrypted message gets hidden in an image by stepic module.
On the other side, the Target_Side notebook takes the image and leverages the public key on it to decode the signature (this phase could detect the middle-man attack because if the message was attacked by a middle man, the public key couldn't be able to decode the signature). After decoding and extracting the encrypted message from the image by PIL and stepic modules, the program uses the same DNA and AES methods to reveal the original message.
