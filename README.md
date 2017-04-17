# Surge APP Shadowsocks Encrypt Support Module
## USEAGE
- Download The SSEncrypt Module form URL Below
```url
https://raw.githubusercontent.com/Unbinilium/Surge-SSEncrypt-Module/master/SSEncrypt.module
```

## Example Conf
```txt
[Proxy]
Shadowsocks = custom,ServerIP,ServerPort,EncryptMethod,Password,https://raw.githubusercontent.com/Unbinilium/Surge-SSEncrypt-Module/master/SSEncrypt.module
```

## Notice
- Now Only Supported This Encrypt Method
```encryption
aes-128-cfb
aes-128-ofb
aes-192-cfb
aes-192-ofb
aes-256-cfb
aes-256-ofb
cast5-cfb
cast5-ofb
rc4
rc4-md5
salsa20
chacha20
chacha20-ietf
```
