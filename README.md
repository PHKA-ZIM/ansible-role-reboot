# Add cron for server reboot with ansible

## Installation steps

- Go to you ansible project folder
- Add following to your requirements file

```
- src: https://github.com/PHKA-ZIM/ansible-role-reboot
  name: ansible-role-reboot
```

- Install to project roles path
```
ansible-galaxy install -r requirements.yml --roles-path ./roles
```

## Use ansible-role-reboot

- Import role and override role variables, e.g.
```
- name: Add reboot cronjob
  roles:
    - role: ansible-role-reboot
```

- All available role vars can be found in `defaults`
