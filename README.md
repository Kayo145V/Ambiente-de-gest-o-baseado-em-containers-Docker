# Ambiente-de-gest-o-baseado-em-containers-Docker
Criação de um sistema de gestão de funcionários que facilita o gerenciamento de informações com operações CRUD.

# Sistema de Gestão de Funcionários

Este projeto implementa um sistema de gestão de funcionários utilizando PHP, MySQL e Docker. O sistema permite a criação, leitura, atualização e exclusão (CRUD) de registros de funcionários.

# Vídeo de Demonstração

Veja o vídeo de demonstração aqui: 
[https://www.youtube.com/watch?v=Npla4rTT7ak](https://www.youtube.com/watch?v=Npla4rTT7ak)

## Estrutura do Projeto

O projeto é composto pelos seguintes arquivos:

- `config.php`: Arquivo de configuração para conexão com o banco de dados MySQL.
- `create.php`: Página para criar novos registros de funcionários.
- `read.php`: Página para visualizar detalhes de um funcionário específico.
- `update.php`: Página para atualizar as informações de um funcionário.
- `delete.php`: Página para excluir um registro de funcionário.
- `index.php`: Página principal que lista todos os funcionários.
- `error.php`: Página de erro para requisições inválidas.
- `docker-compose.yml`: Arquivo para configurar os contêineres Docker.   (TAMBÉM CONTÉM INFORMAÇÕES EXTRAS COMO LOGIN E SENHA DO BANCO DE DADOS)
- `Dockerfile`: Arquivo para construir a imagem do servidor web.  
- `employees.sql`: Script SQL para criar a tabela de funcionários e inserir dados iniciais.

## employees.sql

O arquivo `employees.sql` contém as instruções SQL necessárias para configurar o banco de dados do sistema de gestão de funcionários. Ele inclui:

1. **Criação da Tabela**: O script cria uma tabela chamada `employees` com as seguintes colunas:
   - `id`: Identificador único do funcionário (chave primária).
   - `name`: Nome do funcionário.
   - `salary`: Salário do funcionário.
   - `address`: Endereço do funcionário.

2. **Inserção de Dados Iniciais**: O script também pode incluir alguns registros de exemplo na tabela `employees`, permitindo que você teste o sistema imediatamente após a configuração do banco de dados.

Para executar o script, você pode usar um cliente MySQL ou uma ferramenta de gerenciamento de banco de dados, como o phpMyAdmin. Basta conectar-se ao seu banco de dados e executar o conteúdo do arquivo `employees.sql`.

## Pré-requisitos

Antes de começar, você precisará instalar algumas ferramentas:

1. **Docker**: 
   - [Docker](https://www.docker.com/get-started) é uma plataforma que permite criar, implantar e executar aplicativos em contêineres. Siga as instruções de instalação no site oficial.

2. **Docker Compose**: 
   - O Docker Compose é uma ferramenta para definir e executar aplicativos Docker com múltiplos contêineres. Ele geralmente é incluído na instalação do Docker, mas você pode verificar a documentação [aqui](https://docs.docker.com/compose/install/) para mais detalhes.

3. **MySQL**: 
   - O MySQL é um sistema de gerenciamento de banco de dados relacional. Embora o projeto utilize Docker para configurar o MySQL, você pode precisar de um cliente MySQL para interagir com o banco de dados. Você pode usar:
     - [MySQL Workbench](https://www.mysql.com/products/workbench/)
     - [phpMyAdmin](https://www.phpmyadmin.net/)
     - Ou qualquer outro cliente de sua preferência.

4. **PHP**: 
   - O PHP é uma linguagem de script do lado do servidor. O projeto já inclui um ambiente PHP configurado no Docker, mas se você quiser executar scripts PHP localmente, você pode instalar o PHP seguindo as instruções [aqui](https://www.php.net/manual/pt_BR/install.php).

## Instalação

1. Clone este repositório:
   ```bash
   git clone <URL do repositório>
   cd <nome do diretório>
   
2. Execute o comando a seguir para iniciar os contêineres:
   ```bash
   docker-compose up -d

3. Para configurar o banco de dados, você pode executar o script employees.sql no seu banco de dados MySQL. Este script cria a tabela de funcionários e insere alguns dados iniciais.
  

## Acesso ao sistema

Acesse o sistema através do navegador no endereço http://localhost:8080.

Informações extras como login e senha estão disponíveis no arquivo DOCKER-COMPOSE.YML
----------------------------------------------------------------------------------------------------------------------------

# Em caso de dúvidas entre em contato com: Kayo145v@gmail.com
