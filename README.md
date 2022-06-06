# Ansible Role: mount_shares

### <sub-heading>

Role tailored to my homelab environment for mounting my most commonly used shares

## Requirements

community.general<br>
ansible.posix

## Role Variables

Available variables are listed below, along with default values (see ```defaults/main.yml```)
```shell
packages:
  family: RedHat
  name: nfs-utils
cifs_user: <windows_user>
cifs_pass: <windows_password>
mounts:
  src: <share_path>
  path: <mount_directory>
  type: nfs/cifs
  opts: defaults
```
## Dependencies

None

## Example Playbook
```yaml
    - hosts: all
      roles:
        - <role name>
```

## License

MIT

## Author Information

This role was created in 2022 by [Lee Woodhouse](https://www.leewoodhouse.com/)
