# Ansible-tricks



## Usage

For example against localhost

```bash
alex@vostok:~/ansible-tricks$ ansible-playbook -i "localhost," -c local playbook.yml
```

## Use one line with servers (-m raw for use without simplejson python package)
```bash
ansible all -i voyager,sputnik,vostok, -a "/bin/cat /etc/issue" -u root -m raw
```
