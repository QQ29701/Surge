# Surge APP Shadowsocks Encrypt Support Module

## Usage
- Download The SSEncrypt Module form URL Below
```url
https://raw.githubusercontent.com/Unbinilium/Surge-SSEncrypt-Module/master/SSEncrypt.module
```

## Example Conf
- It is Only the Proxy Part, and You're Suppose to fill **SeverIP**、**ServerPort**、**EncryptMethod** and **Paddword** Manually
```txt
[Proxy]
Shadowsocks = custom,ServerIP,ServerPort,EncryptMethod,Password,https://raw.githubusercontent.com/Unbinilium/Surge-SSEncrypt-Module/master/SSEncrypt.module
```

## Notice
- Now Only Supported These Encryption Method
```encryption
rc4
rc4-md5
aes-128-cfb
aes-192-cfb
aes-256-cfb
aes-128-ctr
aes-192-ctr
aes-256-ctr
bf-cfb
camellia-128-cfb
camellia-192-cfb
camellia-256-cfb
cast5-cfb
des-cfb
idea-cfb
rc2-cfb
seed-cfb
salsa20
chacha20
chacha20-ietf
aes-128-gcm
aes-192-gcm
aes-256-gcm
chacha20-ietf-poly1305
```
