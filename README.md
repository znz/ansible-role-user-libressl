# Ansible role for libressl of user

- Setup libressl into home directory

## Requirements

- Debian
- Ubuntu

## Role Variables

- `libressl_user`: user
- `libressl_group`: group
- `libressl_download_dir`: download directory
- `libressl_build_dir`: build directory
- `libressl_prefix`: prefix argument of configure
- `libressl_version`: libressl version
- `libressl_sha256`: tarball checksum of libressl

## Dependencies

None.

## Example Playbook

Normal usage:

    ---
    - hosts: all
      become: no
      roles:
      - znz.user-libressl

## Example requirements.yml

    - src: https://github.com/znz/ansible-role-user-libressl
      version: master
      name: znz.user-libressl

## License

MIT License
