# Preparando o ambiente

Criada um servidor Ubunt no _Google Cloud Plataform_ (GCP)

## UBUNTU 
   `cat /etc/issue`
   
    Retorno:
    > Ubuntu 18.04.3 LTS \n \l

### Instalando Ansible
   `sudo apt-get install ansible -y`

### Instalando VirtualBox
   `sudo apt install virtualbox`  [1]

### Instalando Vagrant
   `sudo apt install vagrant`

## Teste

### UBUNTU
Após tudo concluido, execute os comandos abaixo para checar se deu tudo certo:
    `python -V` | `python3 -V`

    Retorno:
    > python 3.6.8 

   `ansible --version`

    Deve mostrar algo parecido com a saída abaixo:

    > ansible --version
        ansible 2.6.5
        config file = None
        configured module search path = [u'/Users/nico/.ansible/plugins/modules', u'/usr/share/ansible/plugins/modules']
        ansible python module location = /usr/local/Cellar/ansible/2.6.5/libexec/lib/python2.7/site-packages/ansible
        executable location = /usr/local/bin/ansible
        python version = 2.7.15 (default, Oct  2 2018, 11:47:18) [GCC 4.2.1 Compatible Apple LLVM 10.0.0 (clang-1000.11.45.2)]

**VAGRANT**
`vagrant --version`
Vagrant 2.0.2

# Referencia

[1] - https://linuxize.com/post/how-to-install-vagrant-on-ubuntu-18-04/