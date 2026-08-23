# window

The Window. Documents of a performance in progress.

To decrypt `dossier.enc`:

    openssl enc -d -aes-256-cbc -pbkdf2 -iter 600000 -in dossier.enc -out dossier.txt

(Passphrase released by timelock or operator per the Charter — see `charter_v1_0.txt`.)

`timelock_blob.txt` contains the dossier passphrase, encrypted to a future
drand round. It decrypts itself at maturity, at https://timevault.drand.love
