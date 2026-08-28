# AI Engineer Roadmap

## Objetivo

Este roadmap define uma trilha prática e progressiva de preparação para uma primeira oportunidade profissional como **AI Engineer Junior**.

A estrutura foi organizada a partir das competências observadas em vagas de entrada da área e das dependências técnicas necessárias para desenvolvê-las de forma consistente.

O objetivo não é estudar toda a área de Inteligência Artificial.

O objetivo é atingir um nível em que eu consiga:

- desenvolver aplicações de IA;
- integrar LLMs a sistemas reais;
- construir APIs e trabalhar com dados;
- implementar busca semântica e RAG;
- utilizar ferramentas e workflows com LLMs;
- aplicar práticas básicas de engenharia e produção;
- demonstrar essas competências por meio de projetos;
- explicar e defender decisões técnicas em entrevistas.

---

# Princípio do roadmap

A progressão segue três movimentos:

```text
Fundamentos
    ↓
Construção de sistemas
    ↓
Integração com IA
    ↓
Entrega e demonstração profissional
```

Cada fase possui competências verificáveis.

Estudar um conteúdo não significa automaticamente dominá-lo.

Uma competência somente deverá ser considerada validada quando puder ser demonstrada por exercícios, debugging, projetos, explicação técnica ou avaliação.

---

# Trilha

## 00 — Diagnóstico

Identificação do nível inicial, conhecimentos existentes e lacunas técnicas.

O diagnóstico serve como referência para adaptar os estudos e comparar evolução posteriormente.

---

## 01 — Fundamentos de Programação

Base de lógica necessária para todo o restante da trilha.

Principais temas:

- variáveis e tipos;
- operadores;
- condicionais;
- loops;
- funções;
- estruturas de dados;
- erros;
- resolução de problemas;
- debugging.

### Entrega

**Projeto 01 — Python e Lógica**

---

## 02 — Python Aplicado

Transformação da lógica de programação em código Python organizado e reutilizável.

Principais temas:

- Python aplicado;
- módulos;
- arquivos;
- JSON;
- exceptions;
- ambientes virtuais;
- dependências;
- OOP essencial;
- debugging;
- refatoração.

### Entrega

**Projeto 02 — Aplicação Python Estruturada**

---

## 03 — Ferramentas de Engenharia

Introdução ao fluxo profissional de desenvolvimento de software.

Principais temas:

- terminal;
- Git;
- GitHub;
- branches;
- merge;
- conflitos;
- documentação;
- testes;
- fluxo de desenvolvimento.

---

## 04 — APIs e Backend

Construção da base necessária para integrar aplicações, modelos e serviços.

Principais temas:

- cliente e servidor;
- HTTP;
- JSON;
- REST;
- consumo de APIs;
- autenticação;
- FastAPI;
- Pydantic;
- tratamento de erros;
- testes de API.

---

## 05 — Dados e SQL

Persistência e manipulação dos dados utilizados pelas aplicações.

Principais temas:

- bancos relacionais;
- SQL;
- CRUD;
- modelagem;
- JOINs;
- agregações;
- PostgreSQL;
- integração Python + banco;
- persistência com FastAPI;
- segurança básica;
- Pandas essencial.

### Entrega

**Projeto 03 — API + FastAPI + PostgreSQL**

---

## 06 — Fundamentos de IA e LLMs

Entrada nos fundamentos específicos de AI Engineering.

Principais temas:

- AI, Machine Learning e Deep Learning;
- Transformers;
- Large Language Models;
- tokens;
- context window;
- inferência;
- limitações de LLMs;
- APIs de modelos;
- Prompt Engineering;
- Context Engineering;
- Structured Outputs;
- avaliação básica.

### Entrega

**Projeto 04 — Aplicação com LLM**

---

## 07 — Embeddings e Busca Semântica

Fundamentos necessários para sistemas que recuperam informação por significado.

Principais temas:

- vetores;
- embeddings;
- similaridade;
- busca lexical e semântica;
- chunking;
- metadata;
- vector databases;
- indexação;
- retrieval;
- avaliação de recuperação.

---

## 08 — RAG

Construção de sistemas de Retrieval-Augmented Generation.

Principais temas:

- arquitetura RAG;
- ingestão;
- indexação;
- retrieval;
- construção de contexto;
- geração fundamentada;
- fontes;
- avaliação;
- diagnóstico de falhas;
- melhorias de retrieval.

### Entrega

**Projeto 05 — Sistema RAG**

---

## 09 — Agentes e Orquestração

