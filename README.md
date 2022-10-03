# Data Pipeline com Airflow

Estudos de pipeline de dados com Airflow, utilizando a API do Twitter.

## Instalando o airflow

Atualizando o sistema:
```
sudo apt update
```

Instalando o Python caso ainda não tenha no sistema:
```
sudo apt install -y python3
```

Instalando o gerenciador de pacotes do Python:
```
sudo apt install -y python3-pip
```

Instalando o virtual environment:
```
sudo apt install python3.10-venv
```

Criando o ambiente virtual em Python para isolar do sistema:
```
mkdir airflow_data_pipeline
cd airflow_data_pipeline
python3 -m venv .env
source .env/bin/activate
```

Criando variável de ambiente que aponta para a pasta onde do Airflow:
```
export AIRFLOW_HOME=$(pwd)/airflow
```

Instalando o Airflow:
```
pip install apache-airflow
```

Iniciando o banco de dados:
```
airflow db init
```

Iniciando o Webserver:
```
airflow webserver
```

Iniciando o serviço Scheduler:
```
airflow scheduler
```




