# README #

Dockerfile and supporting tools for running Dedalus as a containerized app.

### Contents ###

* Dockerfile
* ddedalus - a script to run dedalus as a contanerized app. 

### using ddedalus ###
```
$ ddedalus --np 4 myscript.py
```
will run dedalus using mpi on 4 cores inside the container. By default, ddedalus will mount the current directory inside the container. You can change that by doing
```
$ ddedalus --np 4 --workdir=/path/to/workdir myscript.py
```
where `/path/to/workdir` will have both the script and the output.