# Development bootstrap with Ansible to Ubuntu

## Requeriments

Make sure that you have been installed the Ansible.

Download in: www.ansible.com

## Hand-on

Command to Install all.

`
    sudo ansible-playbook -l localhost playbook.yml
`

Command to install a specific role

`
    sudo ansible-playbook -l localhost playbook.yml --tags "<tag_name>"
`
Like that...

`
    sudo ansible-playbook -l localhost playbook.yml --tags java11-oracle
`

or multiple tags

`
    sudo ansible-playbook -l localhost playbook.yml --tags git,java11-oracle,chrome
`

## Avaliables Roles & tags:

- { role: 'git', tags: 'git'}
- { role: 'docker', tags: 'docker'}
- { role: 'java8-oracle', tags: 'java8-oracle'}
- { role: 'java11-oracle', tags: 'java11-oracle'}
- { role: 'openjdk-11', tags: 'openjdk-11'}
- { role: 'node-js', tags: 'nodejs'}
- { role: 'angular-cli', tags: 'angular-cli'}
- { role: 'vs-code', tags: 'vs-code'}
- { role: 'intellij', tags: 'intellij'}
- { role: 'chrome', tags: 'chrome'}
- { role: 'skypeforlinux', tags: 'skype'}

### TODO/WIP

- eclipse
- Double check and refactoring of all