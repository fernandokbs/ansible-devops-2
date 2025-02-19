# Comando para copiar un archivo del host al servidor remoto
ansible -m copy -a"src=./hosts dest=/home/ubuntu" tutorial

# Comando para crear un archivo en el servidor remoto
ansible -m file -a "path=/home/ubuntu/hola.txt state=present" tutorial

# Comando para eliminar un archivo en el servidor remoto
ansible -m file -a "path=/home/ubuntu/hola.txt state=absent" tutorial