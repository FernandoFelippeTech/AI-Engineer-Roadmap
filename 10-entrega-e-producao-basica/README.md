# Fase 10 — Entrega e Produção Básica

## Objetivo

Aprender a transformar uma aplicação de AI Engineering que funciona localmente em um sistema que pode ser configurado, executado, testado e disponibilizado de forma reproduzível.

Ao concluir esta fase, devo compreender os fundamentos de containerização, deploy, cloud, CI/CD, observabilidade e operação necessários para um AI Engineer Junior.

O objetivo não é dominar DevOps, Kubernetes ou arquiteturas distribuídas avançadas, mas conseguir entregar aplicações de IA com práticas básicas de produção.

---

# Módulos

## 01. Aplicação local versus aplicação em produção

**Status:** ⬜ Não iniciado

### Competências

- [ ] Diferenciar ambiente local de ambiente de produção
- [ ] Entender dependências externas de uma aplicação
- [ ] Identificar configurações que variam entre ambientes
- [ ] Entender por que "funciona na minha máquina" não é suficiente
- [ ] Identificar serviços necessários para executar uma aplicação
- [ ] Entender requisitos básicos de disponibilidade e confiabilidade
- [ ] Reconhecer limitações de uma aplicação antes do deploy

---

## 02. Configuração e variáveis de ambiente

**Status:** ⬜ Não iniciado

### Competências

- [ ] Separar configuração de código
- [ ] Utilizar variáveis de ambiente
- [ ] Trabalhar com arquivos `.env` durante desenvolvimento
- [ ] Utilizar `.gitignore` corretamente
- [ ] Evitar secrets no código
- [ ] Diferenciar configurações de desenvolvimento e produção
- [ ] Validar configurações obrigatórias na inicialização
- [ ] Entender princípios básicos de gerenciamento de secrets

---

## 03. Docker

**Status:** ⬜ Não iniciado

### Competências

- [ ] Entender o problema resolvido por containers
- [ ] Diferenciar imagem de container
- [ ] Entender o papel de um `Dockerfile`
- [ ] Criar uma imagem para uma aplicação Python
- [ ] Executar a aplicação em um container
- [ ] Mapear portas
- [ ] Configurar variáveis de ambiente
- [ ] Entender volumes em nível básico
- [ ] Utilizar `.dockerignore`
- [ ] Inspecionar logs de um container
- [ ] Parar e remover containers
- [ ] Reconstruir uma imagem após alterações
- [ ] Investigar falhas básicas de execução

---

## 04. Docker Compose

**Status:** ⬜ Não iniciado

### Competências

- [ ] Entender quando uma aplicação depende de múltiplos serviços
- [ ] Definir serviços em Docker Compose
- [ ] Executar aplicação e banco de dados em conjunto
- [ ] Configurar variáveis de ambiente
- [ ] Trabalhar com volumes
- [ ] Entender comunicação básica entre containers
- [ ] Inicializar e encerrar o ambiente
- [ ] Investigar falhas entre serviços

---

## 05. Cloud Computing essencial

**Status:** ⬜ Não iniciado

### Competências

- [ ] Entender o conceito de cloud computing
- [ ] Reconhecer os principais provedores de cloud
- [ ] Entender compute, storage, database e networking em nível introdutório
- [ ] Entender serviços gerenciados em nível conceitual
- [ ] Diferenciar infraestrutura local de recursos em cloud
- [ ] Entender regiões e disponibilidade em nível básico
- [ ] Reconhecer que recursos em cloud possuem custo
- [ ] Escolher um serviço simples para disponibilizar uma aplicação

---

## 06. Deploy

**Status:** ⬜ Não iniciado

### Competências

- [ ] Preparar uma aplicação para deploy
- [ ] Definir dependências de forma reproduzível
- [ ] Configurar variáveis de ambiente no ambiente remoto
- [ ] Executar uma API em ambiente remoto
- [ ] Verificar se a aplicação está acessível
- [ ] Investigar logs após falhas
- [ ] Atualizar uma aplicação após mudanças
- [ ] Executar smoke tests básicos após deploy
- [ ] Documentar como acessar e executar a aplicação

---

## 07. Logs e observabilidade básica

**Status:** ⬜ Não iniciado

### Competências

- [ ] Diferenciar logs de mensagens temporárias de debugging
- [ ] Utilizar níveis de log quando apropriado
- [ ] Registrar eventos relevantes
- [ ] Registrar erros com contexto útil
- [ ] Evitar registrar secrets
- [ ] Utilizar identificadores para rastrear operações quando necessário
- [ ] Entender métricas em nível introdutório
- [ ] Entender tracing em nível introdutório
- [ ] Investigar uma falha utilizando evidências da execução

---

## 08. Health checks e confiabilidade básica

**Status:** ⬜ Não iniciado

### Competências

