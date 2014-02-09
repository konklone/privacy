
```
$ gpg --gen-key

gpg (GnuPG) 1.4.14; Copyright (C) 2013 Free Software Foundation, Inc.
This is free software: you are free to change and redistribute it.
There is NO WARRANTY, to the extent permitted by law.

Please select what kind of key you want:
   (1) RSA and RSA (default)
   (2) DSA and Elgamal
   (3) DSA (sign only)
   (4) RSA (sign only)
Your selection?
```


```
RSA keys may be between 1024 and 4096 bits long.
What keysize do you want? (2048)
```


```
Requested keysize is 4096 bits
Please specify how long the key should be valid.
         0 = key does not expire
      <n>  = key expires in n days
      <n>w = key expires in n weeks
      <n>m = key expires in n months
      <n>y = key expires in n years
Key is valid for? (0)
```


```
Key does not expire at all
Is this correct? (y/N) y
```


```
You need a user ID to identify your key; the software constructs the user ID
from the Real Name, Comment and Email Address in this form:
    "Heinrich Heine (Der Dichter) <heinrichh@duesseldorf.de>"

Real name:
```


```
Real name: Eric Mill
Email address: eric@konklone.com
Comment: Personal contact


You selected this USER-ID:
    "Eric Mill (Personal contact) <eric@konklone.com>"

Change (N)ame, (C)omment, (E)mail or (O)kay/(Q)uit?
```


```
We need to generate a lot of random bytes. It is a good idea to perform
some other action (type on the keyboard, move the mouse, utilize the
disks) during the prime generation; this gives the random number
generator a better chance to gain enough entropy.
```


```
Not enough random bytes available.  Please do some other work to give
the OS a chance to collect more entropy! (Need 203 more bytes)
```


```
gpg: key E09749E7 marked as ultimately trusted
public and secret key created and signed.

gpg: checking the trustdb
gpg: 3 marginal(s) needed, 1 complete(s) needed, PGP trust model
gpg: depth: 0  valid:   2  signed:   0  trust: 0-, 0q, 0n, 0m, 0f, 2u
gpg: next trustdb check due at 2015-11-16
pub   4096R/E09749E7 2014-02-09
      Key fingerprint = 7F52 586D DB0F 8CAC A8AC  F344 398F C722 E097 49E7
uid                  Eric Mill (Personal contact) <eric@konklone.com>
sub   4096R/BF89D143 2014-02-09
```


```
$ gpg --list-keys

/home/eric/.gnupg/pubring.gpg
-----------------------------
pub   4096R/E09749E7 2014-02-09
uid                  Eric Mill (Personal contact) <eric@konklone.com>
sub   4096R/BF89D143 2014-02-09
```
