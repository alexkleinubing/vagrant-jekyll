# Vagrant - Jekyll

Configuração para o Vagrant levantar uma máquina virtual com Jekyll



## Requisitos

- Virtualbox (5.1.8)
- Vagrant (1.8.5)

*Obs.: As versões entre parenteses são as versões que testei*



## O que isso fará?

Instalará:
- Ubuntu 16.04
- Git
- RVM (Ruby Version Manager)
- Ruby 2.3.0
- Jekyll
- Bundler



## Configurações

- IP da máquina virtual: 192.168.100.179
- Sincroniza diretório atual com ```/var/www/```



## Como usar

Com o Virtualbox e o Vagrant instalados, vá o diretório onde ficam(rão) seus projetos Jekyll, e execute:

- ```git clone https://github.com/alexkleinubing/vagrant-jekyll.git .``` para copiar para diretório atual.
- ```vagrant up``` para levantar a máquina virtual
- ```vagrant ssh``` para acessar a maquina virtual
- ```cd /var/www/``` para acessar o diretório virtual dos projetos
- ```jekyll new <nome-do-projeto>``` para instalar uma aplicação Jekyll no diretório <nome-do-projeto> 
- ```cd <nome-do-projeto>``` para acessar o diretório da aplicação
- ```jekyll serve --host=0.0.0.0``` para servir a aplicação sob todos os IPs (Ctrl+C para cancelar)
- No seu navegador acesse ```192.168.100.179:4000``` para visualizar a aplicação.
