# Projeto para Envio de E-mails com Workers


#### Pasta APP 
````
    - app/app.sh
        Tem como objetivo de instalar as dependencia do python para o projeto
    - app/sender.py
        Aplicação com objetivo se persistirem os e-mails enviados
````

#### Pasta NGINX 
````
    - nginx/default.conf
        Configuração do proxy reverso
````

#### Pasta Scripts 
````
    - scripts/*
        Configuração banco
````

#### Pasta Web 
````
    - web/*
        Aplicação front-end
````

#### Pasta Worker 
````
    - worker/app.sh
        Instalando redis
    - worker/Dockerfile
        Imagens tendo redis instalado redis e python
    - worker/worker.py
        Aplicação com objetivo de enfileirar os envios de emails
````


#### Parando os processos
````
    - docker-compose down
````

#### Criando tabelas 
````
    - docker-compose exec db psql -U postgres -f /scripts/check.sql
````
