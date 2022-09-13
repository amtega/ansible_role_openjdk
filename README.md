# Amtega openjdk role

This is an [Ansible](http://www.ansible.com) role to deploy openjdk Runtime Environment.

## Role Variables

A list of all the default variables for this role is available in `defaults/main.yml`.

The role setups the following facts:

- `openjdk_java_home`: home path of the deployed openjdk java
- `openjdk_java_default_artifact`: dict with the default artifact for downloading openjdk java. Only available when download artifact is not defined.
- `openjdk_effective_version`: openjdk effective version (useful if you use `latest` for version)

## Example Playbook

This is an example playbook:

``` yaml
---
- hosts: localhost
  roles:
    - amtega.openjdk
```

## Testing

Tests are based on [molecule with docker containers](https://molecule.readthedocs.io/en/latest/installation.html).

```shell
cd amtega.openjdk

molecule test --all
```

## License

Copyright (C) 2022 AMTEGA - Xunta de Galicia

This role is free software: you can redistribute it and/or modify it under the terms of:

GNU General Public License version 3, or (at your option) any later version; or the European Union Public License, either Version 1.2 or – as soon they will be approved by the European Commission ­subsequent versions of the EUPL.

This role is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more details or European Union Public License for more details.

## Author Information

- José Enrique Mourón Regueira