Construção de aplicações capazes de utilizar ferramentas e coordenar múltiplas etapas.

Principais temas:

- Tool Calling;
- Function Calling;
- workflows;
- estado;
- agentes;
- agent loops;
- memória;
- LangChain;
- LangGraph;
- observabilidade;
- avaliação de sistemas agentic.

### Diferencial opcional

**MCP — Model Context Protocol**

MCP poderá ser estudado como tecnologia complementar após o domínio dos fundamentos de Tool Calling e agentes.

---

## 10 — Entrega e Produção Básica

Preparação das aplicações para execução reproduzível e disponibilização.

Principais temas:

- configuração;
- variáveis de ambiente;
- Docker;
- Docker Compose;
- cloud;
- deploy;
- logs;
- health checks;
- CI/CD;
- GitHub Actions;
- segurança;
- custos.

---

# Projetos progressivos

Os projetos fazem parte da trilha e não são uma etapa separada deixada para o final.

```text
Fundamentos de Programação
        ↓
Projeto 01 — Python e Lógica
        ↓
Python Aplicado
        ↓
Projeto 02 — Aplicação Python Estruturada
        ↓
APIs + Dados
        ↓
Projeto 03 — API + FastAPI + PostgreSQL
        ↓
LLMs
        ↓
Projeto 04 — Aplicação com LLM
        ↓
Embeddings + RAG
        ↓
Projeto 05 — Sistema RAG
```

Cada projeto deverá reutilizar competências anteriores sempre que fizer sentido.

---

# Projeto de Portfólio

Após as fases técnicas, será desenvolvido um projeto integrado de AI Engineering.

O projeto deverá demonstrar a capacidade de combinar conhecimentos da trilha em uma aplicação coerente.

Não existe obrigação de utilizar todas as tecnologias estudadas.

A arquitetura deverá ser determinada pelo problema.

Possíveis componentes incluem:

```text
FastAPI
   ↓
Aplicação
   ├── PostgreSQL
   ├── LLM
   ├── RAG
   └── Tools / Workflows
           ↓
       Serviços externos
```

O projeto deverá possuir:

- problema real e claramente definido;
- arquitetura justificável;
- código organizado;
- testes;
- avaliação das funcionalidades de IA;
- documentação;
- Git/GitHub;
- containerização;
- CI;
- deploy ou demonstração reproduzível;
- capacidade de defesa técnica.

A especificação detalhada está em `PROJETO-DE-PORTFOLIO.md`.

---

# Validação

O roadmap utiliza quatro estados:

- ⬜ Não iniciado
- 🟦 Em estudo
- 🟨 Em validação
- ✅ Validado

Um módulo não se torna `✅ Validado` apenas porque seu conteúdo foi estudado.

A validação poderá envolver:

- exercícios independentes;
- explicação com palavras próprias;
- leitura de código;
- debugging;
- implementação prática;
- testes;
- projetos;
- avaliações sem assistência.

---

# Uso de IA durante os estudos

Ferramentas de IA podem ser utilizadas como apoio durante o aprendizado.

Elas podem auxiliar em:

- explicações;
- exemplos;
- revisão;
- debugging guiado;
- comparação de soluções;
- documentação.

Entretanto, checkpoints específicos serão realizados **sem assistência de IA**.

O objetivo é garantir que a ferramenta acelere o aprendizado sem esconder lacunas de compreensão.

---

# Checkpoint técnico final

Após concluir as fases e o projeto de portfólio, será realizada uma validação integrada.

O checkpoint deverá avaliar:

- programação;
- debugging;
- Git/GitHub;
- APIs;
- SQL;
- LLMs;
- embeddings;
- RAG;
- Tool Calling;
- workflows e agentes;
- produção básica;
- explicação de arquitetura;
- defesa dos projetos.

Parte dessa avaliação será realizada sem assistência.

---

# 🏁 AI Engineer Junior Ready

Este é o marco final deste roadmap.

Será alcançado quando:

```text
Competências obrigatórias validadas
            +
Projetos concluídos
            +
Projeto de portfólio demonstrável
            +
Checkpoint técnico final aprovado
            ↓
🏁 AI Engineer Junior Ready
```

Ao atingir este marco:

> **Status profissional: Pronto para iniciar candidaturas a vagas de AI Engineer Junior.**

Isso não significa domínio de toda a área de Inteligência Artificial.

Significa possuir fundamentos, competências práticas, evidências de portfólio e capacidade técnica compatíveis com a busca pela primeira oportunidade profissional.

A progressão para níveis Pleno, Sênior ou especializações posteriores não faz parte deste roadmap.