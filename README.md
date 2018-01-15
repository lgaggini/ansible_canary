# ansible_canary

ansible_canary is a local ansible playbook to generate an hostgroup [canarino](https://en.wiktionary.org/wiki/canary_in_a_coal_mine) including one random host from every ansible inventory group to perform canary tests and releases.

## Run
```bash
git clone https://github.com/lgaggini/ansible_canary.git
cd ansible_canary
ansible-playbook canary.yml
```
