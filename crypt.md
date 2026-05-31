# Encrypt file with openssl

```sh
openssl enc -aes-256-cbc -salt -pbkdf2 -iter 998799 -in file.txt -out file.txt.enc
```


# Decrypt file with openssl

```sh
openssl enc -aes-256-cbc -pbkdf2 -iter 998799 -d -in file.txt.enc -out file.txt
```


# Cryptsetup plain mode

```sh
cryptsetup open --type plain --cipher aes-xts-plain64 --hash sha256 --key-size 512 --offset 226715894 --size 12812288 /dev/sda hidden
```
