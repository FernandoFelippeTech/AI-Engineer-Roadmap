# Fase 05 — Dados e SQL

## Objetivo

Desenvolver as competências de dados e persistência necessárias para aplicações de AI Engineering.

Ao concluir esta fase, devo conseguir modelar dados relacionais simples, consultar e modificar informações utilizando SQL e integrar uma aplicação Python/FastAPI com PostgreSQL.

O foco não é administração avançada de bancos de dados, mas a autonomia necessária para construir aplicações que armazenam, consultam e manipulam dados de forma confiável.

---

# Módulos

## 01. Fundamentos de bancos de dados

**Status:** ⬜ Não iniciado

### Competências

- [ ] Entender por que aplicações utilizam bancos de dados
- [ ] Diferenciar persistência em memória, arquivos e banco de dados
- [ ] Entender o conceito de banco de dados relacional
- [ ] Entender tabelas, linhas e colunas
- [ ] Entender tipos básicos de dados
- [ ] Entender chave primária
- [ ] Entender chave estrangeira
- [ ] Identificar relacionamentos simples entre entidades
- [ ] Entender o papel de um sistema gerenciador de banco de dados

---

## 02. SQL — consultas básicas

**Status:** ⬜ Não iniciado

### Competências

- [ ] Entender a finalidade do SQL
- [ ] Utilizar `SELECT`
- [ ] Selecionar colunas específicas
- [ ] Utilizar `WHERE`
- [ ] Trabalhar com operadores de comparação
- [ ] Combinar condições
- [ ] Utilizar `ORDER BY`
- [ ] Utilizar `LIMIT`
- [ ] Consultar dados sem modificar o banco
- [ ] Ler e explicar uma consulta SQL simples

---

## 03. Inserção, atualização e remoção de dados

**Status:** ⬜ Não iniciado

### Competências

- [ ] Utilizar `INSERT`
- [ ] Utilizar `UPDATE`
- [ ] Utilizar `DELETE`
- [ ] Entender o conceito de CRUD
- [ ] Relacionar CRUD com operações SQL
- [ ] Utilizar condições corretamente em alterações
- [ ] Evitar atualizações ou exclusões acidentais em massa
- [ ] Verificar o resultado de uma alteração

---

## 04. Modelagem relacional básica

**Status:** ⬜ Não iniciado

### Competências

- [ ] Transformar entidades simples em tabelas
- [ ] Escolher tipos de dados adequados
- [ ] Definir chaves primárias
- [ ] Definir chaves estrangeiras
- [ ] Representar relacionamentos um-para-muitos
- [ ] Entender relacionamentos muitos-para-muitos em nível básico
- [ ] Evitar duplicação evidente de dados
- [ ] Explicar as decisões básicas de um modelo

---

## 05. JOINs

**Status:** ⬜ Não iniciado

### Competências

- [ ] Entender por que dados relacionados podem estar em tabelas diferentes
- [ ] Utilizar `INNER JOIN`
- [ ] Utilizar `LEFT JOIN`
- [ ] Relacionar tabelas por chaves
- [ ] Selecionar dados provenientes de múltiplas tabelas
- [ ] Identificar resultados inesperados causados por um JOIN incorreto
- [ ] Ler e explicar uma consulta utilizando JOIN

---

## 06. Agregações e agrupamentos

**Status:** ⬜ Não iniciado

### Competências

- [ ] Utilizar `COUNT`
- [ ] Utilizar `SUM`
- [ ] Utilizar `AVG`
- [ ] Utilizar `MIN` e `MAX`
- [ ] Utilizar `GROUP BY`
- [ ] Utilizar `HAVING` em situações básicas
- [ ] Produzir resumos simples a partir dos dados
- [ ] Interpretar corretamente o resultado de uma agregação

---

## 07. PostgreSQL

**Status:** ⬜ Não iniciado

### Competências

- [ ] Entender o papel do PostgreSQL
- [ ] Criar um banco de dados para desenvolvimento
- [ ] Criar tabelas
- [ ] Definir constraints básicas
- [ ] Inserir e consultar dados
- [ ] Trabalhar com relacionamentos
- [ ] Conectar-se ao banco a partir de uma aplicação
- [ ] Utilizar credenciais por variáveis de ambiente
- [ ] Investigar erros básicos de conexão e consultas

