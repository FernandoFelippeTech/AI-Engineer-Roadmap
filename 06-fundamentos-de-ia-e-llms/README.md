# Fase 06 — Fundamentos de IA e LLMs

## Objetivo

Construir a base conceitual e prática necessária para desenvolver aplicações com Inteligência Artificial Generativa e Large Language Models (LLMs).

Ao concluir esta fase, devo compreender o que um LLM faz, quais são suas principais limitações e como integrar modelos a aplicações utilizando APIs.

O foco é AI Engineering aplicado. Conceitos de Machine Learning serão estudados na profundidade necessária para compreender e construir sistemas de IA, sem transformar esta fase em uma formação completa de Data Science ou ML Engineering.

---

# Módulos

## 01. Mapa da Inteligência Artificial

**Status:** ⬜ Não iniciado

### Competências

- [ ] Entender o conceito geral de Inteligência Artificial
- [ ] Diferenciar AI, Machine Learning e Deep Learning
- [ ] Entender onde Generative AI se encaixa
- [ ] Entender onde LLMs se encaixam
- [ ] Diferenciar sistemas baseados em regras de sistemas baseados em modelos
- [ ] Reconhecer exemplos de diferentes tipos de sistemas de IA
- [ ] Explicar essas diferenças utilizando linguagem própria

---

## 02. Machine Learning essencial para AI Engineering

**Status:** ⬜ Não iniciado

### Competências

- [ ] Entender o conceito de modelo
- [ ] Diferenciar treinamento de inferência
- [ ] Entender features e labels em nível conceitual
- [ ] Diferenciar aprendizado supervisionado e não supervisionado
- [ ] Entender classificação e regressão
- [ ] Entender conjuntos de treino, validação e teste
- [ ] Entender overfitting em nível conceitual
- [ ] Entender o propósito de métricas de avaliação
- [ ] Reconhecer que diferentes problemas exigem diferentes métricas
- [ ] Diferenciar utilizar um modelo pronto de treinar um modelo

---

## 03. Fundamentos de Deep Learning e Transformers

**Status:** ⬜ Não iniciado

### Competências

- [ ] Entender o papel geral de redes neurais
- [ ] Entender que Deep Learning utiliza redes com múltiplas camadas
- [ ] Entender o conceito de parâmetros de um modelo
- [ ] Entender o papel geral da arquitetura Transformer
- [ ] Entender o conceito de attention em nível intuitivo
- [ ] Relacionar Transformers com LLMs modernos
- [ ] Diferenciar compreensão conceitual de implementação de uma arquitetura do zero

---

## 04. Large Language Models

**Status:** ⬜ Não iniciado

### Competências

- [ ] Entender o que é um LLM
- [ ] Entender de forma conceitual como um LLM gera texto
- [ ] Entender previsão de próximo token
- [ ] Entender que o modelo trabalha com probabilidades
- [ ] Diferenciar modelo base de modelo instruído
- [ ] Entender o conceito de instruction tuning em nível geral
- [ ] Entender que um LLM não funciona como um banco de dados tradicional
- [ ] Explicar por que uma resposta plausível pode estar incorreta

---

## 05. Tokens e contexto

**Status:** ⬜ Não iniciado

### Competências

- [ ] Entender o que são tokens
- [ ] Entender tokenização em nível conceitual
- [ ] Entender que tokens não correspondem necessariamente a palavras
- [ ] Entender context window
- [ ] Entender que contexto possui limite
- [ ] Relacionar quantidade de tokens com custo e latência
- [ ] Identificar informações relevantes para incluir no contexto
- [ ] Evitar enviar contexto desnecessário quando possível

---

## 06. Inferência e parâmetros de geração

**Status:** ⬜ Não iniciado

### Competências

- [ ] Entender o conceito de inferência
- [ ] Entender o papel de `temperature`
- [ ] Entender limites de saída
- [ ] Reconhecer parâmetros comuns de geração
- [ ] Entender que parâmetros podem alterar o comportamento da resposta
- [ ] Comparar resultados utilizando diferentes configurações
- [ ] Evitar tratar parâmetros como valores universais para qualquer problema

---

## 07. Limitações e riscos de LLMs

**Status:** ⬜ Não iniciado

### Competências

- [ ] Entender hallucinations
- [ ] Reconhecer que confiança aparente não significa precisão
- [ ] Entender limitações de conhecimento e contexto
- [ ] Reconhecer problemas causados por prompts ambíguos
- [ ] Entender riscos básicos relacionados a dados sensíveis
- [ ] Reconhecer que saída de modelo deve ser validada quando utilizada por software
- [ ] Entender que LLMs podem produzir formatos inesperados
- [ ] Definir estratégias básicas para lidar com falhas

---

## 08. APIs de LLMs

**Status:** ⬜ Não iniciado

