# Playbook

Arquivo sempre inicia com `---`

O elemento de primeiro nível é sempre uma lista que começa com um filtro chamado hosts, esse filtro serve para definir em quais hosts do inventário o Ansible vai trabalhar

O segundo elemento da lista é o **tasks**: ele lista de comandos a serem aplicados nos hosts filtrados.

O módulo para alterar nosso servidor ubuntu, utiliza o **apt**