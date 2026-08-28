# Fase 04 — APIs e Backend

## Objetivo

Aprender como aplicações se comunicam pela web e desenvolver APIs em Python utilizando FastAPI.

Ao concluir esta fase, devo conseguir consumir APIs externas, compreender requisições e respostas HTTP e construir uma API REST com validação de dados, tratamento de erros e organização adequada.

Essas competências serão fundamentais posteriormente para integrar aplicações com LLMs, bancos de dados, ferramentas e serviços externos.

---

# Módulos

## 01. Cliente, servidor e comunicação web

**Status:** ⬜ Não iniciado

### Competências

- [ ] Entender o modelo cliente-servidor
- [ ] Entender o que acontece quando uma aplicação faz uma requisição
- [ ] Diferenciar cliente e servidor
- [ ] Entender o papel básico de uma URL
- [ ] Identificar domínio, caminho e parâmetros em uma URL
- [ ] Entender o conceito de endpoint
- [ ] Entender o papel de uma API na comunicação entre sistemas

---

## 02. HTTP

**Status:** ⬜ Não iniciado

### Competências

- [ ] Entender o modelo request/response
- [ ] Entender métodos HTTP
- [ ] Utilizar `GET`
- [ ] Utilizar `POST`
- [ ] Utilizar `PUT` e `PATCH`
- [ ] Utilizar `DELETE`
- [ ] Entender status codes
- [ ] Interpretar códigos `2xx`, `4xx` e `5xx`
- [ ] Entender headers
- [ ] Entender query parameters
- [ ] Entender path parameters
- [ ] Entender request body
- [ ] Identificar as partes de uma requisição e de uma resposta HTTP

---

## 03. JSON em APIs

**Status:** ⬜ Não iniciado

### Competências

- [ ] Entender por que JSON é utilizado em APIs
- [ ] Ler respostas JSON
- [ ] Enviar dados JSON
- [ ] Converter respostas JSON para estruturas Python
- [ ] Acessar dados aninhados
- [ ] Validar a presença de informações esperadas
- [ ] Tratar respostas incompletas ou inesperadas

---

## 04. REST e design básico de APIs

**Status:** ⬜ Não iniciado

### Competências

- [ ] Entender o conceito de REST
- [ ] Entender o conceito de recurso
- [ ] Relacionar métodos HTTP com operações sobre recursos
- [ ] Criar endpoints compreensíveis
- [ ] Utilizar status codes apropriados
- [ ] Diferenciar path parameters de query parameters
- [ ] Evitar colocar ações desnecessárias nos nomes dos endpoints
- [ ] Entender CRUD no contexto de uma API
- [ ] Ler documentação de uma API REST

---

## 05. Consumindo APIs com Python

**Status:** ⬜ Não iniciado

### Competências

- [ ] Fazer uma requisição HTTP utilizando Python
- [ ] Utilizar uma biblioteca como `requests` ou `httpx`
- [ ] Enviar query parameters
- [ ] Enviar headers
- [ ] Enviar dados JSON
- [ ] Ler status codes
- [ ] Interpretar respostas JSON
- [ ] Tratar falhas de conexão
- [ ] Tratar respostas de erro
- [ ] Definir timeout
- [ ] Consumir uma API externa a partir de sua documentação

---

## 06. Autenticação e secrets

**Status:** ⬜ Não iniciado

### Competências

- [ ] Entender por que APIs utilizam autenticação
- [ ] Entender o conceito de API key
- [ ] Entender tokens em nível introdutório
- [ ] Enviar credenciais por headers quando necessário
- [ ] Utilizar variáveis de ambiente
- [ ] Evitar colocar secrets diretamente no código
- [ ] Evitar versionar credenciais no Git
- [ ] Entender o papel de `.env` em desenvolvimento
- [ ] Utilizar `.gitignore` para proteger arquivos locais sensíveis

---

## 07. FastAPI — fundamentos

**Status:** ⬜ Não iniciado

### Competências

