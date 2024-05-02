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
- [x] Initialise a password store for _pass_.
- [x] Configure the SSH agent to use GPG.


## Playbooks

| Playbook     | Description                                                     |
|--------------|-----------------------------------------------------------------|
| main.yml     | Main playbook to generate a key                                 |
| backup.yml   | Backup the key on a usb drive encrypted with luks               |
| print.yml    | Create a PDF with all the information needed to restore the key |
| restore.yml  | Restore the key from a backup drive                             |
| yubikey.yml  | Copy the private keys on a yubikey and configure GPG            |
| yubikey.yml  | Copy the private keys on a yubikey and configure GPG            |
| pass.yml     | Initialise password store for Linux pass utility                |
| packages.yml | Install the packges required                                    |

## Examples

[Example of a printed backup sheet](samples/backup.pdf)


## Links

Some links that I have used to create this project.

- https://github.com/drduh/YubiKey-Guide?tab=readme-ov-file#multiple-hosts
- https://www.maketecheasier.com/backup-gpg-key-linux-paperkey/
