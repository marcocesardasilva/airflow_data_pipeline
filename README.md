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

Criando e acessando a parta para instalação:
```
mkdir airflow
cd airflow
```

Criando variável de ambiente que aponta para a pasta onde do Airflow:
```
export AIRFLOW_HOME=$~/airflow
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
airflow webserver --port 8080
```

Iniciando o serviço Scheduler:
```
airflow scheduler
```

Criar usuário do airflow:
```
airflow users create \
	--username admin \
	--firstname FIRST_NAME \
	--lastname LAST_NAME \
	--role Admin \
	--email marcocesardasilva@gmail.com
```


