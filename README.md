# Security Merlijn busch

Opdracht 1


<?php 
  
// PHP code to illustrate the working  
// of md5(), sha1(), sha512() and hash() 
  
$str = 'Password'; 
$salt = 'Username20Jun96'; 
echo sprintf("The md5 hashed password of %s is: %s\n",  
                                $str, md5($str.$salt)); 
echo sprintf("The sha1 hashed password of %s is: %s\n", 
                                $str, sha1($str.$salt)); 
echo sprintf("The gost hashed password of %s is: %s\n",  
                            $str, sha512($str.$salt)); 
echo sprintf("The gost hashed password of %s is: %s\n",  
                        $str, hash('gost', $str.$salt));                         
                        
                          
?> 


Opdracht 2

To get the size of the modulus of an RSA key call the function RSA_size.

The modulus size is the key size in bits / 8. Thus a 1024-bit RSA key using OAEP padding can encrypt up to (1024/8) – 42 = 128 – 42 = 86 bytes.

A 2048-bit key can encrypt up to (2048/8) – 42 = 256 – 42 = 214 bytes.

Opdrach 3

Github gebruikt SHH key

Using the SSH protocol, you can connect and authenticate to remote servers and services. With SSH keys, you can connect to GitHub without supplying your username or password at each visit.

Zodat ze kunnen checken of iedereen wel inglogt is als ie pushd of pulled

Opdracht 4

BOB moet de public key van hem aan alice geven en zelf de private key houden

Alice moet de public key van haar zelf aan bob geven en de private key houden

