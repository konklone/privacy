### copy from gmail into text file

emails/email-received.asc


```
$ gpg --output email-received.txt --decrypt email-received.asc
```

```
You need a passphrase to unlock the secret key for
user: "Eric Mill (Personal contact) <eric@konklone.com>"
4096-bit RSA key, ID BF89D143, created 2014-02-09 (main key ID E09749E7)
```


```
gpg: encrypted with 4096-bit RSA key, ID D08FE908, created 2011-11-02
      "Parker Higgins (EFF activism team) <parker@eff.org>"
gpg: encrypted with 4096-bit RSA key, ID BF89D143, created 2014-02-09
      "Eric Mill (Personal contact) <eric@konklone.com>"
gpg: Signature made Sun 09 Feb 2014 03:21:22 PM EST using RSA key ID 9A367709
gpg: Good signature from "Parker Higgins (EFF activism team) <parker@eff.org>"
gpg:                 aka "Parker Higgins <parker@parkerhiggins.net>"
gpg: WARNING: This key is not certified with a trusted signature!
gpg:          There is no indication that the signature belongs to the owner.
Primary key fingerprint: 4FF3 AA1B D29E 1638 32DE  C765 9433 5F88 9A36 7709
```


now read email-received.txt