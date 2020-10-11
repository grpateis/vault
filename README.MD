Projeto local
: localhost - sem inventory

Instalação de playbook usando Ansible VAULT

TREINAMENTO ANSIBLE.

-- Dicas

ansible-playbook main.yml --ask-vault-pass
ansible-vault encrypt vars/api_key.yml
ansible-vault decrypt vars/api_key.yml
ansible-vault rekey vars/api_key.yml (mudar senha)
tags: permitem executar somente uma task


com automação
: testar
ansible-playbook main.yml --vault-password-file ~/.ansible/api-key-pass.txt
changed_when:
failed_when:
ignore_errors:


