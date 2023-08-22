# dbt_core

### Prerequisites
- Python 3.10 (Version 3.8 or higher is suitable) 
- Spark (Version 3.1.1) Trift Server
- Linux OS (to directly use the commands in)

## Run Spark Thrift Server

[This docker-compose](https://github.com/ElifSinemAktas/dbt_core/blob/main/docker-compose.yaml) starts a Spark Thrift server and a Postgres database as a Hive Metastore backend.

Resource: https://github.com/dbt-labs/dbt-spark

## Create venv 

```shell
python3 -m venv dbt-env
```
```shell
source dbt-env/bin/activate
```

## Install DBT 
```shell
pip install "dbt-spark[PyHive]"
```

Note: sasl installation can be problem when installing the package.
If you are using linux you can follow the steps [here](https://stackoverflow.com/questions/70347149/installing-sasl-in-python).

