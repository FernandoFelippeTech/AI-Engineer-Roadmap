# Fase 08 — RAG

## Objetivo

Aprender a construir sistemas de Retrieval-Augmented Generation (RAG), combinando recuperação de informações com Large Language Models para produzir respostas fundamentadas em fontes externas.

Ao concluir esta fase, devo conseguir implementar um pipeline RAG completo, avaliar separadamente retrieval e geração, identificar falhas e explicar as principais decisões de arquitetura.

O foco será construir primeiro uma implementação compreensível, evitando depender de frameworks que escondam etapas importantes do processo.

---

# Módulos

## 01. Fundamentos de RAG

**Status:** ⬜ Não iniciado

### Competências

- [ ] Entender o significado de Retrieval-Augmented Generation
- [ ] Explicar por que RAG é utilizado
- [ ] Diferenciar conhecimento do modelo de contexto recuperado
- [ ] Entender quando RAG pode ser mais adequado do que apenas Prompt Engineering
- [ ] Diferenciar RAG de fine-tuning em nível conceitual
- [ ] Identificar problemas que podem ser resolvidos com RAG
- [ ] Reconhecer situações em que RAG não é necessário

---

## 02. Arquitetura de um sistema RAG

**Status:** ⬜ Não iniciado

### Competências

- [ ] Entender a separação entre indexação e consulta
- [ ] Identificar os componentes de um pipeline RAG
- [ ] Entender o papel da fonte de dados
- [ ] Entender o papel do chunking
- [ ] Entender o papel dos embeddings
- [ ] Entender o papel do vector database
- [ ] Entender o papel do retriever
- [ ] Entender o papel do LLM
- [ ] Explicar o fluxo completo de dados no sistema

---

## 03. Ingestão de documentos

**Status:** ⬜ Não iniciado

### Competências

- [ ] Carregar documentos de uma fonte definida
- [ ] Extrair texto utilizável
- [ ] Normalizar dados quando necessário
- [ ] Preservar informações de origem
- [ ] Associar metadata
- [ ] Identificar documentos inválidos ou vazios
- [ ] Tratar falhas durante a ingestão
- [ ] Preparar os dados para indexação

---

## 04. Indexação para RAG

**Status:** ⬜ Não iniciado

### Competências

- [ ] Definir uma estratégia de chunking
- [ ] Gerar embeddings
- [ ] Armazenar conteúdo, vetores e metadata
- [ ] Criar ou atualizar um índice
- [ ] Evitar duplicação evidente
- [ ] Preservar informações necessárias para citações
- [ ] Validar se os documentos foram indexados corretamente
- [ ] Investigar falhas no pipeline de indexação

---

## 05. Retrieval

**Status:** ⬜ Não iniciado

### Competências

- [ ] Transformar uma pergunta em uma consulta de recuperação
- [ ] Recuperar chunks semanticamente relacionados
- [ ] Trabalhar com `top-k`
- [ ] Utilizar filtros por metadata quando apropriado
- [ ] Inspecionar os documentos recuperados
- [ ] Diferenciar relevância de similaridade numérica
- [ ] Identificar informações relevantes que não foram recuperadas
- [ ] Ajustar retrieval com base em evidências

---

## 06. Construção do contexto

**Status:** ⬜ Não iniciado

### Competências

- [ ] Transformar resultados recuperados em contexto para o LLM
- [ ] Organizar múltiplos chunks
- [ ] Preservar identificação das fontes
- [ ] Controlar quantidade de contexto
- [ ] Evitar incluir conteúdo irrelevante quando possível
- [ ] Criar instruções para utilização das fontes
- [ ] Definir comportamento quando a informação necessária não estiver disponível
- [ ] Relacionar contexto utilizado com a resposta produzida

---

## 07. Geração fundamentada

**Status:** ⬜ Não iniciado

### Competências

- [ ] Enviar pergunta e contexto ao LLM
- [ ] Orientar o modelo a utilizar o contexto fornecido
- [ ] Reduzir respostas não fundamentadas
- [ ] Solicitar que o modelo reconheça ausência de informação quando apropriado
- [ ] Produzir respostas compreensíveis
- [ ] Validar formatos estruturados quando utilizados
- [ ] Diferenciar uma falha de geração de uma falha de retrieval

---

## 08. Fontes e rastreabilidade

**Status:** ⬜ Não iniciado

### Competências

- [ ] Preservar a origem dos chunks recuperados
- [ ] Associar fontes à resposta
- [ ] Apresentar referências compreensíveis ao usuário
- [ ] Evitar atribuir uma informação a uma fonte que não a sustenta
- [ ] Permitir rastrear uma resposta até o conteúdo recuperado
- [ ] Utilizar metadata para melhorar rastreabilidade
- [ ] Verificar manualmente exemplos de citações produzidas

---

## 09. Avaliação de retrieval

**Status:** ⬜ Não iniciado

### Competências

- [ ] Criar perguntas com respostas conhecidas
- [ ] Definir quais documentos ou chunks deveriam ser recuperados
- [ ] Verificar se informação relevante aparece nos resultados
- [ ] Identificar falsos resultados relevantes
- [ ] Comparar diferentes configurações de retrieval
- [ ] Avaliar impacto de mudanças no chunking
- [ ] Avaliar impacto de filtros e quantidade de resultados
- [ ] Registrar resultados de experimentos

