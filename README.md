# GPG private key backups

**DO NOT SUBMIT UNENCRYPTED PRIVATE KEYS**

This repositor is a place to backup /r/Futurology uers's private
keys if they so choose. You should encrypt your private key using
another gpg key of your choosing.

If you wish to protect against forgetting your passphrase, you should
store your un-passphrase-protected key in here (encrypted with another key).

To export your key and encrypt with another key, use the following command:

```bash
gpg --export-secret-key lordvadr@futurology.social | \
    gpg -ear you@somewhere.com -r someotherkey@somewherelse.com \
    > you@youremail.wherever.priv
```


To export your public key for use in the automation, use:

```bash
gpg -a --export lordvadr@futurology.social > lordvadr@futurology.social.pub
```
