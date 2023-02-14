# docker + python

----
# Creamos un  contenedor sencillo de python:
 ```docker run -it --rm -v "$PWD":/usr/src/myapp -w /usr/src/myapp python:3 python your-daemon-or-script.py```

 `docker:` comando base
 `run:` crea el contenedor
 `it:` son dos opciones que me valen para interactuar(i) y para que esa interacción sea a través de una terminal(t)
 `rm` borra el contenedor cuando finaliza la acción
 `v` define el mapeo del volúmen que está a continuación
 `$PWD` el directorio donde estamos
 `/usr/src/myapp` el directorio dentro del contenedor
 `w` es el directorio de trabajo "workdir"
 
`python:3` Es la imagen de la que se creará el contenedor

 `python script.py` es el comando para ejecutar dentro del contenedor