---

## 08. Python e banco de dados

**Status:** ⬜ Não iniciado

### Competências

- [ ] Conectar uma aplicação Python ao PostgreSQL
- [ ] Executar consultas a partir do Python
- [ ] Enviar parâmetros de forma segura
- [ ] Evitar construir SQL inseguro por concatenação de strings
- [ ] Converter resultados do banco em estruturas utilizadas pela aplicação
- [ ] Tratar erros básicos de banco de dados
- [ ] Separar acesso a dados da lógica principal quando apropriado

---

## 09. FastAPI e persistência

**Status:** ⬜ Não iniciado

### Competências

- [ ] Persistir dados recebidos por uma API
- [ ] Consultar dados por endpoints
- [ ] Atualizar registros por meio da API
- [ ] Remover registros por meio da API
- [ ] Validar dados antes da persistência
- [ ] Retornar erros adequados quando um recurso não existir
- [ ] Separar modelos da API e persistência quando necessário
- [ ] Manter credenciais fora do código

---

## 10. Integridade, segurança e boas práticas básicas

**Status:** ⬜ Não iniciado

### Competências

- [ ] Entender o propósito de constraints
- [ ] Utilizar `NOT NULL` quando apropriado
- [ ] Entender `UNIQUE`
- [ ] Entender integridade referencial
- [ ] Entender o risco de SQL Injection
- [ ] Utilizar consultas parametrizadas
- [ ] Não armazenar credenciais diretamente no código
- [ ] Entender o princípio de menor privilégio em nível introdutório
- [ ] Diferenciar dados públicos de dados que exigem proteção

---

## 11. Pandas essencial

**Status:** ⬜ Não iniciado

### Competências

- [ ] Entender quando Pandas é útil
- [ ] Criar e interpretar um `DataFrame`
- [ ] Carregar dados tabulares
- [ ] Selecionar colunas e linhas
- [ ] Filtrar dados
- [ ] Identificar valores ausentes
- [ ] Realizar transformações simples
- [ ] Gerar agregações básicas
- [ ] Evitar utilizar Pandas quando estruturas Python ou SQL forem suficientes

---

# Checkpoint da Fase 05

A fase será concluída somente quando eu conseguir:

- [ ] Modelar um pequeno conjunto de dados relacionais
- [ ] Criar tabelas no PostgreSQL
- [ ] Executar operações CRUD com SQL
- [ ] Escrever consultas utilizando filtros
- [ ] Utilizar JOINs
- [ ] Utilizar agregações
- [ ] Conectar Python ao PostgreSQL
- [ ] Integrar FastAPI com persistência
- [ ] Utilizar consultas parametrizadas
- [ ] Investigar erros básicos relacionados ao banco
- [ ] Explicar o caminho dos dados da API até o banco e de volta ao cliente

---

# Projeto 03 — API + FastAPI + PostgreSQL

Após validar as competências necessárias, será desenvolvido um backend completo integrando as fases anteriores.

O projeto deverá incluir:

- API REST com FastAPI;
- validação de entrada e saída;
- PostgreSQL;
- operações CRUD;
- relacionamentos entre dados;
- consultas utilizando filtros;
- pelo menos um JOIN relevante;
- tratamento de erros;
- configuração por variáveis de ambiente;
- testes automatizados;
- documentação para execução do projeto;
- versionamento com Git e GitHub.

O projeto deverá ser desenvolvido com estrutura suficiente para que outra pessoa consiga clonar o repositório, configurar o ambiente e executar a aplicação.

---

## Resultado esperado

Ao concluir esta fase, devo conseguir desenvolver uma aplicação backend que recebe dados por uma API, aplica regras básicas, persiste informações em PostgreSQL e retorna resultados de forma estruturada.

Também devo conseguir consultar e investigar os dados diretamente utilizando SQL.

Essa base permitirá que as próximas aplicações de AI Engineering possuam persistência real, em vez de funcionarem apenas como demonstrações isoladas.