# Getting started with docker and simple app Django

All documentation to install Docker: 

  - https://docs.docker.com/engine/installation/
  

> Generaly in projects that will be in production we build our own image, but
> here is a simple demo so, I'm abstracting this step.


Building image: 
```sh
$ docker build -t demo_app .
```
> The argument `-t` means `tag` the name of our image.

Running:

```sh
$ docker run -it -p 8080:8080  demo_app
``` 
> About arguments: `-i` means `--interactive` keep stdin open even if not attached.
>  `-t` allocate a pseudo-tty, this will allow you to see the container running as 
> your bash prompt was running.
> The argument `-p` publish a port from container to one port in the machine running the container.   

Acess your:

[localhost] - localhost:8080



[localhost]: <localhost:8080>