### Competências

- [ ] Integrar uma aplicação Python com uma API de LLM
- [ ] Configurar credenciais por variáveis de ambiente
- [ ] Enviar instruções e contexto ao modelo
- [ ] Interpretar a resposta da API
- [ ] Tratar erros da API
- [ ] Trabalhar com timeout
- [ ] Entender rate limits em nível básico
- [ ] Considerar custo por utilização
- [ ] Registrar informações úteis para debugging sem expor secrets
- [ ] Separar a integração com o modelo da lógica principal da aplicação

---

## 09. Prompt Engineering

**Status:** ⬜ Não iniciado

### Competências

- [ ] Escrever instruções claras
- [ ] Definir objetivo e contexto
- [ ] Definir restrições
- [ ] Solicitar formatos de saída
- [ ] Utilizar exemplos quando forem úteis
- [ ] Entender zero-shot e few-shot em nível prático
- [ ] Identificar ambiguidades em prompts
- [ ] Comparar versões de um prompt
- [ ] Avaliar resultados em vez de escolher prompts apenas por impressão
- [ ] Evitar depender de frases mágicas sem compreender o problema

---

## 10. Context Engineering

**Status:** ⬜ Não iniciado

### Competências

- [ ] Diferenciar instrução de contexto
- [ ] Selecionar informações relevantes para uma tarefa
- [ ] Organizar contexto de forma compreensível
- [ ] Evitar contexto excessivo ou irrelevante
- [ ] Entender que a qualidade da entrada influencia a qualidade da saída
- [ ] Estruturar informações provenientes de diferentes fontes
- [ ] Preparar contexto para futuras aplicações de RAG e agentes

---

## 11. Structured Outputs

**Status:** ⬜ Não iniciado

### Competências

- [ ] Entender por que software precisa de respostas estruturadas
- [ ] Solicitar saída em formato definido
- [ ] Trabalhar com JSON gerado por modelos
- [ ] Validar a saída antes de utilizá-la
- [ ] Utilizar schemas quando suportados
- [ ] Integrar saída estruturada com modelos Pydantic
- [ ] Tratar respostas inválidas ou incompletas
- [ ] Diferenciar texto destinado a humanos de dados destinados a software

---

## 12. Avaliação básica de aplicações com LLM

**Status:** ⬜ Não iniciado

### Competências

- [ ] Definir exemplos de entrada para avaliação
- [ ] Definir o comportamento esperado
- [ ] Comparar respostas de maneira sistemática
- [ ] Identificar critérios básicos de qualidade
- [ ] Registrar falhas encontradas
- [ ] Comparar mudanças de prompt ou modelo
- [ ] Evitar avaliar uma aplicação utilizando apenas um exemplo
- [ ] Reconhecer quando avaliação humana ainda é necessária

---

# Checkpoint da Fase 06

A fase será concluída somente quando eu conseguir:

- [ ] Explicar a relação entre AI, ML, Deep Learning, Generative AI e LLMs
- [ ] Explicar treinamento e inferência em nível conceitual
- [ ] Explicar tokens e context window
- [ ] Descrever como um LLM produz uma resposta em nível apropriado para Junior
- [ ] Explicar as principais limitações de um LLM
- [ ] Integrar uma aplicação Python com uma API de LLM
- [ ] Trabalhar com credenciais sem expô-las no código
- [ ] Criar e comparar prompts de forma sistemática
- [ ] Construir respostas estruturadas e validá-las
- [ ] Tratar erros básicos da integração
- [ ] Avaliar o comportamento da aplicação utilizando múltiplos exemplos
- [ ] Explicar as decisões tomadas na implementação

---

# Projeto 04 — Aplicação com LLM

Após validar as competências necessárias, será desenvolvida uma aplicação funcional utilizando um LLM.

O projeto deverá incluir:

- integração com uma API de LLM;
- backend em Python;
- gerenciamento seguro de credenciais;
- Prompt Engineering;
- Context Engineering;
- Structured Outputs quando apropriado;
- validação das respostas utilizadas pelo software;
- tratamento de erros;
- testes;
- conjunto básico de casos de avaliação;
- documentação;
- Git e GitHub.

O projeto não deverá ser apenas um chatbot genérico.

O problema será escolhido de forma que o LLM execute uma função clara dentro de uma aplicação e que seja possível justificar por que um modelo de linguagem é adequado para aquela tarefa.

---

## Resultado esperado

Ao concluir esta fase, devo conseguir desenvolver uma aplicação baseada em LLM entendendo o caminho completo entre a entrada do usuário, o backend, a chamada ao modelo, o processamento da resposta e a saída da aplicação.

Também devo conseguir explicar limitações, custos, possíveis falhas e decisões de implementação, em vez de tratar o modelo como uma caixa-preta que simplesmente produz respostas.