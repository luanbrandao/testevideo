### API desenvolvida utilizando a arquitetura DDD


## :wrench: Ferramentas
:large_orange_diamond: Sucrase

:large_orange_diamond: ESLint

:large_orange_diamond: Prettier

:large_orange_diamond: Sequelize


## Banco Dedos
:paperclip: PostgreSQL



<div align="center" , dis>
<img width="900px" src="./img/doc.png">
    <h1 align="center">
        Documentação com Swagger
    </h1>
</div>


## :ballot_box_with_check: Execucanto o projeto
!!! Para executar os comandos abaixo é priciso ter o docker instalado, caso tenho o postgres instalado pode pular esses passos.
</br>
:heavy_check_mark: Criando container do banco postgres no docker
 escolhi a porta 5433, você pode optar por outra
<br>

``` docker run --name postgres -e POSTGRES_PASSWORD=SUA_SENHA -p 5433:5432 -d postgres:11 ```

:heavy_check_mark: rodando o container do postgres
<br>

```  docker start postgres ```


### :ballot_box_with_check: Banco de dados
<p> Crie um banco de dados com o nome 'aftersale' e altere suas credenciais no arquivo 'ormconfig.json' </p>

## Criando o Banco de dados
``` yarn typeorm migrations:run ```

## :ballot_box_with_check: TESTES
``` yarn test ```
``` yarn test:watch ```
``` yarn test:verbose ```
``` yarn test:staged ```
``` yarn test:ci ```

## :ballot_box_with_check: Rodando nossa API
Antes de executar esse comando verifique se seu banco de dados está rodando
``` yarn dev:server ``` 

## :ballot_box_with_check: Documentação 
 acesse: http://localhost:3333/api-docs/#/ 