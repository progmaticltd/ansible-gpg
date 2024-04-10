# Ansible GPG keys generation

An easy to use GPG key generation using Ansible.


## What the playbook is doing

- [x] Generate elliptic curve keys (certify, signing, encryption and authentication).
- [x] Generate backup files for paperkey.
- [x] Generate QRCodes backups of your key.
- [x] Create encrypted backup using luks.
- [x] Generate document to print with the credentials.
- [ ] Transfer the keys on a Yubikey.


## Links

Some links that I have used to create this project.

- https://github.com/drduh/YubiKey-Guide?tab=readme-ov-file#multiple-hosts
- https://www.maketecheasier.com/backup-gpg-key-linux-paperkey/
