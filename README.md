### API desenvolvida utilizando a arquitetura DDD
<div align="center" , dis>
<img width="900px" src="./img/doc.png">
    <h1 align="center">
        DDDs
    </h1>
</div>

# Preparando o ambiente
!!! Para executar os comandos abaixo é priciso ter o docker instalado, caso tenho o postgres instalado pode pular esses passos.
## Criando container do banco postgres no docker
### escolhi a porta 5433, você pode optar por outra
``` docker run --name postgres -e POSTGRES_PASSWORD=SUA_SENHA -p 5433:5432 -d postgres:11 ```
### rodando o container do postgres
```  docker start postgres ```


## Banco de dados
<p> Crie um banco de dados com o nome 'aftersale' e altere suas credenciais no arquivo 'ormconfig.json' </p>

## Criando o Banco de dados
``` yarn typeorm migrations:run ```

# TESTES
``` yarn test ```
``` yarn test:watch ```
``` yarn test:verbose ```
``` yarn test:staged ```
``` yarn test:ci ```

# Rodando nossa API
Antes de executar esse comando verifique se seu banco de dados está rodando
``` yarn dev:server ``` 

# Documentação 
 acesse: http://localhost:3333/api-docs/#/ 