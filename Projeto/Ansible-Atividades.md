# Começando com Ansible

1. Crie uma pasta com o nome wordpress_com_ansible.

2. Baixe o arquivo [Vagrantfile](C:\Users\andressa.farias\Documents\Projetos\E-learning\Ansible\Vagrantfile)


3. Utilizando o terminal, dentro da pasta **wordpress_com_ansible** execute o comando abaixo:
    `vagrant up`

    Retorno:
    ```
        Bringing machine 'wordpress' up with 'virtualbox' provider...
        ==> wordpress: Checking if box 'ubuntu/trusty64' is up to date..
    ```

4) Crie o arquivo de inventário hosts (Dentro da mesma pasta em que está o VagrantFile) e comece colocando o IP da máquina virtual, defina um grupo também (no curso, demos o nome de wordpress):

[wordpress] <!--Grupo, define para o anible para quê o ervidor será utilizado-->
172.17.177.40 <!--IP dá máquina declarada no Vagrantfile -->

5) Teste se sua máquina virtual está funcionando, executando o código abaixo:
    `vagrant ssh`
    
    Utilize o atalho CTRL + C para deslogar da máquina virtual.

6) Rode o comando Ansible abaixo para ter um simples hello world:
    `ansible wordpress -u vagrant --private-key .vagrant/machines/wordpress/virtualbox/private_key -i hosts -m shell -a 'echo Hello, World'`

7) Para ter uma saída mais verbosa, utilize o comando abaixo, onde foi incluído o parâmetro -vvvv

ansible -vvvv wordpress -u vagrant --private-key .vagrant/machines/wordpress/virtualbox/private_key -i hosts -m shell -a 'echo Hello, World'
DISCUTIR NO FORUM


## Como subir sua máquina virtual pelo Vagrant
## Como utilizar a chave privada no Ansible para se comunicar com a VM
## Como executar um Hello, World utilizando Ansible



# Erros

Ao executar o comando `vagrant ssh` é retornada a mensagem:
```
    ssh_exchange_identification: read: Connection reset by peer
```

O problema pode ser causado pois a chave SSH é insegura. Para verificar detalhes do erro, é  indicada a execução do comando: 
    `vagrant ssh --debug`

Não foi reportado problema na chave

Executado o comando 
    `vagrant halt`
    Para fazer o shutdown da máquina.

