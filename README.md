# Robô de Automatização da Importação de Dados do Excel para o SQL Server

## Descrição

Este projeto implementa um robô que automatiza a importação de dados de arquivos Excel para uma tabela específica em um banco de dados SQL Server. O robô é projetado para operar em horários determinados, realizando a carga de dados e, em seguida, entrando em um período de descanso antes de retomar suas atividades. Essa abordagem otimiza o processo de carga, garantindo que os registros sejam processados e inseridos com precisão. Além disso, o robô lida eficientemente com dados nulos e garante a conformidade dos tipos de dados, facilitando a manutenção e a integridade do banco de dados.

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

- **robot.ipynb**: Este é o script principal que realiza a leitura dos arquivos Excel, o processamento dos dados e a inserção no banco de dados SQL Server. O código está bem comentado, facilitando a compreensão das etapas do processo, detalham a lógica utilizada e as decisões tomadas em cada etapa.

- **config.txt**: Arquivo da configuração do SQL Server.

- **README.md**: Este arquivo contém a documentação do projeto.

## Conclusão

A estrutura organizada deste projeto não apenas facilita a manutenção e a navegação pelo código, mas também promove a colaboração eficaz entre os desenvolvedores. Com uma documentação clara e comentários informativos no código, os novos contribuidores podem se integrar rapidamente ao trabalho em equipe. O robô de automatização proporciona uma solução eficiente para a carga de dados, garantindo integridade e confiabilidade no processamento de informações, o que é crucial para a operação de um banco de dados em constante atualização.