- [ ] Entender o propósito de um health check
- [ ] Criar um endpoint de saúde
- [ ] Diferenciar aplicação iniciada de aplicação funcional
- [ ] Verificar dependências críticas quando apropriado
- [ ] Trabalhar com timeout em integrações externas
- [ ] Entender retry em nível básico
- [ ] Reconhecer riscos de retries indiscriminados
- [ ] Implementar tratamento adequado para indisponibilidade de serviços externos

---

## 09. CI/CD básico

**Status:** ⬜ Não iniciado

### Competências

- [ ] Entender Continuous Integration
- [ ] Entender Continuous Delivery/Deployment em nível conceitual
- [ ] Entender o papel de uma pipeline
- [ ] Executar testes automaticamente após mudanças
- [ ] Configurar uma pipeline básica no GitHub
- [ ] Identificar uma pipeline que falhou
- [ ] Corrigir uma falha e validar uma nova execução
- [ ] Entender como automação reduz erros manuais
- [ ] Reconhecer os limites de uma pipeline básica

---

## 10. GitHub Actions

**Status:** ⬜ Não iniciado

### Competências

- [ ] Entender workflows do GitHub Actions
- [ ] Entender eventos que iniciam workflows
- [ ] Configurar ambiente Python
- [ ] Instalar dependências
- [ ] Executar testes
- [ ] Interpretar logs da execução
- [ ] Utilizar secrets de forma apropriada
- [ ] Criar uma verificação automática útil para um projeto
- [ ] Evitar pipelines complexas sem necessidade

---

## 11. Segurança básica para aplicações de IA

**Status:** ⬜ Não iniciado

### Competências

- [ ] Evitar exposição de API keys e credenciais
- [ ] Validar entradas recebidas pela aplicação
- [ ] Entender princípio de menor privilégio em nível básico
- [ ] Reconhecer riscos de dependências externas
- [ ] Reconhecer riscos básicos de Prompt Injection
- [ ] Entender que conteúdo recuperado por RAG também pode ser não confiável
- [ ] Limitar ações disponíveis para agentes
- [ ] Evitar retornar detalhes internos desnecessários em mensagens de erro
- [ ] Reconhecer situações que exigem controles adicionais

---

## 12. Custos e limites operacionais

**Status:** ⬜ Não iniciado

### Competências

- [ ] Identificar componentes que geram custo
- [ ] Entender custo de chamadas a modelos em nível prático
- [ ] Relacionar tokens com custo
- [ ] Relacionar escolha de modelo com custo e latência
- [ ] Entender custos básicos de infraestrutura
- [ ] Configurar limites quando disponíveis
- [ ] Evitar chamadas externas desnecessárias
- [ ] Reconhecer trade-offs entre qualidade, velocidade e custo
- [ ] Estimar custos básicos de uma aplicação pequena

---

# Checkpoint da Fase 10

A fase será concluída somente quando eu conseguir:

- [ ] Containerizar uma aplicação Python/FastAPI
- [ ] Executar aplicação e dependências de forma reproduzível
- [ ] Gerenciar configurações sem expor secrets
- [ ] Explicar conceitos essenciais de cloud
- [ ] Fazer deploy de uma aplicação
- [ ] Validar o funcionamento após o deploy
- [ ] Utilizar logs para investigar uma falha
- [ ] Implementar health check
- [ ] Configurar uma pipeline básica de CI
- [ ] Executar testes automaticamente no GitHub
- [ ] Identificar e corrigir uma pipeline quebrada
- [ ] Aplicar práticas básicas de segurança
- [ ] Identificar custos relevantes da aplicação
- [ ] Explicar como a aplicação passa do código local para execução em produção

---

# Validação prática da fase

Uma aplicação desenvolvida anteriormente deverá ser preparada para execução fora do ambiente local.

A entrega deverá incluir:

```text
Código
    ↓
Testes
    ↓
Git/GitHub
    ↓
CI
    ↓
Docker
    ↓
Configuração
    ↓
Deploy
    ↓
Health Check
    ↓
Logs
    ↓
Aplicação disponível
```

Durante a validação, uma falha deverá ser introduzida ou simulada para que o processo de diagnóstico também seja exercitado.

---

## Fora do escopo obrigatório

Os seguintes temas poderão ser estudados posteriormente, mas não são requisitos para concluir esta fase:

- Kubernetes avançado;
- administração profunda de cloud;
- Infrastructure as Code avançada;
- arquiteturas distribuídas complexas;
- service mesh;
- observabilidade avançada;
- MLOps avançado;
- treinamento distribuído;
- operação de clusters de GPU.

Esses temas não devem atrasar a preparação para a primeira vaga de AI Engineer Junior.

---

## Resultado esperado

Ao concluir esta fase, devo conseguir pegar uma aplicação de AI Engineering desenvolvida localmente e prepará-la para execução reproduzível, testes automatizados e deploy.

Também devo conseguir investigar problemas básicos em produção utilizando logs, compreender os principais componentes de cloud envolvidos e discutir decisões simples de segurança, confiabilidade, custo e operação.

O objetivo é demonstrar que consigo não apenas construir uma funcionalidade de IA, mas também entregar uma aplicação utilizável.