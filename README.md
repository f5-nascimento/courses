# Implementação de Banco de Dados PostgreSQL na Nuvem

## Contextualização
Uma equipe de desenvolvimento de software precisa implementar uma solução de banco de dados na nuvem para atender às necessidades de um projeto corporativo.  
A escolha da empresa foi utilizar o serviço **Render** para hospedar um banco **PostgreSQL**, que permitirá maior escalabilidade, segurança e facilidade de integração com outras ferramentas.

Neste cenário, o time deve estruturar a base de dados, aplicar boas práticas de modelagem, realizar inserções em massa e configurar permissões de acesso, garantindo que a solução seja funcional e segura.

---

## Desafio
Como parte da equipe de desenvolvimento, você deverá implementar e configurar um banco de dados PostgreSQL na nuvem no **Render**, além de executar tarefas de manipulação de dados e controle de usuários.

As etapas do desafio incluem:

---

### 1. Criação do Banco de Dados
- Criar um banco chamado **tools-seunome**, onde `seunome` é substituído pelo nome do aluno.
- Conectar o banco ao **DBeaver** para gerenciar e executar os scripts.

---

### 2. Criação da Tabela `cursos`
Criar uma tabela chamada **cursos** com os seguintes campos:
- id INT, codigo VARCHAR(18), nome VARCHAR(45), modalidade VARCHAR(45), area VARCHAR(45), coordenador VARCHAR(45), campus CHAR(2)
- Todos os campos devem ser **NOT NULL**.  
- O campo **id** deve ser a **chave primária**.  
- Os campos devem seguir o padrão **nomedocampo_nomedatabela** (ex.: `id_curso`).

---

### 3. Manipulação de Dados
- Criar um **INSERT** com **155 registros** (os dados podem ser gerados com auxílio de uma IA generativa).  
- Atualizar o campo `campus_curso` de todos os registros com `id_curso > 100` para **PE**.  
- Excluir todos os registros com `id_curso > 150`.  

---

### 4. Consultas
- Realizar uma consulta que exiba os nomes de todos os cursos cujo `nome_curso` começa com a letra **B**.  
- Criar uma **VIEW** chamada `relatorio` que execute essa consulta.  

---

### 5. Gerenciamento de Usuários
- Criar o usuário **felnascimento** com senha **12345**.  
- Conceder permissão ao usuário **felnascimento** para executar a **view relatorio**.  

---

## Entrega
Os alunos deverão enviar:
1. Os **scripts SQL** de cada ação realizada.  
2. O **host do banco** e o **nome do banco** para validação.  

---

## Resultados Esperados
- Banco de dados **tools-seunome** corretamente criado e acessível pelo Render e DBeaver.  
- Tabela **cursos** criada conforme as especificações, respeitando o padrão de nomenclatura.  
- Inserção em massa de **155 registros** concluída com sucesso.  
- Atualização correta do campo `campus_curso` para registros com `id_curso > 100`.  
- Exclusão de registros com `id_curso > 150` realizada corretamente.  
- Consulta que retorna os cursos cujo nome começa com **B** implementada com sucesso.  
- **View relatorio** criada corretamente a partir da consulta.  
- Usuário **felnascimento** criado com senha definida e permissões de execução atribuídas à view.  
- Scripts, host e nome do banco entregues dentro do prazo estabelecido.  
