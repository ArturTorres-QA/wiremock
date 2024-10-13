_Estudo_
# wiremock
- [Instalar java](https://www.java.com/pt-BR/download/manual.jsp)
- [Instalar java SE Kit 11 ou superior](https://www.oracle.com/br/java/technologies/javase/jdk11-archive-downloads.html)
- [Instalando wiremock no windows](https://wiremock.org)
- Crie uma pasta, mova o arquivo do wiremock
- Acesse o vsCode e navegue até a pasta onde o wiremock foi adicionado 
   - Abra o terminal do vsCode
      - Comando para executar: `-jar wiremock-standalone-3.9.1.jar`
  
# Projeto de mock
Nesse projeto, possui um exemplo de API de jogos.
- Listagem de jogos, com nome, modelo e ano de lançamento.


## O que está sendo validado:
*GET*
#### Listar jogos: 
- Url: localhost8080/api/games

*POST*
#### Cadastrar novos jogos:
- Url: localhost8080/api/games
  - Cadastrar jogos: Se o cadastro de jogo for igual ao name  "god of war" no parâmetro "name". = O mock tem que responder 201
#### Cadastrar novos jogos - Inválido (erro 500):
- Url: localhost8080/api/games
  - Cadastro jogo invalido: Se o cadastro do jogo for igual a um "shin megami tensei" no parâmetro "name" = O mock tem que responder 500
