# Docker stacks

## JupyterLab - datascience

```
$ cd jupyter-ds
$ docker build --rm -t youngwookim/my-datascience-notebook .

```

```
docker run --rm --user root -p 8888:8888 -e GRANT_SUDO=yes -e JUPYTER_ENABLE_LAB=yes -v "$PWD":/home/jovyan youngwookim/my-datascience-notebook:latest

```

See more details: https://jupyter-docker-stacks.readthedocs.io/en/latest/

## JupyterLab - spark

```
$ cd jupyter-spark
$ docker build --rm -t youngwookim/my-spark-notebook .

```

```
docker run --rm --user root -p 8888:8888 -e GRANT_SUDO=yes -e JUPYTER_ENABLE_LAB=yes -v "$PWD":/home/jovyan youngwookim/my-spark-notebook:latest

```
