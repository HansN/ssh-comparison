---
title: SSHJ
homepage: https://github.com/hierynomus/sshj
source-repository: https://github.com/hierynomus/sshj
changelog: https://github.com/hierynomus/sshj
license: "[Apache-2.0](https://github.com/hierynomus/sshj/blob/master/LICENSE)"
#first-release:
#    date: YYYY-MM-DD
latest-release:
    version: 0.15.0
    date: 2015-11-20
#changelog: URL
client: no
server: no
library: client
protocols:
    cipher:
        - aes128-ctr
        - aes192-ctr
        - aes256-ctr
        - aes128-cbc 
        - aes192-cbc 
        - aes256-cbc 
        - 3des-ctr
        - 3des-cbc
        - blowfish-ctr
        - blowfish-cbc
        - twofish128-ctr
        - twofish192-ctr
        - twofish256-ctr
        - twofish128-cbc
        - twofish192-cbc
        - twofish256-cbc
        - twofish-cbc
        - serpent128-ctr
        - serpent192-ctr
        - serpent256-ctr
        - serpent128-cbc
        - serpent192-cbc
        - serpent256-cbc
        - idea-ctr
        - idea-cbc
        - cast128-ctr
        - cast128-cbc
        - arcfour
        - arcfour128
        - arcfour256
        - camellia128-ctr
        - camellia192-ctr
        - camellia256-ctr
        - camellia128-cbc
        - camellia192-cbc
        - camellia256-cbc
        - camellia128-ctr@openssh.org
        - camellia192-ctr@openssh.org
        - camellia256-ctr@openssh.org
        - camellia128-cbc@openssh.org
        - camellia192-cbc@openssh.org
        - camellia256-cbc@openssh.org
    compression:
        - zlib              # disabled by default
        - zlib@openssh.com  # disabled by default
        - none
    hostkey:
        - ssh-rsa
        - ssh-dss
        - ecdsa-sha2-nistp256
        - ssh-ed25519
    kex:
        - curve25519-sha256@libssh.org
        - diffie-hellman-group-exchange-sha256
        - ecdh-sha2-nistp521
        - ecdh-sha2-nistp384
        - ecdh-sha2-nistp256
        - diffie-hellman-group-exchange-sha1
        - diffie-hellman-group14-sha1
        - diffie-hellman-group1-sha1
    mac:
        - hmac-sha1
        - hmac-sha1-96
        - hmac-md5
        - hmac-md5-96
        - hmac-sha2-256
        - hmac-sha2-512
    userauth:
        - publickey
        - password
        - keyboard-interactive
        - gssapi-with-mic
        - hostbased
---
* Pure Java implementation.
