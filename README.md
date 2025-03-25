Desafio de projeto 1

O desafio, proposto pelo curso Santander - Linux para iniciantes no dio.me, consiste em criar um arquivo do tipo Bash Script e colocar dentro dele toda a infraestrutura de usuários, grupos de usuários, diretórios e permissões que serão criadas automaticamente. 

Comandos utilizados no terminal:

* mkdir /nome_rep: Utilizado para criação de repositórios.
* groupadd nome_grupo: Utilizado para a criação de grupos.
* useradd nome_usuario: Utilizado para a criação de usuários.
* chown root:nome_grupo /nome_rep: Utilizado para alterar o dono de todos os repositórios, sendo esse o user root.
* chmod permissoes/nome_rep: Utilizado para alterar as permissões dos repositórios.

Parâmetros de useradd:

* -m: cria o diretório pessoal do usuário.
* -s: shell de login da nova conta (/bin/bash).
* -p $(openssl passwd -crypt Senha123): atribui senha automaticamente.
* -G: lista de grupos complementares da nova conta.

Permissões de chmod: 

* 0: Nenhuma permissão de acesso.
* 1: Permissão de execução.
* 2: Permissão de escrita.
* 4: Permissão de leitura.

Para obter qualquer permissão, é somado os números correspondentes. No caso do desafio o diretório /publico teria permissão total(777), enquanto os demais teriam permissão apenas do dono e do grupo pertencente ao repositório(770).

Para mais informações: https://www.linux.ime.usp.br/~albasalo/Apostila/apostila.pdf
================================================================================================================================================================================================================
Desafio de projeto 2

O segundo desafio de projeto consiste em criar um script de um servidor web utilizando o Apache. Nele temos os comandos de update e upgrade, as instalações do apache2 e do unzip, além de baixar os arquivos do repositório github do professor/instrutor Denilson Bonatti, sua descompactação e cópia para onde está o servidor web.
