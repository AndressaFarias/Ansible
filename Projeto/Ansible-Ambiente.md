# Preparando o ambiente

Criada uma máquina Ubuntu no _Google Cloud Plataform_ (GCP)

## UBUNTU 
   `cat /etc/issue`
   
    Retorno:
    > Ubuntu 18.04.3 LTS \n \l

### Instalando Ansible
   `sudo apt-get install ansible`

### Instalando VirtualBox
   `sudo apt install virtualbox`  [1]

### Instalando Vagrant
   `sudo apt install vagrant` [1]

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


## MacOS

### Instalar Ansible e Python 

Instale o _brew_ através do comando abaixo:
    `/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`

O comando abaixo instala o _Python_ e o _Ansible_:
    `brew install python@2 ansible@2.0`

### Vagrant
* Acesse o site do Vagrant pegue o link para download para sistema operacional
    ` wget https://releases.hashicorp.com/vagrant/2.2.6/vagrant_2.2.6_linux_amd64.zip`

* Descompacte

* Teste de instalação
    `./vagrant version`


## Windows
    Ansible não tem suporte para Windows.


# Referencia

[1] - https://linuxize.com/post/how-to-install-vagrant-on-ubuntu-18-04/