make `emails/email-send.txt` from `http://alcoman.railfan.net/fear.html`



```
$ wget https://www.eff.org/files/2013/11/03/parkerkey.txt
```


```
$ gpg --import parkerkey.txt
gpg: key 9A367709: public key "Parker Higgins (EFF activism team) <parker@eff.org>" imported
gpg: Total number processed: 1
gpg:               imported: 1  (RSA: 1)
gpg: 3 marginal(s) needed, 1 complete(s) needed, PGP trust model
gpg: depth: 0  valid:   2  signed:   0  trust: 0-, 0q, 0n, 0m, 0f, 2u
gpg: next trustdb check due at 2015-11-16
```


```
$ gpg --list-keys
/home/eric/.gnupg/pubring.gpg
-----------------------------
pub   4096R/E09749E7 2014-02-09
uid                  Eric Mill (Personal contact) <eric@konklone.com>
sub   4096R/BF89D143 2014-02-09

pub   4096R/9A367709 2011-11-02 [expires: 2014-11-04]
uid                  Parker Higgins (EFF activism team) <parker@eff.org>
uid                  Parker Higgins <parker@parkerhiggins.net>
sub   4096R/D08FE908 2011-11-02 [expires: 2014-11-04]
```


```
$ gpg --output email-send.asc --sign --armor --encrypt --recipient parker@eff.org email-send.txt

You need a passphrase to unlock the secret key for
user: "Eric Mill (Personal contact) <eric@konklone.com>"
4096-bit RSA key, ID E09749E7, created 2014-02-09
```


```
gpg: D08FE908: There is no assurance this key belongs to the named user

pub  4096R/D08FE908 2011-11-02 Parker Higgins (EFF activism team) <parker@eff.org>
 Primary key fingerprint: 4FF3 AA1B D29E 1638 32DE  C765 9433 5F88 9A36 7709
      Subkey fingerprint: 3447 66D7 8A1D 9BBC 57AD  F927 6214 1335 D08F E908

It is NOT certain that the key belongs to the person named
in the user ID.  If you *really* know what you are doing,
you may answer the next question with yes.

Use this key anyway? (y/N)
```

Multiple recipients can by reusing the `--recipient` flag:

```
$ gpg --output email-send.asc --sign --armor --encrypt \
    --recipient parker@eff.org \
    --recipient mike@free.law email-send.txt
```


### paste into gmail!
