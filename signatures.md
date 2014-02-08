# What is signed email?, 
## or: What is this .asc attachment all about?

The .asc attachment on this message is my digital signature. If you set up your email to use PGP (pretty good privacy), this signature (and yours) will let us encrypt our conversations so that we are the only ones who can read the contents. It's like sending email in an envelope rather than written on a postcard.

A **verified signature** provides two properties:

* **authentication**: this message really is from me (your friend, not an impostor)
* **integrity**: this message hasn't been tampered with since me (your friend) wrote it

However, you'll need to verify the signature before you can be sure of either property. Just seeing this .asc attachment or some PGP-related gobbledy-gook at the bottom of an email message isn't enough to verify it (see *Insecure ways to verify signatures* below) as a message from your friend that hasn't been tampered with. 

Read more at: ...

## Tools for using OpenPGP on your device

[GPG](https://www.gnupg.org/)

[MacGPG Tools](https://gpgtools.org/) - download and install the suite

[mailvelope](https://mailvelope.com/) - OpenPGP encryption for webmail. It's a browser extension that allows exchange of encrypted emails following the OpenPGP encryption standard. 

## What signed email *doesn't* guarantee

It doesn't guarantee that the person claimed in the FROM line is actually the person you think it's from. You'll need to confirm that the private key used to sign the message matches the key held by that person. Check the Short ID and/or talk with them to confirm.

It doesn't guarantee that others haven't read your message.

Or that people haven't gathered the meaning of your message from parts of your email that are NOT encrypted, like the subject line, or time and other meta-data associated with your message.



## What's next?

Download, install, and create your first key. 

Upload it to a keyserver.

Find a friend and do the same.

Try sending an encrypted email between the two of you.

Optional: Sign each other's keys (in person, confirming that you're signing the right keys).

## Insecure ways to verify signatures
![XKCD explains PGP.](http://imgs.xkcd.com/comics/pgp.png)
