# Fase 09 — Agentes e Orquestração

## Objetivo

Aprender a construir aplicações de IA capazes de utilizar ferramentas, executar ações e coordenar múltiplas etapas de processamento.

Ao concluir esta fase, devo compreender a diferença entre uma chamada simples a um LLM, Tool Calling, workflows e agentes, além de conseguir implementar esses padrões com controle de estado, tratamento de falhas e limites claros de execução.

Frameworks como LangChain e LangGraph serão utilizados após a compreensão dos mecanismos fundamentais que eles abstraem.

---

# Módulos

## 01. De LLMs para sistemas capazes de agir

**Status:** ⬜ Não iniciado

### Competências

- [ ] Diferenciar geração de texto de execução de ações
- [ ] Entender por que um LLM não executa uma função apenas por descrevê-la
- [ ] Entender o papel da aplicação na execução de ferramentas
- [ ] Diferenciar LLM, ferramenta e orquestrador
- [ ] Identificar tarefas que podem exigir ferramentas
- [ ] Reconhecer situações em que uma chamada simples ao LLM é suficiente
- [ ] Evitar utilizar agentes quando um fluxo determinístico resolve o problema

---

## 02. Tool Calling e Function Calling

**Status:** ⬜ Não iniciado

### Competências

- [ ] Entender o conceito de Tool Calling
- [ ] Entender Function Calling como mecanismo de integração
- [ ] Definir uma ferramenta com nome, descrição e parâmetros
- [ ] Utilizar schemas para os argumentos
- [ ] Permitir que o modelo selecione uma ferramenta
- [ ] Interpretar uma solicitação de chamada de ferramenta
- [ ] Executar a função correspondente na aplicação
- [ ] Retornar o resultado da ferramenta ao modelo
- [ ] Produzir uma resposta final utilizando o resultado
- [ ] Entender que o modelo solicita a ação, mas a aplicação controla sua execução

---

## 03. Validação e segurança de ferramentas

**Status:** ⬜ Não iniciado

### Competências

- [ ] Validar argumentos antes da execução
- [ ] Rejeitar parâmetros inválidos
- [ ] Tratar exceptions das ferramentas
- [ ] Definir timeout quando apropriado
- [ ] Evitar expor secrets ao modelo
- [ ] Limitar quais operações podem ser executadas
- [ ] Diferenciar operações de leitura de operações com efeitos colaterais
- [ ] Reconhecer quando uma ação exige confirmação
- [ ] Registrar chamadas úteis para debugging
- [ ] Evitar confiar cegamente em argumentos produzidos pelo LLM

---

## 04. Workflows determinísticos

**Status:** ⬜ Não iniciado

### Competências

- [ ] Entender o conceito de workflow
- [ ] Dividir uma tarefa em etapas
- [ ] Encadear operações
- [ ] Criar decisões condicionais
- [ ] Definir caminhos explícitos de execução
- [ ] Compartilhar dados entre etapas
- [ ] Tratar falhas em etapas específicas
- [ ] Entender quando um workflow é preferível a um agente
- [ ] Construir um workflow utilizando Python antes de depender de um framework

---

## 05. Estado

**Status:** ⬜ Não iniciado

### Competências

- [ ] Entender o conceito de estado em uma aplicação de IA
- [ ] Identificar informações que precisam persistir entre etapas
- [ ] Atualizar estado de forma controlada
- [ ] Diferenciar estado temporário de persistente
- [ ] Evitar armazenar informações desnecessárias
- [ ] Entender problemas causados por estado inconsistente
- [ ] Utilizar estruturas de dados claras para representar estado
- [ ] Inspecionar o estado durante debugging

---

## 06. Fundamentos de agentes

**Status:** ⬜ Não iniciado

### Competências

- [ ] Entender o conceito de agente em aplicações com LLM
- [ ] Diferenciar agente de workflow determinístico
- [ ] Entender o ciclo decisão → ação → observação
- [ ] Permitir que um modelo escolha entre múltiplas ferramentas
- [ ] Utilizar o resultado de uma ferramenta em uma próxima decisão
- [ ] Definir condições de encerramento
- [ ] Definir limite de iterações
- [ ] Reconhecer riscos de loops desnecessários
- [ ] Entender que maior autonomia aumenta a necessidade de controle

---

## 07. Agent Loop

**Status:** ⬜ Não iniciado

### Competências

- [ ] Implementar um loop simples de agente
- [ ] Receber uma tarefa
- [ ] Solicitar uma decisão ao modelo
- [ ] Identificar uma chamada de ferramenta
- [ ] Executar a ferramenta
- [ ] Adicionar a observação ao estado
- [ ] Repetir o processo quando necessário
- [ ] Detectar uma resposta final
- [ ] Interromper a execução ao atingir limites
- [ ] Investigar um loop que não termina corretamente

---

## 08. Memória e contexto em sistemas agentic

**Status:** ⬜ Não iniciado

### Competências

- [ ] Diferenciar contexto atual de memória persistente
- [ ] Entender memória de curto prazo em nível aplicado
- [ ] Entender memória persistente em nível introdutório
- [ ] Selecionar informações relevantes para o contexto
- [ ] Evitar crescimento ilimitado do histórico
- [ ] Reconhecer riscos de recuperar memórias irrelevantes
- [ ] Entender que memória não significa enviar todo o histórico ao modelo
- [ ] Relacionar memória, estado e persistência