---

## 10. Avaliação de respostas RAG

**Status:** ⬜ Não iniciado

### Competências

- [ ] Avaliar se a resposta responde à pergunta
- [ ] Avaliar se a resposta está sustentada pelo contexto
- [ ] Identificar afirmações sem suporte
- [ ] Verificar se as fontes apresentadas sustentam a resposta
- [ ] Criar um conjunto pequeno e reproduzível de casos de teste
- [ ] Comparar mudanças no pipeline
- [ ] Evitar avaliar o sistema apenas por impressão subjetiva
- [ ] Reconhecer limitações de avaliações automáticas

---

## 11. Diagnóstico de falhas em RAG

**Status:** ⬜ Não iniciado

### Competências

- [ ] Identificar falhas de ingestão
- [ ] Identificar falhas de chunking
- [ ] Identificar falhas de indexação
- [ ] Identificar falhas de retrieval
- [ ] Identificar contexto irrelevante ou insuficiente
- [ ] Identificar falhas de geração
- [ ] Formular hipóteses antes de alterar o sistema
- [ ] Testar uma alteração por vez
- [ ] Comparar resultados antes e depois de uma mudança
- [ ] Explicar a causa provável de uma falha

---

## 12. Melhorias de retrieval

**Status:** ⬜ Não iniciado

### Competências

- [ ] Ajustar `top-k` com justificativa
- [ ] Utilizar filtros por metadata
- [ ] Comparar estratégias de chunking
- [ ] Entender busca híbrida em nível introdutório
- [ ] Entender reranking em nível introdutório
- [ ] Reconhecer quando uma técnica adicional realmente melhora o sistema
- [ ] Evitar adicionar complexidade sem evidência de benefício

---

## 13. RAG como aplicação

**Status:** ⬜ Não iniciado

### Competências

- [ ] Expor o sistema por uma API
- [ ] Validar entradas
- [ ] Tratar erros de serviços externos
- [ ] Gerenciar secrets
- [ ] Registrar informações úteis para debugging
- [ ] Armazenar dados persistentes quando necessário
- [ ] Criar testes para componentes críticos
- [ ] Documentar arquitetura e execução
- [ ] Organizar o código em componentes compreensíveis

---

# Checkpoint da Fase 08

A fase será concluída somente quando eu conseguir:

- [ ] Explicar RAG sem depender de definições decoradas
- [ ] Diferenciar RAG, Prompt Engineering e fine-tuning
- [ ] Explicar separadamente indexação e consulta
- [ ] Construir um pipeline de ingestão e indexação
- [ ] Implementar retrieval
- [ ] Construir contexto para um LLM
- [ ] Gerar respostas fundamentadas
- [ ] Preservar e apresentar fontes
- [ ] Avaliar retrieval separadamente da resposta final
- [ ] Criar casos reproduzíveis de avaliação
- [ ] Diagnosticar uma falha proposital no pipeline
- [ ] Justificar mudanças utilizando resultados de testes
- [ ] Explicar a arquitetura completa do sistema

---

# Projeto 05 — Sistema RAG

Após validar as competências necessárias, será desenvolvido um sistema RAG completo utilizando documentos ou uma base de conhecimento com utilidade real.

O projeto deverá incluir:

- ingestão de documentos;
- processamento e chunking;
- metadata;
- embeddings;
- armazenamento vetorial;
- retrieval;
- integração com LLM;
- respostas fundamentadas;
- indicação de fontes;
- API com FastAPI;
- configuração segura;
- tratamento de erros;
- testes;
- conjunto de avaliação;
- documentação da arquitetura;
- Git e GitHub.

O projeto não deverá ser apenas uma demonstração de biblioteca ou tutorial reproduzido.

Deverá existir um problema definido, decisões técnicas justificáveis e evidências de que o comportamento do sistema foi avaliado.

---

## Estratégia de implementação

A primeira versão deverá priorizar componentes explícitos e compreensíveis.

Frameworks de orquestração poderão ser introduzidos posteriormente, mas não deverão substituir a compreensão das etapas fundamentais.

O objetivo é conseguir explicar:

```text
Documentos
    ↓
Ingestão
    ↓
Chunking + Metadata
    ↓
Embeddings
    ↓
Vector Database
    ↓
Retrieval
    ↓
Contexto
    ↓
LLM
    ↓
Resposta + Fontes
```

Quando ocorrer uma falha, devo conseguir investigar **em qual parte desse fluxo ela provavelmente surgiu**.

---

## Resultado esperado

Ao concluir esta fase, devo conseguir desenvolver, testar e explicar um sistema RAG completo.

Também devo conseguir avaliar se um problema está na recuperação da informação ou na geração da resposta e realizar melhorias baseadas em evidências, em vez de alterar prompts, modelos e parâmetros aleatoriamente.

Essa competência representa uma das capacidades centrais esperadas para o perfil de AI Engineer Junior definido neste roadmap.