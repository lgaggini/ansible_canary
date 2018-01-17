# ansible_canary

ansible_canary is a local ansible playbook to generate an hostgroup [canarino](https://en.wiktionary.org/wiki/canary_in_a_coal_mine) including one random host from every ansible inventory group to perform canary tests and releases.

## Usage
### Dynamic
You can edit and use `canary.yml` playbook to dinamically generate the canarino hostgroup and apply some task to it.
### Static
Otherwise you can use the `canary_out.yml` playbook to generate a static inventory file for the canarino hostgroup. It will compile the `ansible-canary-hosts.j2` template into ansible-canary-hosts inventory file.

## Run
```bash
git clone https://github.com/lgaggini/ansible_canary.git
cd ansible_canary
ansible-playbook canary.yml (canary_out.yml)
```
