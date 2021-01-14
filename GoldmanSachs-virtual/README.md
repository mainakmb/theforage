# Used stuffs and guidence
I used __hashcat__, an advanced password cracking tool to recover passwords from hashes.

#### Download hashcat
```
https://hashcat.net/hashcat/
Get the binaries
```
#### Change the passwd file
For simplier usage, I changed the __passwd_dump.txt__ file, removed the username and kept only the hashes.

#### Use hashcat
Run hashcat in CLI 
```
hashcat --help
hashcat -m 0 -a 3 -d 1 passwd_dump.txt
```
Here I am using hash type as __MD5__ ,attck type __Brute Force__ , then I selected device as -d 1, as Device 1 was my GPU. GPU makes it easier to compute the hashes.
After performing command hashcat will use your CPU/GPU for computing those hashes to a valid password format.
Please follow the __solution-statement__ for analysis.
