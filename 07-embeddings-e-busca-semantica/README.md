# Fase 07 — Embeddings e Busca Semântica

## Objetivo

Compreender como informações podem ser representadas numericamente e recuperadas por significado, construindo a base necessária para sistemas de RAG e outras aplicações de AI Engineering.

Ao concluir esta fase, devo conseguir gerar embeddings, armazená-los, realizar buscas por similaridade e construir um fluxo simples de busca semântica.

O objetivo não é estudar toda a matemática de espaços vetoriais em profundidade, mas compreender os conceitos necessários para implementar, investigar e explicar esse tipo de sistema.

---

# Módulos

## 01. Representações vetoriais

**Status:** ⬜ Não iniciado

### Competências

- [ ] Entender o conceito de vetor em nível aplicado
- [ ] Entender que dados podem ser representados numericamente
- [ ] Relacionar representações vetoriais com Machine Learning
- [ ] Entender o conceito de espaço vetorial em nível intuitivo
- [ ] Entender que proximidade entre vetores pode representar similaridade
- [ ] Diferenciar representação numérica de significado literal
- [ ] Explicar por que vetores são úteis em sistemas de busca semântica

---

## 02. Embeddings

**Status:** ⬜ Não iniciado

### Competências

- [ ] Entender o que é um embedding
- [ ] Entender como texto pode ser convertido em embeddings
- [ ] Entender que embeddings possuem múltiplas dimensões
- [ ] Entender que conteúdos semanticamente relacionados tendem a possuir representações próximas
- [ ] Gerar embeddings utilizando um modelo ou API
- [ ] Comparar embeddings de diferentes textos
- [ ] Entender que modelos de embeddings diferentes podem produzir representações incompatíveis
- [ ] Escolher um modelo de embeddings considerando o problema em nível básico

---

## 03. Similaridade

**Status:** ⬜ Não iniciado

### Competências

- [ ] Entender o conceito de similaridade entre vetores
- [ ] Entender cosine similarity em nível conceitual
- [ ] Reconhecer outras medidas de distância em nível introdutório
- [ ] Calcular ou utilizar uma implementação de similaridade
- [ ] Ordenar resultados por similaridade
- [ ] Entender que maior similaridade não garante relevância perfeita
- [ ] Investigar resultados semanticamente inesperados

---

## 04. Busca lexical versus busca semântica

**Status:** ⬜ Não iniciado

### Competências

- [ ] Entender busca baseada em correspondência de palavras
- [ ] Entender busca baseada em significado
- [ ] Comparar busca lexical e busca semântica
- [ ] Identificar situações em que busca lexical pode ser suficiente
- [ ] Identificar situações em que busca semântica oferece vantagem
- [ ] Entender que diferentes estratégias podem ser combinadas
- [ ] Avaliar resultados utilizando consultas reais

---

## 05. Chunking

**Status:** ⬜ Não iniciado

### Competências

- [ ] Entender por que documentos são divididos em chunks
- [ ] Entender o impacto do tamanho dos chunks
- [ ] Entender o conceito de overlap
- [ ] Comparar diferentes estratégias simples de chunking
- [ ] Preservar contexto relevante durante a divisão
- [ ] Evitar chunks excessivamente pequenos ou grandes sem justificativa
- [ ] Relacionar chunking com qualidade da recuperação
- [ ] Avaliar uma estratégia utilizando exemplos reais

---

## 06. Metadata

**Status:** ⬜ Não iniciado

### Competências

- [ ] Entender o papel de metadata
- [ ] Associar informações de origem aos chunks
- [ ] Armazenar identificadores de documentos
- [ ] Registrar informações úteis como título, seção ou fonte
- [ ] Utilizar metadata para filtrar resultados
- [ ] Preservar informações necessárias para rastrear a origem de um resultado
- [ ] Evitar armazenar metadata sem utilidade para a aplicação

---

## 07. Vector Databases

**Status:** ⬜ Não iniciado

### Competências

