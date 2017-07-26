# Surge APP Shadowsocks Encrypt Support Module

## Usage
- Download The SSEncrypt Module form URL Below
```url
https://raw.githubusercontent.com/Unbinilium/Surge/master/SSEncrypt.module
```

## Example Conf
- It is Only the Proxy Part, and You're Suppose to fill **SeverIP**、**ServerPort**、**EncryptMethod** and **Paddword** Manually
```conf
[Proxy]
Shadowsocks = custom,ServerIP,ServerPort,EncryptMethod,Password,https://raw.githubusercontent.com/Unbinilium/Surge/master/SSEncrypt.module
```
- If You're using <a href="https://github.com/shadowsocks/simple-obfs" target="_blank">simple-obfs</a>, Please try this example after fill **ObfsMethod** and **ObfsHost** Manually
```conf
custom,ServerIP,ServerPort,EncryptMethod,Password,https://raw.githubusercontent.com/Unbinilium/Surge/master/SSEncrypt.module,obfs=ObfsMethod,obfs-host=ObfsHost
```

## Notice
- Now Only Supported these Encrypt Method
```encrypt
rc4
rc4-md5
rc2-cfb
bf-cfb
des-cfb
idea-cfb
seed-cfb
cast5-cfb
camellia-128-cfb
camellia-192-cfb
camellia-256-cfb
aes-128-cfb
aes-192-cfb
aes-256-cfb
aes-128-ctr
aes-192-ctr
aes-256-ctr
salsa20
chacha20
chacha20-ietf
aes-128-gcm
aes-192-gcm
aes-256-gcm
chacha20-ietf-poly1305
```
- Now Supported these Obfs Method
```obfs
http
tls
```
- Also, the default Obfs Host is here. Change it if you like. Suggest to Use CDN Domain which is not Blocked
```obfs
cloudfront.com
```

## Suggestions
- For Better Security, these Encrypt Method are Supported <a href="https://en.wikipedia.org/wiki/Authenticated_encryption" target="_blank">AEAD</a> (Authenticated Encryption with Associated Data)
```encrypt
aes-128-gcm
aes-192-gcm
aes-256-gcm
chacha20-ietf-poly1305
```
- Add a TLS Obfs and Change the default Obfs Host
- Try to Use TCP Fast Open by Add that perfix ```,tfo=true``` in the end of the line of the Proxy Part

## Manual for Surge App
- View Official Surge <a href="https://manual.nssurge.com/" target="_blank">Manual Guide </a>
