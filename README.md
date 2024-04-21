# Ansible GPG keys generation

A powerful, complete and easy to use GPG key generation using Ansible locally.

**🚧 This is an early stage of the project, expect changes and issues.**


## What the playbook is doing

- [x] Generate elliptic curve keys (certify, signing, encryption and authentication).
- [x] Generate backup files for paperkey.
- [x] Generate QRCodes backups of your key.
- [x] Create or maintain LUKS encrypted backup drives.
- [x] Restore keys from LUKS encrypted backup drives.
- [x] Transfer the keys on a Yubikey.
- [x] Create a PDF document ready to be printed.

## Links

Some links that I have used to create this project.

- https://github.com/drduh/YubiKey-Guide?tab=readme-ov-file#multiple-hosts
- https://www.maketecheasier.com/backup-gpg-key-linux-paperkey/
