# Projeto de Portfólio — AI Engineering

## Objetivo

Construir um projeto integrado que demonstre, em uma aplicação real, as principais competências exigidas para uma primeira vaga de AI Engineer Junior.

O projeto deverá ser tecnicamente compreensível, executável, testável e apresentável em processos seletivos.

O objetivo não é utilizar o maior número possível de tecnologias.

Cada componente deverá existir porque resolve uma necessidade real do problema escolhido.

---

# Princípios do projeto

O projeto deverá:

- resolver um problema claramente definido;
- possuir um usuário ou cenário de uso identificável;
- utilizar IA como parte necessária da solução;
- possuir backend estruturado;
- trabalhar com dados persistentes quando necessário;
- possuir testes;
- ser versionado com Git;
- possuir documentação clara;
- ser executável de forma reproduzível;
- possuir uma versão disponibilizada ou demonstrável;
- permitir explicar as principais decisões técnicas.

O projeto não deverá ser apenas:

- um chatbot genérico;
- uma cópia de tutorial;
- uma interface para enviar prompts a uma API;
- uma coleção de tecnologias sem integração coerente;
- uma aplicação cuja arquitetura eu não consiga explicar.

---

# Competências que o projeto deve demonstrar

## 01. Python e engenharia de software

- [ ] Código organizado em módulos
- [ ] Funções com responsabilidades claras
- [ ] Tratamento de exceptions
- [ ] Configuração separada do código
- [ ] Dependências definidas
- [ ] Estrutura compreensível
- [ ] Refatoração quando necessária

---

## 02. Git e GitHub

- [ ] Histórico de commits compreensível
- [ ] Uso adequado de `.gitignore`
- [ ] Ausência de secrets versionados
- [ ] README profissional
- [ ] Processo de desenvolvimento visível
- [ ] Repositório executável a partir das instruções documentadas

---

## 03. API e backend

- [ ] Backend utilizando FastAPI
- [ ] Endpoints com responsabilidades claras
- [ ] Validação de entrada
- [ ] Modelos de dados
- [ ] Status codes adequados
- [ ] Tratamento de erros
- [ ] Documentação da API

---

## 04. Dados e persistência

Quando aplicável:

- [ ] Banco de dados
- [ ] Modelagem adequada ao problema
- [ ] Operações CRUD necessárias
- [ ] Consultas parametrizadas
- [ ] Separação entre acesso a dados e regras da aplicação
- [ ] Credenciais configuradas de forma segura

---

## 05. Integração com LLM

- [ ] Integração com um modelo de linguagem
- [ ] Prompt Engineering justificável
- [ ] Context Engineering
- [ ] Structured Outputs quando apropriado
- [ ] Validação da saída utilizada pelo software
- [ ] Tratamento de falhas da API
- [ ] Consideração de custo e latência
- [ ] Casos básicos de avaliação

---

## 06. Retrieval e RAG

Se o problema escolhido justificar RAG:

- [ ] Pipeline de ingestão
- [ ] Chunking
- [ ] Metadata
- [ ] Embeddings
- [ ] Armazenamento vetorial
- [ ] Retrieval
- [ ] Construção de contexto
- [ ] Respostas fundamentadas
- [ ] Rastreabilidade das fontes
- [ ] Avaliação de retrieval
- [ ] Avaliação da resposta final

RAG deverá ser utilizado somente quando houver uma necessidade real de recuperar conhecimento externo.

---

## 07. Tools, workflows e agentes

Se o problema escolhido exigir ações ou múltiplas etapas:

- [ ] Tool Calling
- [ ] Validação dos argumentos das ferramentas
- [ ] Tratamento de falhas
- [ ] Workflow explícito
- [ ] Estado quando necessário
- [ ] Limites de execução
- [ ] Observabilidade das ações

Um agente somente deverá ser utilizado quando oferecer vantagem real sobre um workflow determinístico.

---

## 08. Testes e avaliação

