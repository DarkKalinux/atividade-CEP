# atividade-CEP
atividade dia 11/03/24 5° Período
# Projeto de Consulta de Endereço por CEP

## Objetivo
Este projeto tem como objetivo implementar um sistema que consulta informações de endereço a partir de um CEP fornecido pelo usuário. O sistema verifica se o CEP já foi consultado anteriormente, utilizando um banco de dados para armazenar as informações de forma persistente. Caso o CEP não tenha sido consultado, o sistema faz a consulta à API ViaCEP e salva os dados para futuras consultas, otimizando o tempo de resposta em buscas subsequentes.

## Fluxo do Programa
1. O sistema solicita um CEP ao usuário.
2. Verifica no banco de dados se o CEP já foi consultado anteriormente.
3. Se o CEP existir no banco de dados, exibe as informações para o usuário.
4. Se o CEP não existir no banco de dados, busca os dados na API ViaCEP.
5. Os dados do endereço e a data/hora da consulta são salvos no banco de dados.
6. O sistema informa ao usuário que a busca foi realizada via API e que os dados foram armazenados para futuras consultas.

## Tecnologias Utilizadas
- **Java 21**: Linguagem de programação utilizada para desenvolver o sistema.
- **Hibernate ORM**: Framework de mapeamento objeto-relacional para interagir com o banco de dados.
- **PostgreSQL**: Banco de dados relacional utilizado para persistir as informações dos endereços.
- **ViaCEP API**: API externa utilizada para consultar as informações de endereço a partir do CEP.
- **Jakarta EE**: Conjunto de especificações para construir aplicações empresariais em Java.
- **Maven**: Ferramenta de automação de builds para gerenciar dependências e construir o projeto.
- **JUnit 5**: Framework de testes unitários utilizado para garantir a qualidade do código.

## Como Executar o Projeto

### 1. Clonar o Repositório
Primeiro, clone o repositório para o seu ambiente local:

```bash
git clone https://github.com/SEU_USUARIO/AtividadeCEP.git
cd AtividadeCEP
