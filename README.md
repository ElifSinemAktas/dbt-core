# dbt Core

dbt Core is a popular open-source command-line tool that's used for orchestrating and managing the transformation and modeling of data in your data warehouse. It's particularly well-suited for data analytics teams that work with SQL-based transformations in data warehousing environments. Here are some reasons why you might consider using DBT in your data workflows:

- Modularity and Reusability
- Version Control
- Code Reviws and Collaboration
- Data Testing
- Incremental Processing
- Easy Deployment
- Documentation
- Data Lineage
- Elastic Compute Scaling
- Community and Ecosystem

## 1. Prerequisites
- Python 3.10 (Version 3.8 or higher is suitable) 
- Spark (Version 3.1.1) Trift Server
- Linux OS (to directly use the commands in)

## 2. Steps

- Install DBT
- Create Spark Trift Server using Docker
- 
- 

## 2.1 Run Spark Thrift Server

[This docker-compose](https://github.com/ElifSinemAktas/dbt_core/blob/main/docker-compose.yaml) starts a Spark Thrift server and a Postgres database as a Hive Metastore backend.

Resource: https://github.com/dbt-labs/dbt-spark

## 2.2 Create venv 

```shell
python3 -m venv dbt-env
```
```shell
source dbt-env/bin/activate
```

## 2.3 Install DBT 
```shell
pip install "dbt-spark[PyHive]"
```

Note: sasl installation can be problem when installing the package.
If you are using linux you can follow the steps [here](https://stackoverflow.com/questions/70347149/installing-sasl-in-python).

