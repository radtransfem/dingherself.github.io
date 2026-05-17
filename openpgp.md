---
layout: default
title: OpenPGP
sitemap: true
---

# OpenPGP

For email encryption/signing (note that the private key for this one is <a href="https://proton.me/support/how-is-the-private-key-stored" target="_blank" rel="noopener noreferrer">managed by Proton</a>, even if they claim not to have access to the password that protects it):

- [64C4 C38D 5BEC 5BE1 FB93 BF63 DA02 A9E7 DC4B 6DAC](https://openpgpkey.dingthemself.com/64C4C38D5BEC5BE1FB93BF63DA02A9E7DC4B6DAC.asc)

If better security is needed, encrypt your message to this key (which I keep offline) and send it over directly in plain text:

- [799D A37A 5A20 DC45 6ECB  55A6 2D86 424E 27FC 7AE9](https://openpgpkey.dingthemself.com/799DA37A5A20DC456ECB55A62D86424E27FC7AE9.asc)

You can also fetch the keys via WKD. Or,

``` 
curl -s https://openpgpkey.dingthemself.com/.well-known/openpgpkey/dingthemself.com/hu/8n7kp7z3z33ssxk5e5zcya58g4o9y9az https://openpgpkey.dingthemself.com/.well-known/openpgpkey/dingthemself.com/hu/8g1e4z8b7aju56yjyd9ufqsyhndkytsr | gpg --import
```