- [ ] Testes automatizados para componentes importantes
- [ ] Casos de erro
- [ ] Testes da API
- [ ] Casos reproduzíveis para funcionalidades de IA
- [ ] Critérios de qualidade definidos
- [ ] Registro de falhas relevantes
- [ ] Evidências de melhorias realizadas após avaliação

---

## 09. Entrega

- [ ] Dockerfile
- [ ] Aplicação executável em container
- [ ] Docker Compose quando necessário
- [ ] Variáveis de ambiente
- [ ] Health check
- [ ] Logs úteis
- [ ] Pipeline de CI
- [ ] Testes executados automaticamente
- [ ] Deploy funcional ou demonstração reproduzível

---

## 10. Segurança básica

- [ ] Secrets não expostos
- [ ] Entradas validadas
- [ ] Erros tratados sem exposição desnecessária de detalhes internos
- [ ] Operações sensíveis limitadas
- [ ] Riscos básicos de Prompt Injection considerados quando aplicável
- [ ] Conteúdo externo tratado como potencialmente não confiável

---

# Arquitetura

Antes da implementação completa, deverá existir uma representação simples da arquitetura.

Exemplo conceitual:

```text
Cliente
   ↓
FastAPI
   ↓
Camada de aplicação
   ├── Banco de dados
   ├── LLM
   ├── Retrieval / RAG
   └── Tools
          ↓
Serviços externos
```

A arquitetura final dependerá do problema escolhido.

Tecnologias não deverão ser adicionadas apenas para preencher este diagrama.

---

# README do projeto

O repositório final deverá possuir documentação suficiente para que outra pessoa consiga entender o projeto sem precisar ler todo o código.

O README deverá explicar:

- problema;
- solução;
- principais funcionalidades;
- arquitetura;
- stack;
- decisões técnicas relevantes;
- como executar;
- configuração necessária;
- testes;
- limitações conhecidas;
- possíveis melhorias;
- demonstração do funcionamento.

---

# Demonstração para recrutadores

Em poucos minutos, devo conseguir demonstrar:

1. qual problema o projeto resolve;
2. como a aplicação funciona;
3. onde a IA participa da solução;
4. como os dados percorrem o sistema;
5. uma decisão técnica importante;
6. como a aplicação foi testada;
7. uma limitação conhecida;
8. uma melhoria que eu faria em uma próxima versão.

---

# Defesa técnica

Sem consultar documentação ou utilizar assistência de IA, devo conseguir responder perguntas como:

- Por que esse problema precisa de IA?
- Por que escolhi essa arquitetura?
- Por que escolhi esse modelo?
- Como os dados percorrem o sistema?
- Como a aplicação lida com uma resposta inválida do LLM?
- Onde o sistema pode falhar?
- Como eu investigaria uma falha?
- Como sei se a funcionalidade de IA está funcionando bem?
- Por que utilizei ou não utilizei RAG?
- Por que utilizei ou não utilizei um agente?
- Como protejo as credenciais?
- Como os testes são executados?
- Como a aplicação é disponibilizada?

Não é necessário memorizar detalhes irrelevantes.

O objetivo é demonstrar compreensão das decisões fundamentais do próprio projeto.

---

# Critério de conclusão

O projeto somente será considerado concluído quando:

- [ ] Resolver o problema proposto
- [ ] Possuir arquitetura compreensível
- [ ] Possuir código organizado
- [ ] Possuir testes
- [ ] Possuir avaliação das funcionalidades de IA
- [ ] Possuir documentação
- [ ] Ser reproduzível
- [ ] Ser demonstrável
- [ ] Possuir histórico Git adequado
- [ ] Não expuser secrets
- [ ] Eu conseguir explicar as principais decisões sem assistência
- [ ] Eu conseguir diagnosticar cenários básicos de falha

---

## Resultado esperado

Ao concluir o projeto, devo possuir uma evidência concreta e pública de que consigo integrar conhecimentos de programação, backend, dados, LLMs e práticas de engenharia para construir uma aplicação de IA.

O projeto será uma das principais evidências técnicas utilizadas durante candidaturas e entrevistas para vagas de AI Engineer Junior.