- [ ] Entender o papel de um framework web
- [ ] Criar uma aplicação FastAPI
- [ ] Executar a aplicação localmente
- [ ] Criar endpoints
- [ ] Trabalhar com diferentes métodos HTTP
- [ ] Utilizar path parameters
- [ ] Utilizar query parameters
- [ ] Receber dados no request body
- [ ] Retornar respostas JSON
- [ ] Utilizar a documentação automática da API
- [ ] Testar endpoints durante o desenvolvimento

---

## 08. Validação de dados com Pydantic

**Status:** ⬜ Não iniciado

### Competências

- [ ] Entender por que dados de entrada precisam ser validados
- [ ] Criar modelos de dados
- [ ] Definir tipos esperados
- [ ] Trabalhar com campos obrigatórios e opcionais
- [ ] Interpretar erros de validação
- [ ] Utilizar modelos em endpoints FastAPI
- [ ] Separar modelos de entrada e saída quando necessário
- [ ] Evitar confiar cegamente nos dados enviados pelo cliente

---

## 09. Tratamento de erros em APIs

**Status:** ⬜ Não iniciado

### Competências

- [ ] Identificar diferentes tipos de falha em uma API
- [ ] Retornar status codes adequados
- [ ] Criar mensagens de erro úteis
- [ ] Utilizar `HTTPException`
- [ ] Diferenciar erro do cliente de erro do servidor
- [ ] Evitar expor informações internas desnecessárias
- [ ] Tratar falhas de serviços externos
- [ ] Investigar erros utilizando logs e traceback

---

## 10. Organização básica de backend

**Status:** ⬜ Não iniciado

### Competências

- [ ] Separar endpoints de lógica de negócio quando necessário
- [ ] Organizar código em módulos
- [ ] Evitar concentrar toda a aplicação em um único arquivo
- [ ] Gerenciar configurações por variáveis de ambiente
- [ ] Organizar dependências
- [ ] Criar código reutilizável
- [ ] Manter responsabilidades compreensíveis
- [ ] Documentar como executar a API

---

## 11. Testes básicos de API

**Status:** ⬜ Não iniciado

### Competências

- [ ] Entender o que deve ser testado em um endpoint
- [ ] Testar respostas de sucesso
- [ ] Testar entradas inválidas
- [ ] Testar status codes
- [ ] Testar estrutura básica das respostas
- [ ] Executar testes automaticamente
- [ ] Investigar a causa de um teste de API que falhou

---

# Checkpoint da Fase 04

A fase será concluída somente quando eu conseguir:

- [ ] Explicar cliente, servidor, HTTP e REST
- [ ] Interpretar uma requisição e uma resposta HTTP
- [ ] Consumir uma API externa a partir da documentação
- [ ] Tratar erros durante o consumo de uma API
- [ ] Trabalhar com autenticação sem expor credenciais
- [ ] Construir uma API utilizando FastAPI
- [ ] Validar dados utilizando Pydantic
- [ ] Implementar tratamento adequado de erros
- [ ] Organizar a aplicação em mais de um módulo quando necessário
- [ ] Criar testes básicos para endpoints
- [ ] Explicar o fluxo completo de uma requisição dentro da própria aplicação

---

# Aplicação prática da fase

Durante esta fase será construída uma API progressivamente.

Ela deverá incluir:

- múltiplos endpoints;
- diferentes métodos HTTP;
- path e query parameters;
- entrada e saída em JSON;
- validação com Pydantic;
- tratamento de erros;
- consumo de pelo menos um serviço externo;
- configuração por variáveis de ambiente;
- testes automatizados básicos.

A aplicação será utilizada como preparação para o projeto que integrará backend e banco de dados na fase seguinte.

---

## Resultado esperado

Ao concluir esta fase, devo conseguir ler a documentação de uma API, integrá-la a uma aplicação Python e desenvolver meu próprio backend utilizando FastAPI.

Também devo conseguir explicar como os dados percorrem o caminho entre cliente, API, lógica da aplicação e serviços externos.

Essa base será reutilizada posteriormente para construir APIs que exponham funcionalidades de LLMs, RAG e agentes.