- [ ] Entender o propósito de um vector database
- [ ] Diferenciar banco relacional de armazenamento orientado à busca vetorial
- [ ] Criar uma coleção ou índice vetorial
- [ ] Armazenar embeddings
- [ ] Associar embeddings a conteúdo e metadata
- [ ] Executar buscas por similaridade
- [ ] Recuperar os resultados mais próximos
- [ ] Atualizar ou remover dados quando necessário
- [ ] Entender persistência em nível básico
- [ ] Utilizar pelo menos uma solução de armazenamento vetorial na prática

---

## 08. Pipeline de indexação

**Status:** ⬜ Não iniciado

### Competências

- [ ] Receber documentos ou dados de origem
- [ ] Extrair o conteúdo necessário
- [ ] Dividir conteúdo em chunks
- [ ] Associar metadata
- [ ] Gerar embeddings
- [ ] Armazenar os vetores
- [ ] Evitar indexação duplicada quando possível
- [ ] Identificar em qual etapa ocorreu uma falha
- [ ] Explicar o fluxo completo de indexação

---

## 09. Pipeline de busca semântica

**Status:** ⬜ Não iniciado

### Competências

- [ ] Receber uma consulta do usuário
- [ ] Gerar o embedding da consulta
- [ ] Executar busca por similaridade
- [ ] Definir quantidade de resultados recuperados
- [ ] Retornar conteúdo e metadata relevantes
- [ ] Inspecionar os resultados recuperados
- [ ] Identificar resultados irrelevantes
- [ ] Ajustar parâmetros básicos da recuperação
- [ ] Explicar o fluxo completo da consulta até os resultados

---

## 10. Avaliação básica de retrieval

**Status:** ⬜ Não iniciado

### Competências

- [ ] Criar um pequeno conjunto de consultas de teste
- [ ] Definir quais informações deveriam ser recuperadas
- [ ] Comparar resultados esperados e recuperados
- [ ] Identificar falhas de recuperação
- [ ] Investigar se a falha está relacionada a chunking, embeddings, metadata ou consulta
- [ ] Comparar alterações de configuração
- [ ] Evitar avaliar qualidade utilizando apenas uma consulta
- [ ] Registrar decisões e resultados de experimentos

---

# Checkpoint da Fase 07

A fase será concluída somente quando eu conseguir:

- [ ] Explicar embeddings utilizando linguagem própria
- [ ] Explicar por que similaridade vetorial permite busca semântica
- [ ] Gerar embeddings de textos
- [ ] Comparar semanticamente diferentes conteúdos
- [ ] Criar uma estratégia de chunking e justificar a escolha
- [ ] Associar metadata aos dados indexados
- [ ] Armazenar embeddings em uma solução vetorial
- [ ] Implementar busca por similaridade
- [ ] Construir um pipeline completo de indexação
- [ ] Construir um pipeline completo de busca
- [ ] Avaliar resultados utilizando múltiplas consultas
- [ ] Investigar resultados ruins sem alterar parâmetros aleatoriamente

---

# Aplicação prática da fase

Será desenvolvido um mecanismo simples de busca semântica antes da introdução de RAG.

O fluxo deverá seguir aproximadamente:

```text
Documentos
    ↓
Extração
    ↓
Chunking
    ↓
Metadata
    ↓
Embeddings
    ↓
Vector Database
    ↓
Indexação
```

Para uma consulta:

```text
Pergunta
    ↓
Embedding da pergunta
    ↓
Busca por similaridade
    ↓
Resultados mais relevantes
    ↓
Conteúdo + fonte
```

Neste momento, o sistema deverá funcionar **sem depender de um LLM para produzir a resposta final**.

Essa separação permitirá avaliar se a recuperação funciona corretamente antes de adicionar geração de linguagem ao sistema.

---

## Resultado esperado

Ao concluir esta fase, devo conseguir construir um sistema que recebe documentos, transforma seu conteúdo em representações vetoriais e recupera informações semanticamente relacionadas a uma consulta.

Também devo conseguir investigar por que determinado conteúdo foi ou não recuperado e explicar como chunking, embeddings, metadata e busca vetorial afetam o resultado.

Essa competência será utilizada diretamente na próxima fase para construir sistemas de Retrieval-Augmented Generation (RAG).