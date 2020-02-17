# Ansible: Sua infraestrutura como código

Infraestrutura como código é a base da cultura DevOps, encurtando assim o ciclo de feedback entre os times de desenvolvimento e os de infraestrutura.

As máquinas gerenciadas pelo Ansible só precisam do Python e de um servidor SSH instalados.

É apartir da máquina de controle com o Ansible instalado que gerenciamos as outras máquinas.


## Componentes 

**hosts:** Indica para qual grupo ou host do arquivo de inventário o Ansible vai aplicar as tarefas.

**tasks:** Lista os principais comandos a serem executados nos hosts selecionados.


## Alguns conceios de Ansible

* **Inventário** — É uma lista de hosts (nós) podendo ser o nome — www.exemplo.com.br –, o endereço IP — 192.168.0.10 –, uma faixa de nomes ou endereços IP — www[1:9].exemplo.com.br ou 192.168.1.[10:99] — relacionados individualmente ou dentro de um grupo.

* **Módulo** — São trechos de código executados remotamente em um nó e que controlam recursos do sistema como serviços, pacotes, arquivos ou até mesmo a execução de comandos. Eles podem ser usados de forma direta ou através dos playbooks.

* **Nó** — Ou, se preferir, node. É um host, ou melhor, um host gerenciado pelo Ansible.

* **Playbook** — É um arquivo no formato YAML que permite execução de diversos módulos, agrupá-los em tarefas, adicionar e atribuir variáveis.