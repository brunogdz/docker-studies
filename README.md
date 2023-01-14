# DevOps com AWS

## Docker

### Comandos

Você acessa o container, nesse exemplo o ubuntu e consegue executar os comandos e até mesmo instalar coisas
```console
bruno@bar:~$ docker run -it ubuntu
root@3434232634231:/#
```

Para sair é só executar o exit
```console
root@3434232634231:/# exit
```

### Comandos para listagem de container
```console
bruno@bar:~$ docker ps 
```

Comando que lista todos
```console
bruno@bar:~$ docker ps -a
```

Executar o container de forma background

```console
bruno@bar:~$ docker run -dti ubuntu
```

Para remover os containers que não estão em uso, primeiro liste os containers:
```console
docker ps -a
CONTAINER ID   IMAGE         COMMAND        CREATED             STATUS                         PORTS     NAMES
0e47a9e2ddd3   ubuntu        "bash"         4 minutes ago       Exited (137) 21 seconds ago              funny_wright
```

E agora você só executar o comando com os 3 primeiros caracteres
```console
docker rm 0e4
```

E para remover as imagens, só executar 
```console
docker images
```

e executar
```console
docker rmi hello-world
```

Para renomear um container é utilizando o comando
```console
docker run -dti --name Ubuntu-B ubuntu
```