---

## 09. LangChain

**Status:** ⬜ Não iniciado

### Competências

- [ ] Entender o propósito do LangChain
- [ ] Reconhecer as abstrações oferecidas pelo framework
- [ ] Integrar modelos utilizando suas interfaces
- [ ] Trabalhar com prompts e structured outputs
- [ ] Criar e utilizar tools
- [ ] Compor operações
- [ ] Entender onde o framework reduz código repetitivo
- [ ] Conseguir relacionar abstrações do framework aos mecanismos estudados anteriormente
- [ ] Evitar depender de abstrações que não consigo explicar

---

## 10. LangGraph

**Status:** ⬜ Não iniciado

### Competências

- [ ] Entender o propósito do LangGraph
- [ ] Representar um workflow como grafo
- [ ] Entender nodes e edges
- [ ] Trabalhar com estado
- [ ] Criar caminhos condicionais
- [ ] Implementar ciclos controlados
- [ ] Integrar ferramentas
- [ ] Definir condições de encerramento
- [ ] Inspecionar a execução de um grafo
- [ ] Construir um workflow agentic simples

---

## 11. Observabilidade e debugging

**Status:** ⬜ Não iniciado

### Competências

- [ ] Registrar etapas importantes da execução
- [ ] Identificar qual ferramenta foi selecionada
- [ ] Registrar duração de operações quando útil
- [ ] Identificar erros em ferramentas
- [ ] Inspecionar alterações de estado
- [ ] Identificar loops inesperados
- [ ] Rastrear uma execução do início ao fim
- [ ] Evitar registrar secrets ou dados sensíveis
- [ ] Formular hipóteses antes de alterar prompts ou arquitetura

---

## 12. Avaliação de sistemas com ferramentas e agentes

**Status:** ⬜ Não iniciado

### Competências

- [ ] Criar tarefas reproduzíveis para avaliação
- [ ] Verificar se a ferramenta correta foi selecionada
- [ ] Verificar se os argumentos utilizados foram adequados
- [ ] Avaliar se a tarefa foi concluída
- [ ] Identificar etapas desnecessárias
- [ ] Comparar comportamento entre diferentes casos
- [ ] Testar cenários de erro
- [ ] Avaliar se um agente realmente oferece vantagem sobre um workflow
- [ ] Registrar falhas para futuras melhorias

---

# Checkpoint da Fase 09

A fase será concluída somente quando eu conseguir:

- [ ] Explicar Tool Calling utilizando linguagem própria
- [ ] Implementar Tool Calling sem depender de um framework de agentes
- [ ] Validar argumentos antes de executar uma ferramenta
- [ ] Construir um workflow determinístico
- [ ] Trabalhar com estado entre etapas
- [ ] Explicar a diferença entre workflow e agente
- [ ] Implementar um agent loop simples
- [ ] Definir limites e condições de encerramento
- [ ] Utilizar múltiplas ferramentas com segurança básica
- [ ] Utilizar LangChain compreendendo as abstrações utilizadas
- [ ] Construir um workflow com LangGraph
- [ ] Investigar uma execução com falha
- [ ] Avaliar se o sistema concluiu corretamente uma tarefa
- [ ] Justificar quando utilizar ou não um agente

---

# Aplicação prática da fase

Será construída uma aplicação capaz de utilizar múltiplas ferramentas para concluir tarefas.

Uma arquitetura possível será:

```text
Usuário
    ↓
Aplicação
    ↓
LLM
    ↓
Decisão
    ├── Responder
    │
    └── Utilizar ferramenta
            ↓
        Validação
            ↓
        Execução
            ↓
        Resultado
            ↓
        Estado
            ↓
        Próxima decisão
```

A aplicação deverá possuir limites explícitos e comportamento observável.

O objetivo não é criar um sistema com o maior número possível de agentes, mas construir uma solução em que a utilização de ferramentas ou autonomia seja tecnicamente justificável.

---

# Diferencial opcional — MCP

Após dominar Tool Calling e os fundamentos de agentes, poderei estudar Model Context Protocol (MCP) como competência adicional.

### Competências opcionais

- [ ] Entender o problema que MCP busca resolver
- [ ] Entender a relação entre aplicações de IA, MCP clients e MCP servers
- [ ] Diferenciar MCP de Tool Calling
- [ ] Consumir ferramentas disponibilizadas por um MCP server
- [ ] Entender MCP como protocolo de integração, e não como substituto dos fundamentos anteriores

MCP é tratado como diferencial e tecnologia emergente, não como requisito obrigatório para concluir esta fase.

---

## Resultado esperado

Ao concluir esta fase, devo conseguir construir aplicações de IA que utilizam ferramentas e coordenam múltiplas etapas de forma controlada.

Também devo conseguir escolher entre uma chamada simples ao LLM, um workflow determinístico ou um agente, justificando a decisão com base no problema em vez de utilizar agentes apenas por tendência tecnológica.

Frameworks como LangChain e LangGraph deverão funcionar como ferramentas de engenharia que aceleram a implementação, e não como substitutos da compreensão do sistema.