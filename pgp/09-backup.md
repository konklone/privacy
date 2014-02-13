### exporting secret key to prepare for backup


```
$ gpg --armor --export-secret-keys eric@konklone.com
```


```
-----BEGIN PGP PRIVATE KEY BLOCK-----
Version: GnuPG v1.4.14 (GNU/Linux)

[ ... contents of key ... ]

-----END PGP PRIVATE KEY BLOCK-----
```


```
$ gpg --armor --export-secret-keys eric@konklone.com > eric-private-key.asc
```


### generating private key fingerprint for signing party or whatever

