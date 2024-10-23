# Automatização da Importação de Dados do Excel para SQL Server

## Descrição

Este projeto automatiza a importação de dados de arquivos Excel para uma tabela específica em um banco de dados SQL Server. O objetivo é facilitar a carga de dados, garantindo que os registros sejam processados e inseridos corretamente, enquanto lida com dados nulos e tipos de dados.

## Funcionalidades

- Execução programada do robô com controle de horários.
- Tratamento de erros com mensagens informativas.
- Armazenamento seguro de senhas por meio de criptografia.
- Leitura de arquivos Excel (.xlsx).
- Remoção de registros nulos em colunas obrigatórias.
- Conversão de tipos de dados (datas e numéricos).
- Inserção de registros em tabelas SQL Server.
- Movimentação de arquivos processados para uma pasta separada.

## Pré-requisitos

- Python 3.x
- Bibliotecas:
  - `os`
  - `cryptography.fernet`
  - `pyodbc`
  - `pandas`
  - `shutil`
  - `time`
  - `sqlalchemy`
- SQL Server configurado e acessível

# Estrutura do Projeto

A estrutura do projeto foi organizada de forma a facilitar a navegação e a manutenção. Abaixo está uma visão geral dos diretórios e arquivos principais:

- **robot.py**: Este é o script principal que realiza a leitura dos arquivos Excel, o processamento dos dados e a inserção no banco de dados SQL Server. O código está bem comentado, facilitando a compreensão das etapas do processo, detalham a lógica utilizada e as decisões tomadas em cada etapa.

- **config.txt**: Arquivo da configuração do SQL Server.

- **README.md**: Este arquivo contém a documentação do projeto.

## Conclusão

Esta estrutura permite uma melhor organização e manutenção do código, facilitando a colaboração entre os desenvolvedores e o acompanhamento do progresso do projeto.
