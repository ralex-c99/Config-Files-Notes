# Crypto

`md5sum <file>` = generates md5 hash of a file
`sha1sum <file>` = generates sha1 hash of a file

`gpg --gen-key` = generates (private, public) key pair
`gpg --list-keys` = list all public keys
`gpg --list-secret-keys` = list all secret keys
`gpg --detach-sign <file>` = generates a signature for a file
`gpg --export -a <key-id> <public-key.name>` = export a public key
`gpg --keyserver <server-name> --send-keys` = send your keys to a server
`gpg --delete-keys <key-id>` = delete public keys
`gpg --delete-secret-keys <key-id>` = delete secret keys (AVOID THIS!!!)
`gpg --export-secret-keys -a <key-id>` = export secret key
`gpg --import pubkey.asc` = import public key
`gpg --allow-secret-key-import sec.key` = import secret key
`gpg --verify test.sig test`= verify a file using the signature
`gpg --encrypt --recipient friend_pub.key file_w_msg` = encrypt a file using a public key
`gpg --decrypt test.gpg` = decrypt a file