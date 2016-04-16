# Ansible Role: CIFS
[![Build Status](https://travis-ci.org/sbaerlocher/ansible.cifs.svg?branch=master)](https://travis-ci.org/sbaerlocher/ansible.cifs)

## Description

Mount a CIFS Folder.

## Installation

```
$ ansible-galaxy install sbaerlocher.cifs
```

## Requirements

None

## Role Variables

| Variable               | Default     | Comments (type) |
|:-----------------------|:------------|:----------------|
|samba_folder:           |             |                 |
| - name:                |             | The name        |
|   src: "//NETWORK_PATH"|             | The network path|
|   path: "LOCAL_PATH"   |             | The local path  |
|   user:                |             | The user        |
|   password:            |             | The password    |
|   file_mode:           |             | The file mode   |
|   dir_mode:            |             | The dir mode    |

## Dependencies

None

## Example Playbook

```yml
- hosts: all
  roles:
     - sbaerlocher.cifs
```

## Changelog

### 1.0

* Initial release

### 1.1

* add multiple os support

## Author

* [Simon Bärlocher](https://sbaerlocher.ch)
 
## License

This project is under the MIT License. See the [LICENSE](https://sbaerlo.ch/licence) file for the full license text.

## Copyright

(c) 2016, Simon Bärlocher