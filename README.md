# Bases de Datos: Infraestructura

Este repositorio contiene el listado de software y las plantillas de Docker utilizadas para los cursos de la disciplina de Sistemas de Información

## Instaladores

#### Sistemas Gestores de Bases de Datos

- **MySQL** (SQL) [[Instalador](https://dev.mysql.com/downloads/installer/)] [[Tutorial](https://www.youtube.com/watch?v=u96rVINbAUI)]
- **PostgreSQL** (SQL) [[Instalador](https://www.postgresql.org/download/)] [[Tutorial](https://www.youtube.com/watch?v=uN0AfifH1TA&t=40s)]
- **MonetDB** (Multidimensional | Columnar) [[Instalador](https://www.monetdb.org/easy-setup/)] [[Tutorial](https://www.youtube.com/watch?v=G9vqMxhRr04&list=PLAATrwEHac5jMc-5FU_bkPn8RUBOKCoQp)
- **DuckDB** (Multidimensional | Columnar) [[Instalador](https://duckdb.org/docs/installation/?version=stable&environment=cli&platform=win&download_method=package_manager&architecture=x86_64)] [[Tutorial](https://www.youtube.com/watch?v=ZX5FdqzGT1E&t=19s)]
- **Redis** (Llave-valor) [[Instalador](https://redis.io/docs/latest/operate/oss_and_stack/install/install-stack/binaries/)] [[Tutorial](https://redis.io/docs/latest/operate/oss_and_stack/install/install-stack/)] 
- **Etcd** (Llave-valor) [[Instalador](https://github.com/etcd-io/etcd/releases/)] [[Tutorial](https://github.com/etcd-io/etcd/releases/)] 
- **Couchbase** (Documentos) [[Instalador](https://www.couchbase.com/downloads/?family=couchbase-server)] [[Tutorial](https://www.youtube.com/watch?v=ZJP-4jT0Tj8)] 
- **MongoDB** (Documentos) [[Instalador](https://www.mongodb.com/try/download/community)] [[Tutorial](https://www.mongodb.com/docs/manual/installation/)]
- **Neo4J** (Grafos) [[Instalador](https://neo4j.com/deployment-center/)] [[Tutorial](https://www.youtube.com/watch?v=qAFivl3z8jo)]

#### Clientes

- **DBeaver** [[Instalador](https://dbeaver.io/download/)]
- **MongoDB Compass** [[Instalador](https://www.mongodb.com/try/download/compass)]
- **Etcd Manger** [[Instalador](https://etcdmanager.io/)]

## Docker

- Docker Desktop [[Instalador](https://www.docker.com/products/docker-desktop/)] [[Tutorial](https://www.youtube.com/watch?v=ZyBBv1JmnWQ)]
- Jupyter/MySQL (Clases Prácticas)
  - Ir a `docker/lab-notebooks` 
  - Ejecutar `docker compose up`
  - Buscar en el output de la consola la url del servidor de Jupyter y pegarla en el navegador (localhost:8888)


## Jupyter Lab sin Docker

En caso de quere utilizar la configuración de Jupyter sin Docker

1. Instalar MySQL en su SO

   - [Windows](https://dev.mysql.com/doc/refman/8.4/en/windows-installation.html)
   - [MacOS](https://dev.mysql.com/doc/refman/8.4/en/macos-installation.html)
   - [Linux](https://dev.mysql.com/doc/refman/8.4/en/linux-installation.html)

2. Instalar Python

3. Instalar VS Code y la [extensión de Jupyter](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter)

4. Instalar el cliente de MySQL en python:

   - Windows:

     ```
     pip install ipython-sql sqlalchemy==1.4.46 mysqlclient
     ```

   - MacOS:

     ```
     brew install pkg-config
     pip install ipython-sql sqlalchemy==1.4.46 mysqlclient
     ```

   - Linux:

     ```
     sudo apt-get install python3-dev default-libmysqlclient-dev build-essential pkg-config
     pip install ipython-sql sqlalchemy==1.4.46 mysqlclient
     ```

     
