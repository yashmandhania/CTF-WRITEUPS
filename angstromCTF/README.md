# angstrom-ctf-2021

MISC

--SANITY CHECK--
-join the discord server https://discord.gg/Dduuscw 
-the flag will be the topic of the general section (channel) on the server 

--ARCHAIC--
run the commands 
-mkdir archaicflag 
- cp /problems/2021/archaic/archive.tar.gz /archaicflag 
- cd archaic flag 
- tar -x -f archive.tar.gz
- chmod  +r flag.txt
- cat flag 

CRYPTOGRAPHY

--RELATIVELY SIMPLE ALGORITHM--
-open the RSA file to get the value of p,q,c,n and e 
-use an onlne RSA decoder to get the flag 
-resource https://www.dcode.fr/rsa-cipher


--Exclusive Cipher--
-the given flag is encoded XOR cipher 
-use an online XOR cipher decoder to get the flag by entering the key 
-resource https://www.dcode.fr/xor-cipher


--Keysar v2--
-Used https://www.boxentriq.com/code-breaking/cipher-identifier to check the output file

-Found that it was monosubstituion cipher,simple brute force attack got us to a readable paragraph

-Flag:
actf{keyedcaesarmorelikesubstitution


REVERSE ENGINEERING

--FREE FLAGS!!1!!--
-Connecting to the server (using nc shell.actf.co 21703)returned a question,answering the questions would return the flag.txt file.
Using gidhra got the C code of program

-The first answer was 31337 (hex to decimal conversion)

-Second question had two equations
Solving them gave the two numbers
 723 419 
-The third answer was banana 

-Flag:
actf{what_do_you_mean_bananas_arent_animals}
