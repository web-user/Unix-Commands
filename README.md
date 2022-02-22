# Unix-Commands
Unix Commands

## Conda run 

```sh
$ curl https://repo.anaconda.com/archive/Anaconda3-2021.11-Linux-x86_64.sh --output anaconda.sh
$ ha256sum anaconda.sh
$ sha256sum anaconda.sh
$ bash anaconda.sh\n
$ source ~/.bashrc
$ conda create -n proj_env python=3.6
$ conda activate proj_env
$ conda deactivate
$ pip install -r requirements.txt

```

## Docker run 

```sh
$ docker logs -f <container_name>
$ docker exec -it <container_name> bash
$ docker exec -t <container_name> pg_dumpall -U user_name > dump_local_`date +%d-%m-%Y"_"%H_%M_%S`.sql
$ cat dump_03-02-2022_10_59_55.sql | docker exec -i <container_name> psql -U test -d test

```