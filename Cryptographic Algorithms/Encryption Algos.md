Encryption Algos

**Encryption Algos**
| Algos | DES | 3DES | RC4 | AES | Blowfish | Twofish |
|-----|------|-----|-----|----------|---------|-----|
| Key Bit Length | 64 | 3 | 40-2048 | 128, 192, 256 | 1-448 bit | 128-256 |
| Block | - | - | Steam | - | - | - |
| Weakness | Small key, easy brute | 3 times harder but easy brute | key gen issue, made WEP bad too | Strong | Strong | Strong |

**Hashing Algos**
| Algos | MD5 | SHA-1 | SHA-2 | SHA-3 | HMAC | RIPEMD |
|-------|-----|-------|-------|-------|------|--------|
| Output bits | 128 | 128 | 256 | 256-512 | Same as algo used | 128-320 |
| Block Size  | 512 | 512 | 512 | 576-1152 | Same as algo used | ^ |
| Collision | - | - | - | - | - | Weak, 128 bit result is too small, larger key is ok | 

**Cryptographic Protocol**
| Protocols | WEP | WPA | WPA2 | CCMP | TKIP | 
|-----------|-----|-----|------|------|------|
| Based on  | RC4 | RC4 and TKIP or LEAP | AES, counter mode and CCMP | replace WEP, combine with WPA2 | replace WEP, combine with WPA2, RC4 |
| Features  |     | PSK or ENT | PSK or ENT | AES | key-mixing function with IV and a secret root key 
| Bad       | Yes | Yes | No | No | Yes
| Why       | Static common key, poor IV | Brute force RC4 | 

**Authentication Protocols**
| Protocols | EAP | PEAP | EAP-FAST | EAP-TLS | EAP-TTLS | IEEE 802.1x | RADIUS Federation |
|-----------|-----|------|----------|---------|----------|-------------|-------------------|
| Acronym   | Extensible Authenticaion Protocol | Protected EAP | Flexable Auth via Secure Tunneling | EAP Transport Layer Security | EAP Tunneled Transport Layer Security |  | |
| What | Auth Framework, in the clear | Protects EAP within TLS | Cisco protcol, replace LEAP | IETF standard over TLS, **STRONGEST** | extension of EAP-TLS, creates VPN like tunnel, username not in clear |  |  |