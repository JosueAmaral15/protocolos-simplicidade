# Protocolo Simplicidade 1

**Autor**: Josué Amaral  
**Data de Criação**: 30 de Novembro de 2025  
**Versão**: 2.3  
**Última Atualização**: 01 de Janeiro de 2026  
**Objetivo**: Metodologia profissional para desenvolvimento incremental de qualidade

**Changelog v2.3** (01/01/2026):
- ✅ **[NOVO]** Stack Padrão Recomendado para Sites/Aplicações Web
- ✅ Next.js 15.5.2 + React 19.1.1 + TypeScript 5.9.2 como padrão
- ✅ Stack completo: Turbopack, Tailwind CSS, Zustand, Jest, ESLint
- ✅ Inclui integrações: Cloudinary, Stripe, APIs de IA (opcional)
- ✅ Deploy em Vercel (gratuito), backend em Heroku
- ✅ Aplicável quando usuário NÃO especificar tecnologias
- ✅ Justificativa: Cobre 90% dos casos de uso web modernos
- ✅ Quando NÃO usar: Vue/Angular, Python backend, desktop/mobile

**Changelog v2.2** (01/01/2026):
- ✅ **[CRÍTICO]** Adicionada Etapa 1.0: Busca e Leitura Completa de Documentação (PRIORITÁRIO)
- ✅ IA DEVE procurar e ler 100% da documentação markdown ANTES de qualquer tarefa
- ✅ Busca recursiva por todos arquivos .md no workspace (find + grep)
- ✅ Se não encontrar documentação, IA deve perguntar ao usuário
- ✅ Se não existir, IA deve criar estrutura mínima (README, REQUIREMENTS, TASKS)
- ✅ Templates completos para criação de documentação inicial
- ✅ Checklist de 9 itens obrigatórios antes de prosseguir
- ✅ Orientações sobre comentários no código (por quê, não apenas o que)
- ✅ Rationale: Contexto é tudo, evita duplicação e retrabalho

**Changelog v2.1** (01/01/2026):
- ✅ **[OBRIGATÓRIO]** Adicionada Etapa 1.5: Pesquisa de Tecnologias Adequadas ao Projeto
- ✅ IA deve investigar e recomendar stacks tecnológicos profissionais no início do projeto
- ✅ Baseado em requisitos: tipo de app, funcionalidades, escala, preferências do desenvolvedor
- ✅ 8 categorias cobertas: Frontend, Backend, Desktop, Visualização, IA/ML, BD, Auth, Testes
- ✅ Apresentar 2-3 stacks completos com justificativas, vantagens, casos de uso reais
- ✅ Pesquisas online permitidas (GitHub, docs oficiais, Stack Overflow, Stack Share)
- ✅ Documentação obrigatória da stack escolhida em docs/ARCHITECTURE.md
- ✅ Checklist de 10 itens para validação
- ✅ Rationale: Evita retrabalho, garante qualidade profissional, aumenta produtividade

**Changelog v2.0** (10/12/2025):
- ✅ **[COMPLEMENTAÇÃO]** Adicionada seção "🎯 Quando Usar Simplicidade 1?"
- ✅ Critérios claros: ✅ Quando usar (8 critérios) | ❌ Quando NÃO usar (6 critérios)
- ✅ Migração: Quando evoluir para Simplicidade 2 (equipes) ou 3 (produção solo)
- ✅ Rationale detalhado: Por quê Simplicidade 1 é ágil mas insuficiente para produção
- ✅ Inspiração: Conceitos adaptados do Simplicidade 3 v3.1 (tabelas comparativas, critérios)

**Changelog v1.9** (09/12/2025):
- ✅ **[ETAPA 3]** Adicionada recomendação para IA fornecer sugestões e palpites nas perguntas
- ✅ Formato recomendado: "❓ Pergunta + 💡 Sugestão da IA + Opções A/B/C"
- ✅ Rationale: Acelera decisões, reduz carga cognitiva, mantém consistência com código existente
- ✅ Classificação: **OPCIONAL mas ALTAMENTE RECOMENDADO**

**Changelog v1.8** (02/12/2025):
- ✅ **[REORGANIZAÇÃO]** Revisão de Código integrada nas etapas CLI e GUI
- ✅ Etapa 7: Verificar Implementação CLI (inclui 9 critérios de qualidade)
- ✅ Etapa 8: Verificar Implementação GUI (inclui 9 critérios de qualidade)
- ✅ Etapa 9: Verificar Integração com Programa Principal (mantida como etapa separada)
- ✅ 9 Critérios: Omissão, Ambiguidade, Fato Incorreto, Redundância, Inconsistência, Falta de Integração, Menor Coesão, Maior Acoplamento, Informação Estranha
- ✅ Revisão integrada ao processo de verificação CLI/GUI
- ✅ Total de etapas: 12 → 13 (adicionada verificação de integração após GUI)

**Changelog v1.7** (02/12/2025):
- ✅ **[CRÍTICO]** Adicionada Etapa 8.5: Revisão de Código (ANTES dos testes)
- ✅ 9 Critérios de Qualidade: Omissão, Ambiguidade, Fato Incorreto, Redundância, Inconsistência, Falta de Integração, Menor Coesão, Maior Acoplamento, Informação Estranha
- ✅ Checklist completo de revisão (36 itens de verificação)
- ✅ Ferramentas recomendadas (pylint, vulture, radon, black, isort)
- ✅ Processo de revisão CLI e GUI detalhado
- ✅ Exemplos práticos de problemas e correções
- ✅ Integração com Etapa 9 (testar após revisar)
- ✅ Total de etapas: 12 → 13 (8.5 adicionada entre 8 e 9)

**Changelog v1.6**:
- ✅ **[AVANÇADO]** Adicionada Etapa 9.2: Testes em Threads/Processos com Monitoramento
- ✅ Execução de testes em processo separado (`multiprocessing.Process`)
- ✅ Logging em tempo real via `Queue` (progresso de cada teste)
- ✅ Cancelamento manual a qualquer momento (Ctrl+C gracioso)
- ✅ Timeout global + individual (dupla proteção)
- ✅ Estatísticas em tempo real (passed/failed/elapsed)
- ✅ Implementação completa de `test_runner_monitored.py` (~150 linhas)
- ✅ Checklist adicional opcional (6 itens)

**Changelog v1.5**:
- ✅ **[CRÍTICO]** Adicionada Etapa 9.1: Segurança em Testes
- ✅ 7 soluções obrigatórias para evitar loops infinitos e timeouts
- ✅ Timeout máximo obrigatório (30s por teste)
- ✅ Ambiente headless obrigatório para testes GUI (QT_QPA_PLATFORM=offscreen)
- ✅ Dry-run obrigatório antes de executar testes (syntax + import + collect)
- ✅ Checklist de segurança com 6 itens obrigatórios
- ✅ Regras de ouro e comandos seguros documentados
- ✅ Lições aprendidas de bugs críticos em produção

**Changelog v1.4**:
- ✅ Reorganizada ordem final: Implementar → Integrar GUI → CLI → Testar → Organizar → Documentar → Commit
- ✅ Testes movidos para DEPOIS das verificações de integração (testar sistema integrado)
- ✅ Organizar pasta raiz movido para ANTES da documentação (documentar estado limpo)
- ✅ Lógica: Integrar → Testar integração → Limpar repositório → Documentar estado final

**Changelog v1.3**:
- ✅ Reorganizada ordem das etapas: Verificação de Integração GUI e CLI agora vêm ANTES da Documentação
- ✅ Nova ordem: Testes → Integração GUI → CLI → Documentação → Organizar → Commit
- ✅ Lógica: Verificar integração antes de documentar garante que a documentação reflete o estado real

**Changelog v1.2**:
- ✅ Adicionada Etapa 8: Verificar integração com programa principal
- ✅ Adicionada Etapa 9: Verificar implementação CLI com passagem de parâmetros
- ✅ Total de etapas: 10 → 12

---

## 🎯 Filosofia Central

> "Sempre vão ter tarefas complexas para fazer, mas também aquelas que são mais difíceis e aquelas que são mais fáceis. **Quero que você sempre comece pelas mais fáceis**."

**Princípio**: Do simples ao complexo, incremental, profissional e completo.

---

## ⚠️ Regra de Ouro: Prioridade Absoluta para Erros no Workspace

> **CRÍTICO PARA IAs**: Antes de implementar novas funcionalidades ou continuar com tarefas, **todos os erros no workspace devem ser corrigidos POR VOCÊ (IA)**.

### 🤖 Esta Regra é Para Assistentes de IA

**Se você é uma IA (Cursor, GitHub Copilot, etc.):**
- ✅ **VOCÊ DEVE** corrigir todos os erros existentes ANTES de implementar novas funcionalidades
- ✅ **VOCÊ DEVE** resolver problemas de forma proativa, não esperar que humanos os corrijam
- ✅ **VOCÊ DEVE** tratar a correção de erros como prioridade máxima
- ✅ **VOCÊ DEVE** limpar o workspace antes de adicionar novo código

**Esta regra NÃO significa:**
- ❌ Que desenvolvedores humanos devem parar de implementar quando existem erros
- ❌ Que o projeto não pode avançar enquanto houver erros
- ❌ Que humanos precisam corrigir os erros manualmente

### 🚨 Tipos de Erros que Bloqueiam o Desenvolvimento

Considere a existência de erros no workspace (visíveis na aba "Problemas" do IDE) como **indesejável e bloqueante**. Caso aconteça alguma ocorrência dos seguintes tipos de erro, a **correção é prioridade absoluta** antes de continuar:

1. **❌ Problemas de Sintaxe**
   - Erros de parsing do código
   - Parênteses, chaves ou colchetes não fechados
   - Indentação incorreta (Python)
   - Ponto-e-vírgula faltando (JavaScript, C, Java)

2. **❌ Inconsistências de Código**
   - Variáveis declaradas mas não utilizadas
   - Imports não utilizados ou faltantes
   - Código morto (unreachable code)
   - Type mismatches (TypeScript, Python com type hints)

3. **❌ Omissões Inesperadas**
   - Funções declaradas mas não implementadas
   - Parâmetros obrigatórios faltando
   - Return statements ausentes quando esperados
   - Documentação obrigatória faltando

4. **❌ Fatos Incorretos**
   - Referências a variáveis inexistentes
   - Chamadas de funções com número errado de argumentos
   - Acesso a propriedades inexistentes
   - Imports de módulos inexistentes

5. **❌ Ambiguidades**
   - Warnings de type checking
   - Possíveis null/undefined references
   - Shadowing de variáveis
   - Conversões de tipo implícitas perigosas

6. **❌ Arquivos Faltosos**
   - Dependências não instaladas
   - Módulos importados mas não encontrados
   - Arquivos de configuração ausentes
   - Assets referenciados mas inexistentes

7. **❌ Falhas de Execução**
   - Build failures
   - Compilation errors
   - Testes falhando
   - Linter errors (quando configurado)

### ✅ Quando Pode Continuar

**SOMENTE** continue com o desenvolvimento de novas funcionalidades quando:

- ✅ **Zero erros** na aba "Problemas" do workspace
- ✅ **Todos os builds** completam com sucesso
- ✅ **Todos os testes** passam (se já existentes)
- ✅ **Linter/formatter** não reporta erros críticos
- ✅ **Type checker** não reporta erros (se aplicável)

### 📋 Checklist Antes de Cada Tarefa

```markdown
Antes de iniciar qualquer tarefa nova:

[ ] Verificar aba "Problemas" do IDE (0 erros)
[ ] Executar build do projeto (sucesso)
[ ] Executar testes existentes (todos passando)
[ ] Executar linter/formatter (sem erros críticos)
[ ] Verificar imports e dependências (todas resolvidas)
[ ] Confirmar que código está em estado limpo (commitável)
```

### ⏱️ Tempo Estimado para Correção

- **Erros de Sintaxe**: ~2-5 minutos por erro
- **Imports/Dependências**: ~5-10 minutos
- **Type Errors**: ~5-15 minutos por erro
- **Testes Falhando**: ~10-30 minutos (depende da complexidade)

**Regra Prática**: Se você tem >10 erros no workspace, **dedique 1-2 horas** para limpar tudo antes de prosseguir.

### 🎯 Rationale

**Por quê esta regra é crítica?**

1. **Prevenção de Cascata**: Um erro não corrigido pode gerar 10 novos erros
2. **Qualidade do Código**: Código com erros = dívida técnica imediata
3. **Confiabilidade**: Funcionalidades novas em cima de código quebrado = bugs garantidos
4. **Produtividade**: Corrigir erros antigos + novos é mais demorado que corrigir só os antigos
5. **Profissionalismo**: Código limpo e sem erros é requisito mínimo

**Mensagem para IAs**: 
> "Até que os erros não sejam sanados POR VOCÊ (IA), as tarefas e as funcionalidades não podem continuar sendo implementadas POR VOCÊ (IA). Corrija os erros primeiro, depois continue com a implementação."

---

## 🚫 Hierarquia de Prioridades Bloqueantes

> **CRÍTICO**: Entenda a ordem de prioridades que **BLOQUEIAM** o desenvolvimento até serem resolvidas.

### 📊 Ordem de Prioridade (Do Mais ao Menos Crítico)

```
┌─────────────────────────────────────────────────────────┐
│ 1️⃣ MAIS CRÍTICO: ❓ Dúvidas da IA (veja seção abaixo)  │
│    ↓ DEVE ser resolvido ANTES de continuar              │
├─────────────────────────────────────────────────────────┤
│ 2️⃣ BLOQUEANTE: 📚 Documentação (quando necessária)     │
│    ↓ DEVE ser escrita/atualizada ANTES de implementar   │
├─────────────────────────────────────────────────────────┤
│ 3️⃣ BLOQUEANTE: ❌ Correção de Bugs/Erros               │
│    ↓ DEVE ser corrigido ANTES de novas features         │
├─────────────────────────────────────────────────────────┤
│ 4️⃣ NORMAL: ✨ Implementação de Novas Features          │
│    Somente após 1, 2 e 3 estarem resolvidos             │
└─────────────────────────────────────────────────────────┘
```

### 🎯 Significado de "Bloqueante"

**Bloqueante** significa que:
- 🚫 **IMPEDE** continuar com outras tarefas
- 🚫 **OBRIGA** a parar e resolver IMEDIATAMENTE
- 🚫 **NÃO PERMITE** pular ou adiar
- 🚫 **EXIGE** resolução completa antes de prosseguir

### 1️⃣ Prioridade Máxima: ❓ Dúvidas da IA

**Quando**: Sempre que a IA tiver qualquer dúvida sobre requisitos, arquitetura, decisões técnicas

**Ação Obrigatória**:
- ✅ **PARAR** imediatamente
- ✅ **FORMULAR** perguntas claras
- ✅ **AGUARDAR** respostas do desenvolvedor
- ❌ **NÃO ASSUMIR** nada sem confirmar

**Rationale**: Implementar com dúvidas = garantia de retrabalho

### 2️⃣ Bloqueante: 📚 Documentação (Quando Necessária)

> **NOVO REQUISITO CRÍTICO**: Documentação é **BLOQUEANTE** quando há necessidade de documentar.

**Quando é necessário documentar** (bloqueante):

1. **🆕 Antes de implementar feature nova**:
   - Se a feature altera comportamento existente → Documentar ANTES
   - Se adiciona nova API/interface pública → Documentar ANTES
   - Se muda fluxo do usuário → Documentar ANTES

2. **🔄 Durante alterações arquiteturais**:
   - Mudanças em estrutura de pastas → Atualizar docs ANTES
   - Novos módulos/componentes → Documentar ANTES
   - Alterações em dependências → Atualizar docs ANTES

3. **🐛 Após correção de bugs críticos**:
   - Se bug afetou comportamento documentado → Atualizar docs IMEDIATAMENTE
   - Se workaround foi documentado → Remover workaround da doc

4. **📝 Quando documentação está desatualizada**:
   - Se README não reflete estado atual → Atualizar BLOQUEANTE
   - Se API docs estão incorretas → Corrigir BLOQUEANTE
   - Se guias de instalação falharam → Atualizar BLOQUEANTE

**O que documentar** (bloqueante):

| Item | Onde | Quando é Bloqueante |
|------|------|---------------------|
| **API pública** | docs/API.md | ✅ ANTES de implementar |
| **Arquitetura** | docs/ARCHITECTURE.md | ✅ ANTES de mudar estrutura |
| **Requisitos** | docs/REQUIREMENTS.md | ✅ ANTES de implementar features |
| **Instalação** | README.md | ✅ ANTES de adicionar dependências |
| **Uso básico** | README.md | ✅ ANTES de release |
| **Changelog** | CHANGELOG.md | ✅ ANTES de commit |
| **Breaking changes** | CHANGELOG.md | ✅ IMEDIATAMENTE |

**Ação Obrigatória**:
- ✅ **PARAR** implementação se documentação está pendente
- ✅ **ESCREVER/ATUALIZAR** documentação necessária
- ✅ **VALIDAR** que documentação está correta e completa
- ✅ **COMMITAR** documentação junto com código (ou antes)
- ❌ **NÃO IMPLEMENTAR** sem documentar primeiro

**Exemplo de fluxo bloqueante**:
```
Desenvolvedor pede: "Adicionar endpoint /api/users"

❌ ERRADO:
1. Implementar endpoint
2. Testar endpoint
3. (Esquecer de documentar)
4. Commit

✅ CORRETO:
1. 📚 Documentar API em docs/API.md (BLOQUEANTE)
   - Endpoint: POST /api/users
   - Body: { name, email }
   - Response: { id, name, email, created_at }
   - Errors: 400, 409, 500
2. Implementar endpoint conforme documentação
3. Testar endpoint
4. Atualizar CHANGELOG.md
5. Commit (código + docs juntos)
```

**Quando documentação NÃO é bloqueante** (pode vir depois):
- ⚠️ Comentários internos no código (escrever junto, mas não bloqueia)
- ⚠️ Docs de desenvolvimento (guides, tutorials) - pode vir depois
- ⚠️ Refinamentos de exemplos - pode melhorar depois
- ⚠️ Tradução de docs - pode vir depois

**Rationale**:
1. **Documentação desatualizada = mentira**: Pior que não ter docs
2. **Previne confusão**: Implementar sem docs = outros não entendem
3. **Design thinking**: Documentar ANTES força pensar na interface
4. **Qualidade**: Se não consegue documentar, design está ruim
5. **Manutenibilidade**: Docs atualizados = código mais fácil de manter

**Mensagem para IAs**:
> "Se há necessidade de documentar algo (API, arquitetura, breaking change, requisitos), a documentação é **BLOQUEANTE**. Você NÃO PODE implementar até documentar. Documente ANTES de codificar. Documentação desatualizada é pior que código ruim."

### 3️⃣ Bloqueante: ❌ Correção de Bugs/Erros

**Quando**: Existem erros no workspace, builds falhando, testes falhando

**Ação Obrigatória**:
- ✅ **CORRIGIR** todos os erros ANTES de novas features
- ✅ **LIMPAR** workspace (0 erros)
- ✅ **VALIDAR** que builds e testes passam
- ❌ **NÃO ADICIONAR** código novo em cima de código quebrado

**Rationale**: Código quebrado + código novo = mais código quebrado

### 4️⃣ Normal: ✨ Novas Features

**Quando**: Após 1, 2 e 3 estarem 100% resolvidos

**Ação**:
- ✅ Implementar features incrementalmente
- ✅ Seguir protocolo do simples ao complexo
- ✅ Testar cada parte antes de avançar

### 🔄 Fluxo Completo

```
Tarefa solicitada
    ↓
1. Tenho dúvidas? → SIM → ❓ PERGUNTAR (BLOQUEANTE) → Aguardar resposta
    ↓ NÃO
2. Precisa documentar? → SIM → 📚 DOCUMENTAR (BLOQUEANTE) → Escrever/atualizar
    ↓ NÃO
3. Há erros no workspace? → SIM → ❌ CORRIGIR (BLOQUEANTE) → Limpar tudo
    ↓ NÃO
4. ✨ IMPLEMENTAR FEATURE (NORMAL) → Codificar → Testar → Commit
```

### 📋 Checklist de Desbloqueio

Antes de implementar qualquer feature, confirme:

```markdown
[ ] 1️⃣ Zero dúvidas sobre a tarefa (perguntas respondidas)
[ ] 2️⃣ Documentação necessária está escrita/atualizada
[ ] 3️⃣ Zero erros no workspace (0 problemas)
[ ] 3️⃣ Builds passando (sem compilation errors)
[ ] 3️⃣ Testes passando (se existentes)
[ ] ✅ DESBLOQUEADO: Pode implementar feature
```

**Regra de Ouro**:
> "Dúvidas → Documentação → Bugs → Features. Nesta ordem. Sempre."

---

## ❓ Regra Obrigatória: Perguntas Bloqueantes para Dúvidas

> **CRÍTICO PARA IAs**: Sempre que a inteligência artificial estiver com alguma pergunta ou dúvida sobre alguma tarefa que essa inteligência artificial deve fazer, é **OBRIGATÓRIO** que essa IA faça perguntas sobre a tarefa correspondente que se deve fazer.

### 🚫 Dúvidas São Bloqueantes

**Regra Fundamental**:
> **A dúvida sobre a tarefa é BLOQUEANTE.**
>
> A inteligência artificial **NÃO PODE CONTINUAR** até sanar **TODAS as suas dúvidas** sobre o que a mesma deve fazer.

### 🤖 Esta Regra é Para Assistentes de IA

**Se você é uma IA (Cursor, GitHub Copilot, etc.):**

#### ✅ VOCÊ DEVE:
- ✅ **PARAR imediatamente** ao identificar qualquer dúvida sobre a tarefa
- ✅ **FORMULAR perguntas claras** sobre todos os pontos de incerteza
- ✅ **AGUARDAR respostas** do programador antes de continuar
- ✅ **VALIDAR seu entendimento** fazendo perguntas confirmatórias
- ✅ **ESCLARECER requisitos ambíguos** antes de implementar
- ✅ **QUESTIONAR premissas** que não foram explicitamente confirmadas
- ✅ **PERGUNTAR sobre edge cases** e comportamentos esperados

#### ❌ VOCÊ NÃO DEVE:
- ❌ **Assumir ou adivinhar** o que o programador quer
- ❌ **Prosseguir com incertezas** não resolvidas
- ❌ **Implementar baseado em suposições** não confirmadas
- ❌ **Ignorar ambiguidades** na especificação
- ❌ **Tomar decisões críticas** sem consultar o programador
- ❌ **Continuar silenciosamente** quando não entender algo

### 🎯 Tipos de Dúvidas que São Bloqueantes

#### 1. **Dúvidas sobre Requisitos**
```markdown
❓ Exemplos de perguntas obrigatórias:
- "Qual deve ser o comportamento quando o usuário inserir valor negativo?"
- "A funcionalidade deve validar email em tempo real ou apenas ao submeter?"
- "Qual a prioridade entre performance e precisão neste cálculo?"
- "Devo implementar cache para esta operação?"
```

#### 2. **Dúvidas sobre Arquitetura**
```markdown
❓ Exemplos de perguntas obrigatórias:
- "Devo criar um novo módulo ou adicionar ao módulo X existente?"
- "Esta lógica pertence ao CORE, CLI ou GUI?"
- "Devo usar herança ou composição para esta funcionalidade?"
- "Qual o padrão de design mais apropriado aqui?"
```

#### 3. **Dúvidas sobre Integração**
```markdown
❓ Exemplos de perguntas obrigatórias:
- "Esta funcionalidade deve se integrar com o módulo Y existente?"
- "Devo modificar a API pública ou criar uma nova?"
- "Como esta feature se relaciona com a funcionalidade X já implementada?"
- "Preciso manter compatibilidade com versões anteriores?"
```

#### 4. **Dúvidas sobre Dados**
```markdown
❓ Exemplos de perguntas obrigatórias:
- "Qual o formato esperado dos dados de entrada?"
- "Qual o range válido para este parâmetro?"
- "Como devo lidar com dados ausentes ou inválidos?"
- "Qual o encoding esperado para arquivos de texto?"
```

#### 5. **Dúvidas sobre Comportamento**
```markdown
❓ Exemplos de perguntas obrigatórias:
- "O que deve acontecer se a operação falhar?"
- "Devo fazer rollback ou logging em caso de erro?"
- "Como notificar o usuário sobre erros?"
- "Qual o timeout aceitável para esta operação?"
```

#### 6. **Dúvidas sobre Testes**
```markdown
❓ Exemplos de perguntas obrigatórias:
- "Quais edge cases específicos devo testar?"
- "Qual o critério de aceitação para esta funcionalidade?"
- "Devo mockar dependências externas nos testes?"
- "Qual a cobertura de testes esperada?"
```

### 📋 Processo de Esclarecimento de Dúvidas

#### Passo 1: Identificar Dúvidas
```markdown
Antes de iniciar qualquer tarefa:

[ ] Ler especificação completa da tarefa
[ ] Identificar TODOS os pontos de incerteza
[ ] Listar TODAS as perguntas necessárias
[ ] Classificar dúvidas por tipo (requisitos, arquitetura, etc.)
```

#### Passo 2: Formular Perguntas Claras
```markdown
Características de boas perguntas:

✅ Específicas: "Qual o comportamento esperado quando X?"
✅ Objetivas: Permitem resposta clara (sim/não ou descrição concreta)
✅ Contextualizadas: Incluem informação relevante
✅ Priorizadas: Mais críticas primeiro

❌ Evitar perguntas vagas: "Como devo fazer isso?"
❌ Evitar múltiplas perguntas em uma: Separar em perguntas individuais
```

**Exemplo de Perguntas Bem Formuladas**:
```markdown
Tenho as seguintes dúvidas sobre a tarefa "Implementar validação de CPF":

1. **Validação de Formato**:
   ❓ Devo aceitar CPF com pontuação (XXX.XXX.XXX-XX) ou apenas números?
   💡 Sugestão: Aceitar ambos e normalizar internamente
   
2. **Validação de Dígitos Verificadores**:
   ❓ Devo validar os dígitos verificadores ou apenas o formato?
   💡 Sugestão: Validar dígitos para garantir CPF válido
   
3. **Tratamento de Erros**:
   ❓ Como devo notificar o usuário de CPF inválido?
   A) Retornar None
   B) Levantar ValueError
   C) Retornar tupla (bool, mensagem)
   💡 Sugestão: Opção B (ValueError) seguindo padrão Python

4. **Casos Especiais**:
   ❓ CPFs com todos dígitos iguais (ex: 111.111.111-11) devem ser rejeitados?
   💡 Sugestão: Sim, pois são inválidos na prática
```

#### Passo 3: Aguardar Confirmação
```markdown
Ação da IA:

🛑 PARAR toda implementação
📝 APRESENTAR lista de perguntas ao programador
⏳ AGUARDAR respostas completas
✅ CONFIRMAR entendimento antes de prosseguir
```

#### Passo 4: Validar Entendimento
```markdown
Após receber respostas:

[ ] Repetir entendimento: "Então, devo fazer X e Y, correto?"
[ ] Confirmar casos especiais: "No caso Z, devo fazer W?"
[ ] Esclarecer ambiguidades restantes
[ ] Obter aprovação explícita: "Posso prosseguir com este entendimento?"
```

### 🎯 Exemplos Práticos

#### Exemplo 1: Tarefa com Requisitos Ambíguos

**Tarefa Recebida**: "Implementar cálculo de desconto"

**❌ ERRADO (IA assume e implementa)**:
```python
# IA assume 10% de desconto sem perguntar
def calculate_discount(price):
    return price * 0.9
```

**✅ CORRETO (IA faz perguntas primeiro)**:
```markdown
Antes de implementar "Cálculo de desconto", preciso esclarecer:

1. **Porcentagem do Desconto**:
   ❓ Qual a porcentagem de desconto a ser aplicada?
   💡 Sugestão: 10% como padrão, mas configurável?

2. **Regras de Aplicação**:
   ❓ O desconto se aplica a todos os produtos ou há condições?
   A) Todos os produtos
   B) Apenas produtos em promoção
   C) Baseado em valor mínimo do pedido
   💡 Sugestão: Opção C (valor mínimo R$ 100)

3. **Tipo de Desconto**:
   ❓ Desconto percentual ou valor fixo?
   💡 Sugestão: Percentual para flexibilidade

4. **Acumulação**:
   ❓ Descontos podem ser acumulados com outras promoções?
   💡 Sugestão: Não, aplicar apenas o maior desconto

Aguardo confirmação para prosseguir com a implementação.
```

#### Exemplo 2: Tarefa com Detalhes Técnicos Ausentes

**Tarefa Recebida**: "Adicionar suporte a export de relatórios"

**❌ ERRADO (IA assume formato)**:
```python
# IA assume PDF sem perguntar
def export_report(data):
    generate_pdf(data)
```

**✅ CORRETO (IA esclarece detalhes)**:
```markdown
Preciso de esclarecimentos sobre "Export de relatórios":

1. **Formatos de Exportação**:
   ❓ Quais formatos devo suportar?
   A) PDF apenas
   B) PDF + Excel
   C) PDF + Excel + CSV
   💡 Sugestão: Opção B (PDF para visualização, Excel para análise)

2. **Template/Layout**:
   ❓ Existe um template específico para os relatórios?
   💡 Sugestão: Usar template da empresa se existir, senão criar padrão

3. **Geração Assíncrona**:
   ❓ Relatórios grandes devem ser gerados em background?
   💡 Sugestão: Sim, com notificação quando concluído (>1000 registros)

4. **Localização**:
   ❓ Onde os arquivos gerados devem ser salvos?
   A) Pasta temporária do sistema
   B) Downloads do usuário
   C) Configurável pelo usuário
   💡 Sugestão: Opção C (configurável com default em Downloads)

5. **Nome do Arquivo**:
   ❓ Qual o padrão de nomenclatura?
   💡 Sugestão: "relatorio_YYYY-MM-DD_HHmmss.ext"

Aguardo definições para implementar corretamente.
```

### ✅ Checklist de Perguntas Obrigatórias

**Antes de iniciar QUALQUER tarefa**:

```markdown
[ ] 1. Requisitos Funcionais Claros?
   - [ ] Entendo o QUE deve ser feito?
   - [ ] Entendo o PORQUÊ desta funcionalidade?
   - [ ] Conheço os critérios de aceitação?

[ ] 2. Requisitos Técnicos Definidos?
   - [ ] Sei COMO implementar (arquitetura)?
   - [ ] Conheço as tecnologias/bibliotecas a usar?
   - [ ] Entendo as restrições técnicas?

[ ] 3. Casos de Uso Cobertos?
   - [ ] Sei o fluxo normal de uso?
   - [ ] Conheço os edge cases?
   - [ ] Sei como lidar com erros?

[ ] 4. Integração Clara?
   - [ ] Sei como integrar com código existente?
   - [ ] Conheço as dependências?
   - [ ] Entendo o impacto em outras partes?

[ ] 5. Validação Definida?
   - [ ] Sei como testar a funcionalidade?
   - [ ] Conheço os cenários de teste?
   - [ ] Entendo a cobertura esperada?

Se QUALQUER item acima for ❌ NÃO: PARAR e fazer perguntas!
```

### 🚨 Consequências de NÃO Fazer Perguntas

**O que acontece quando IA assume ao invés de perguntar**:

1. **❌ Implementação Incorreta**
   - Funcionalidade não atende requisitos reais
   - Retrabalho necessário (perda de tempo)
   - Frustração do programador

2. **❌ Bugs Introduzidos**
   - Comportamento inesperado
   - Edge cases não tratados
   - Problemas em produção

3. **❌ Arquitetura Inadequada**
   - Código difícil de manter
   - Violação de padrões do projeto
   - Dívida técnica acumulada

4. **❌ Perda de Confiança**
   - Programador deixa de confiar na IA
   - Necessidade de revisão manual de tudo
   - Redução de produtividade

### 🎯 Benefícios de Fazer Perguntas

**O que se ganha ao esclarecer dúvidas antes de implementar**:

1. **✅ Implementação Correta na Primeira Tentativa**
   - Zero retrabalho
   - Economia de tempo
   - Qualidade alta

2. **✅ Alinhamento com Expectativas**
   - Código atende exatamente o que foi pedido
   - Programador satisfeito
   - Confiança na IA aumenta

3. **✅ Arquitetura Adequada**
   - Código segue padrões do projeto
   - Fácil de manter e evoluir
   - Integração suave com código existente

4. **✅ Prevenção de Bugs**
   - Edge cases identificados e tratados
   - Validações apropriadas implementadas
   - Código robusto desde o início

### 📊 Métricas de Sucesso

**Indicadores de que a IA está fazendo perguntas corretamente**:

- ✅ **Taxa de retrabalho < 10%**: Implementações corretas na primeira tentativa
- ✅ **Tempo de esclarecimento < 20%**: Perguntas não atrasam significativamente
- ✅ **Satisfação do programador alta**: Código atende expectativas
- ✅ **Bugs pós-implementação baixos**: < 1 bug por 10 funcionalidades
- ✅ **Commits limpos**: Menos commits de correção após inicial

### 🎓 Conclusão

> **"É melhor gastar 5 minutos esclarecendo dúvidas do que 2 horas corrigindo implementação incorreta."**

**Mensagem para IAs**:
> "NUNCA assuma. SEMPRE pergunte quando houver a menor dúvida. Sua função é implementar CORRETAMENTE, não rapidamente. Perguntas são um sinal de profissionalismo, não de incapacidade. O programador prefere responder 10 perguntas agora do que revisar 100 linhas de código errado depois."

**Regra de Ouro para IAs**:
> **"Quando em dúvida, PARE e PERGUNTE. Dúvida é BLOQUEANTE até ser resolvida."**

---

## 🔍 Busca Binária para Localização de Defeitos

> **IMPORTANTE PARA IAs**: Quando estiver lidando com correção de erros e eliminação de bugs, lembre-se de que existe a possibilidade de utilizar **busca binária** para localizar defeitos de maneira eficiente.

### 🎯 Conceito Central

A busca binária é uma técnica poderosa que reduz o espaço de busca pela metade a cada iteração, permitindo localizar defeitos em **O(log N) passos**, onde N é o número de linhas, comandos ou instruções do algoritmo.

**Exemplo Prático**: 
- Se um erro está na linha 48 de um arquivo com 512 linhas
- Busca linear: até 512 verificações
- Busca binária: apenas **9 verificações** (log₂(512) = 9)

### 📋 Metodologia de Busca Binária para Debugging

#### **1️⃣ Passo Inicial: Dividir o Código ao Meio**

Começando com um arquivo de N linhas onde existe um erro:
1. Comente metade do código (ex: linhas 257-512)
2. Execute/teste a metade restante (linhas 1-256)
3. Verifique se o erro persiste

**Decisão**:
- ✅ **Erro persiste**: O bug está na metade ativa (1-256)
- ❌ **Erro desaparece**: O bug está na metade comentada (257-512)

#### **2️⃣ Recursão: Continue Dividindo**

Uma vez identificada a metade com o problema, repita o processo:

**Iteração 2** (erro em 1-256):
- Comente linhas 129-256
- Teste linhas 1-128
- Identifique qual quarto contém o bug

**Iteração 3** (erro em 1-128):
- Comente linhas 65-128
- Teste linhas 1-64
- Identifique qual oitavo contém o bug

**Continue até** localizar exatamente a linha/bloco problemático.

#### **3️⃣ Exemplo Completo: 512 Linhas → Linha 48**

```
Iteração 1: [1-512]   → Testar [1-256]   ✅ Erro presente
Iteração 2: [1-256]   → Testar [1-128]   ✅ Erro presente  
Iteração 3: [1-128]   → Testar [1-64]    ✅ Erro presente
Iteração 4: [1-64]    → Testar [1-32]    ❌ Erro ausente → Bug em [33-64]
Iteração 5: [33-64]   → Testar [33-48]   ✅ Erro presente
Iteração 6: [33-48]   → Testar [33-40]   ✅ Erro presente
Iteração 7: [41-48]   → Testar [41-44]   ✅ Erro presente
Iteração 8: [45-48]   → Testar [45-46]   ✅ Erro presente
Iteração 9: [47-48]   → Testar [linha 47] ❌ Erro ausente → ✅ Bug na linha 48!
```

**Resultado**: 9 iterações para encontrar o bug em 512 linhas (vs. até 512 tentativas lineares).

### 🛠️ Técnicas de Implementação

#### **A) Comentários Temporários**
```python
# BUSCA BINÁRIA - Iteração 1: Testando [1-256]
# Linhas 257-512 temporariamente desabilitadas
# def funcao_suspeita():  
#     codigo_potencialmente_bugado()
#     mais_codigo()
```

#### **B) Flags de Debug**
```python
DEBUG_BINARY_SEARCH = True
RANGE_START = 1
RANGE_END = 256

if DEBUG_BINARY_SEARCH and not (RANGE_START <= current_line <= RANGE_END):
    return  # Pular execução fora do range de teste
```

#### **C) Git Bisect** (para bugs introduzidos em commits)
```bash
# Usar git bisect para encontrar commit que introduziu o bug
git bisect start
git bisect bad HEAD              # Commit atual tem bug
git bisect good v1.0.0           # Commit v1.0.0 não tinha bug
# Git automaticamente faz busca binária nos commits
```

#### **D) Testes Unitários Particionados**
```python
# Dividir suite de testes ao meio
pytest tests/test_module_part1.py  # Primeira metade
pytest tests/test_module_part2.py  # Segunda metade
# Identificar qual metade contém teste falhando
```

### 🎨 Aplicações Criativas da Busca Binária

A busca binária não se limita a linhas de código. Pode ser aplicada a:

1. **📦 Dependências/Imports**:
   - Comente metade dos imports
   - Identifique qual import causa conflito/erro
   
2. **🔧 Parâmetros de Configuração**:
   - Desabilite metade das configurações
   - Encontre configuração problemática

3. **🗃️ Dados de Entrada**:
   - Processe metade do dataset
   - Identifique qual subset causa erro

4. **⚙️ Features/Funcionalidades**:
   - Desabilite metade das features
   - Localize feature que causa regressão

5. **🧩 Módulos/Componentes**:
   - Desabilite metade dos módulos
   - Encontre módulo com bug

6. **📅 Histórico de Versões** (Git Bisect):
   - Teste versão no meio do histórico
   - Encontre commit que introduziu bug

7. **🔄 Iterações de Loop**:
   - Execute metade das iterações
   - Identifique em qual iteração erro ocorre

### ✅ Checklist de Busca Binária para Debugging

```markdown
[ ] 1. Confirmar que erro é reproduzível consistentemente
[ ] 2. Identificar escopo total (N linhas/módulos/commits)
[ ] 3. Calcular número de iterações necessárias: log₂(N)
[ ] 4. Criar backup ou branch de testes
[ ] 5. Iteração 1: Comentar/desabilitar metade superior/inferior
[ ] 6. Executar teste e verificar se erro persiste
[ ] 7. Anotar resultado e reduzir escopo pela metade
[ ] 8. Repetir até isolar linha/bloco/commit exato
[ ] 9. Analisar código isolado para entender causa raiz
[ ] 10. Aplicar correção e validar com testes
[ ] 11. Remover código de debug/comentários temporários
```

### 🎯 Quando Usar Busca Binária para Debugging

**✅ Use quando:**
- Erro é reproduzível mas causa não é óbvia
- Codebase grande (>100 linhas)
- Suspeita de que bug está em região específica mas ampla
- Erro apareceu após mudanças grandes (múltiplos commits)
- Teste falha mas não há indicação clara do problema
- Performance degradou mas não sabe qual função é responsável

**❌ Não use quando:**
- Erro é esporádico/não reproduzível (race condition, timing issue)
- Stack trace já aponta linha exata do problema
- Código é muito pequeno (<50 linhas)
- Bug é óbvio após leitura rápida do código

### ⏱️ Eficiência da Busca Binária

| Tamanho (N) | Busca Linear | Busca Binária | Ganho |
|------------|--------------|---------------|-------|
| 32 linhas  | até 32 passos | 5 passos | 6.4x mais rápido |
| 128 linhas | até 128 passos | 7 passos | 18.3x mais rápido |
| 512 linhas | até 512 passos | 9 passos | 56.9x mais rápido |
| 1024 linhas | até 1024 passos | 10 passos | 102.4x mais rápido |
| 4096 linhas | até 4096 passos | 12 passos | 341.3x mais rápido |

### 💡 Dicas Práticas

1. **Documente o Processo**: Anote cada iteração e resultado
2. **Use Controle de Versão**: Crie branches para cada teste
3. **Automatize Quando Possível**: Scripts para comentar/descomentar blocos
4. **Combine com Logs**: Adicione prints para confirmar execução de blocos
5. **Teste Isoladamente**: Garanta que o teste é determinístico
6. **Valide Antes e Depois**: Confirme que bug existe antes e foi corrigido depois

### 🚀 Rationale

**Por quê a busca binária é poderosa para debugging?**

1. **⚡ Eficiência Algorítmica**: O(log N) vs O(N) - economia exponencial de tempo
2. **🎯 Isolamento Preciso**: Reduz incerteza sistematicamente
3. **🧠 Menor Carga Cognitiva**: Decisões simples (erro presente: sim/não)
4. **📊 Previsibilidade**: Sabe exatamente quantos passos serão necessários
5. **🔄 Aplicabilidade Universal**: Funciona para código, dados, configurações, histórico
6. **✅ Garantia de Sucesso**: Se o bug é reproduzível, a busca binária sempre encontra

**Mensagem para IAs**:
> "A criatividade no uso de busca binária não tem limites. Sempre considere se um problema de debugging pode ser reduzido a uma busca binária - você economizará tempo e encontrará bugs mais rapidamente."

---

## 🧠 Fator de Memória Associativa

> **IMPORTANTE PARA IAs**: Durante investigação e correção de erros, aplique o **Fator de Memória Associativa** para aprender com padrões passados e acelerar diagnósticos futuros.

**Versão:** 1.0  
**Data:** 2025-12-28

### 🎯 Visão Geral

O **Fator de Memória Associativa** é um conceito fundamental que integra os Protocolos Simplicidade, permitindo que a inteligência artificial aprenda com padrões de erros passados e aplique esse conhecimento na investigação e correção de defeitos futuros.

#### 🔍 O Que é Memória Associativa?

Memória associativa é a capacidade de:
- ✅ **Reconhecer padrões** recorrentes em erros e defeitos
- ✅ **Associar causas e efeitos** específicos em diferentes contextos
- ✅ **Generalizar soluções** a partir de casos específicos
- ✅ **Deduzir problemas** do geral para o específico
- ✅ **Induzir regras** do específico para o geral

#### 🎯 Objetivo

Permitir que a IA desenvolva uma "memória" de problemas e soluções, criando associações entre:
- Tipos de erro e suas causas raiz
- Sintomas observados e diagnósticos precisos
- Contextos de projeto e padrões de defeito
- Soluções aplicadas e sua eficácia

---

### 🐍 Conexão com Python Traceback

#### 📊 Como o Traceback Funciona

O Traceback do Python apresenta erros em uma estrutura **top-down** (de cima para baixo, ou de fora para dentro):

```python
Traceback (most recent call last):
  File "main.py", line 10, in <module>          # ← RAIZ (Orquestrador)
    processar_dados()
  File "processador.py", line 45, in processar_dados  # ← GALHO (Coordenador)
    validar_entrada(dados)
  File "validador.py", line 23, in validar_entrada    # ← FOLHA (Executor)
    assert len(dados) > 0                             # ← ERRO ESPECÍFICO
AssertionError: lista vazia
```

#### 🎯 Metodologia Top-Down de Investigação

**Nível 1: Orquestrador (main.py)**
- Onde o erro foi **disparado**?
- Qual o **contexto** de execução?
- Quais **dados** foram passados?

**Nível 2: Coordenador (processador.py)**
- Como os dados foram **transformados**?
- Qual **lógica de negócio** foi aplicada?
- Houve **validações intermediárias**?

**Nível 3: Executor (validador.py)**
- Qual **operação específica** falhou?
- Qual **pré-condição** foi violada?
- Qual a **causa raiz** técnica?

#### 🧠 Associação com Memória

A IA deve **lembrar** e **associar**:
- **Padrão observado**: `AssertionError` em validação de entrada
- **Causa comum**: Dados vazios não tratados em nível superior
- **Solução típica**: Adicionar verificação antes de chamar `validar_entrada()`
- **Prevenção futura**: Sempre validar lista não-vazia antes de processar

#### 🔄 Analogia com Árvore de Importações

A estrutura de Traceback espelha a Árvore de Importações:

```
main.py (RAIZ)
  └─ processador.py (GALHO)
       └─ validador.py (FOLHA) ← Erro aqui!
```

**Insight de Memória Associativa**:
- Erros em **folhas** geralmente indicam **pré-condições violadas**
- Erros em **galhos** geralmente indicam **lógica de coordenação incorreta**
- Erros na **raiz** geralmente indicam **integração ou orquestração problemática**

---

### 🔬 Abordagens Dedutiva e Indutiva

#### 📉 Abordagem Dedutiva (Geral → Específico)

**Conceito**: Partir de uma regra geral para identificar casos específicos.

**Exemplo Prático**:

**Regra Geral**: "Erros de `AttributeError` geralmente indicam que um objeto não foi inicializado corretamente"

**Aplicação Específica**:
```python
# Erro observado
AttributeError: 'NoneType' object has no attribute 'process'

# Dedução:
1. ✅ Regra geral: AttributeError → objeto não inicializado
2. ✅ Hipótese: variável retornou None ao invés de objeto
3. ✅ Investigação: verificar métodos que retornam o objeto
4. ✅ Solução: adicionar verificação de None ou corrigir inicialização
```

**Fluxo Dedutivo**:
```
Teoria Geral (conhecimento prévio)
         ↓
Hipótese Específica (baseada no erro)
         ↓
Teste da Hipótese (debugging)
         ↓
Confirmação/Refutação
```

#### 📈 Abordagem Indutiva (Específico → Geral)

**Conceito**: Observar casos específicos repetidos para criar uma regra geral.

**Exemplo Prático**:

**Observação 1**:
```python
# Projeto A
IndexError: list index out of range
# Causa: loop usando range(len(lista) + 1)
```

**Observação 2**:
```python
# Projeto B  
IndexError: list index out of range
# Causa: acesso a lista[i] sem verificar len(lista)
```

**Observação 3**:
```python
# Projeto C
IndexError: list index out of range
# Causa: iteração manual com índice incrementado incorretamente
```

**Indução (Regra Geral)**:
> "70% dos `IndexError` são causados por manipulação manual incorreta de índices.  
> **Solução preventiva**: Sempre preferir iteradores (`for item in lista`) ao invés de índices manuais."

**Fluxo Indutivo**:
```
Caso Específico 1
      +
Caso Específico 2
      +
Caso Específico 3
      ↓
Padrão Identificado
      ↓
Regra Geral (nova memória associativa)
      ↓
Aplicação Preventiva em Projetos Futuros
```

#### 🔄 Combinação Dedutiva-Indutiva (Neuro-Simbólica)

**Ciclo Completo de Aprendizado**:

1. **Dedutivo**: Aplicar regras gerais existentes para diagnosticar erro atual
2. **Validação**: Confirmar ou refutar a hipótese dedutiva
3. **Indutivo**: Se padrão novo é observado, adicionar à base de conhecimento
4. **Refinamento**: Atualizar regras gerais com novos casos específicos

**Exemplo de Ciclo**:
```
[Dedutivo] Regra: "TypeError geralmente indica tipo incompatível"
           ↓
[Aplicação] Erro: TypeError ao somar string + int
           ↓
[Validação] ✅ Confirmado: tentativa de soma incompatível
           ↓
[Indutivo] Novo padrão: "TypeError com '+' → verificar tipos antes de operação"
           ↓
[Memória] Armazenar: "Sempre validar tipos antes de operações matemáticas"
```

---

### 🐛 Taxonomia de Defeitos de Software

A taxonomia de defeitos de software identifica cinco categorias principais de problemas altamente indesejáveis e inesperados:

#### 1️⃣ Fato Incorreto

**Definição**: Informação no código que está errada ou desatualizada.

**Exemplos**:
```python
# ❌ Fato incorreto
PI = 3.14  # Valor impreciso

# ✅ Correção
PI = 3.14159265359  # Valor correto com precisão adequada
```

```python
# ❌ Fato incorreto  
MAX_UPLOAD_SIZE = 5 * 1024  # Comentário diz "5MB" mas código é 5KB

# ✅ Correção
MAX_UPLOAD_SIZE = 5 * 1024 * 1024  # 5MB correto
```

**Memória Associativa**:
- Sempre validar **constantes numéricas** contra requisitos
- Revisar **comentários** para garantir alinhamento com código
- Usar **testes de limites** para valores críticos

#### 2️⃣ Informação Estranha

**Definição**: Código, comentários ou lógica que não pertence ao contexto atual.

**Exemplos**:
```python
# ❌ Informação estranha
def calcular_preco(valor):
    # TODO: implementar desconto para clientes VIP
    # print("DEBUG: valor =", valor)  # Código de debug esquecido
    # import random  # Import não utilizado
    resultado = valor * 1.1
    return resultado
```

```python
# ✅ Correção
def calcular_preco(valor):
    """Calcula preço com taxa de 10%."""
    resultado = valor * 1.1
    return resultado
```

**Memória Associativa**:
- Remover **código comentado** não utilizado
- Eliminar **imports desnecessários** (use linter)
- Limpar **TODOs** concluídos ou movê-los para sistema de tarefas

#### 3️⃣ Ambiguidade

**Definição**: Código ou documentação que pode ser interpretado de múltiplas formas.

**Exemplos**:
```python
# ❌ Ambíguo
def processar(dados):
    """Processa os dados."""  # O que significa "processar"?
    return dados
```

```python
# ✅ Específico
def normalizar_e_validar_entrada_usuario(dados_brutos):
    """
    Normaliza entrada do usuário (lowercase, trim) e valida formato de email.
    
    Args:
        dados_brutos: String com email fornecido pelo usuário
        
    Returns:
        String com email normalizado e validado
        
    Raises:
        ValueError: Se formato de email é inválido
    """
    email_normalizado = dados_brutos.strip().lower()
    if "@" not in email_normalizado:
        raise ValueError("Email inválido: falta '@'")
    return email_normalizado
```

**Memória Associativa**:
- Usar **nomes descritivos** que explicam intenção
- Adicionar **docstrings detalhadas** com Args/Returns/Raises
- Incluir **exemplos de uso** na documentação
- Preferir **especificidade** sobre brevidade

#### 4️⃣ Inconsistência

**Definição**: Violação de padrões ou convenções estabelecidas no projeto.

**Exemplos**:
```python
# ❌ Inconsistente
def calcular_total(preco):  # snake_case
    return preco * 1.1

def CalcularDesconto(preco):  # PascalCase - INCONSISTENTE!
    return preco * 0.9

def calcPreco(valor):  # camelCase - INCONSISTENTE!
    return valor
```

```python
# ✅ Consistente
def calcular_total(preco):  # snake_case
    return preco * 1.1

def calcular_desconto(preco):  # snake_case
    return preco * 0.9

def calcular_preco_final(valor):  # snake_case
    return valor
```

**Mais Exemplos de Inconsistência**:
```python
# ❌ Ordem de parâmetros inconsistente
def enviar_email(destinatario, assunto, corpo): pass
def enviar_sms(corpo, numero): pass  # Ordem diferente!

# ✅ Ordem consistente
def enviar_email(destinatario, assunto, corpo): pass
def enviar_sms(destinatario, corpo): pass
```

**Memória Associativa**:
- Estabelecer **guia de estilo** no início do projeto
- Usar **linters** (pylint, flake8) para enforçar padrões
- Manter **consistência de nomenclatura** (snake_case para Python)
- Seguir **ordem de parâmetros** consistente em funções similares
- Aplicar **padrões de retorno** uniformes (sempre retornar tipo, nunca misturar None com valores)

#### 5️⃣ Omissão

**Definição**: Código ou lógica faltante que deveria existir.

**Exemplos**:
```python
# ❌ Omissão: falta validação de entrada
def dividir(a, b):
    return a / b  # ZeroDivisionError se b == 0!
```

```python
# ✅ Com validação
def dividir(a, b):
    if b == 0:
        raise ValueError("Divisor não pode ser zero")
    return a / b
```

```python
# ❌ Omissão: falta tratamento de exceção
dados = baixar_dados_api()  # Pode falhar por rede!
processar(dados)
```

```python
# ✅ Com tratamento
try:
    dados = baixar_dados_api()
except RequestException as e:
    logger.error(f"Falha ao baixar dados: {e}")
    dados = carregar_dados_cache()
processar(dados)
```

**Memória Associativa**:
- Sempre adicionar **validação de pré-condições**
- Implementar **tratamento de exceções** para operações que podem falhar
- Incluir **testes de borda** (edge cases) para detectar omissões
- Adicionar **logging** em operações críticas
- Documentar **limitações conhecidas** se algo não pode ser implementado

#### 🎯 Impacto no Desenvolvimento

Estes cinco tipos de defeitos são **altamente indesejáveis e inesperados** porque:

❌ **Não contribuem** para o atendimento dos requisitos do desenvolvedor  
❌ **Não satisfazem** as necessidades do cliente direto  
❌ **Não agregam valor** para os clientes do cliente (usuários finais)  
❌ **Introduzem riscos** de bugs em produção  
❌ **Reduzem confiabilidade** do sistema  
❌ **Aumentam custos** de manutenção e suporte

✅ **Objetivo dos Protocolos**: **Eliminar sistematicamente** estes cinco defeitos através de processos rigorosos de validação, revisão e testes.

---

### 🔄 Padrões de Erro e Memória Associativa

#### 🎯 Erros Independentes de Entrada

**Conceito**: Erros que ocorrem **sempre**, independentemente dos dados fornecidos.

**Exemplo**:
```python
# ❌ Erro sempre presente
def processar_lista(items):
    resultado = []
    for i in range(len(items) + 1):  # BUG: sempre causa IndexError
        resultado.append(items[i])
    return resultado
```

**Características**:
- ✅ Reproduzível em **100% dos casos**
- ✅ Não depende de **dados específicos**
- ✅ Indica erro **estrutural** na lógica
- ✅ Mais fácil de **diagnosticar e corrigir**

**Memória Associativa**:
> "Se erro ocorre em todos os testes com dados diferentes, o problema está na **lógica** e não nos **dados**."

#### 🎯 Erros em Escopo Específico

**Conceito**: Erros confinados a um módulo, função ou arquivo específico.

**Exemplo**:
```python
# Módulo: validador.py
def validar_cpf(cpf):
    # BUG: validação incorreta aqui
    return len(cpf) == 11  # Simplificação excessiva!

# Múltiplos lugares usando validador.py:
# - cadastro.py: falha na validação
# - login.py: falha na validação  
# - perfil.py: falha na validação
```

**Características**:
- ✅ **Um único local** com bug
- ✅ **Múltiplos sintomas** em diferentes partes do sistema
- ✅ Corrigir **uma vez** resolve **todos os casos**

**Memória Associativa**:
> "Se múltiplos componentes apresentam o mesmo erro, procure **dependência compartilhada** (import comum)."

#### 🎯 Erros por Importação de Código Bugado

**Conceito**: Algoritmos diferentes falham porque importam o mesmo módulo com defeito.

**Exemplo**:
```python
# utils.py (CÓDIGO BUGADO)
def formatar_data(data):
    return data.strftime("%d/%m/%Y")  # BUG: falha se data = None

# modulo_a.py
from utils import formatar_data
resultado_a = formatar_data(data_a)  # ❌ Falha

# modulo_b.py  
from utils import formatar_data
resultado_b = formatar_data(data_b)  # ❌ Falha

# modulo_c.py
from utils import formatar_data  
resultado_c = formatar_data(data_c)  # ❌ Falha
```

**Investigação com Memória Associativa**:

1. **Observação**: 3 módulos diferentes falham com mesmo `AttributeError`
2. **Padrão**: Todos importam `utils.formatar_data`
3. **Hipótese**: Bug está em `utils.py`, não nos módulos que o usam
4. **Validação**: Testar `formatar_data` isoladamente
5. **Correção**: Corrigir em `utils.py` uma única vez
6. **Verificação**: Todos os 3 módulos voltam a funcionar

**Memória Associativa**:
> "Padrão de erro idêntico em módulos diferentes → investigar **dependências compartilhadas** primeiro."

#### 📊 Base de Conhecimento de Padrões

A IA deve construir e manter uma **base de conhecimento associativa**:

| Padrão de Erro | Causa Provável | Estratégia de Investigação | Solução Típica |
|----------------|----------------|----------------------------|----------------|
| `AttributeError: 'NoneType'` | Variável não inicializada | Rastrear retorno de None | Adicionar verificação ou corrigir inicialização |
| `IndexError: list index out of range` | Loop com índices incorretos | Verificar ranges e len() | Usar iteradores ao invés de índices |
| `KeyError` | Chave não existe no dicionário | Verificar população do dict | Usar dict.get() ou validar chave existe |
| `TypeError: unsupported operand` | Tipos incompatíveis | Verificar tipos de variáveis | Adicionar conversão ou validação de tipo |
| `RecursionError: maximum recursion depth` | Recursão sem caso base | Analisar condição de parada | Adicionar/corrigir caso base |
| `ImportError` / `ModuleNotFoundError` | Dependência faltante | Verificar requirements | Instalar dependência |

**Atualização Contínua**:
- ✅ A cada erro resolvido, **adicionar** à base de conhecimento
- ✅ A cada padrão confirmado, **reforçar** associação
- ✅ A cada falso positivo, **refinar** regra de diagnóstico

---

### 🧠 Integração com Inteligência Artificial Neuro-Simbólica

#### 🎯 O Que é IA Neuro-Simbólica?

**IA Simbólica** (Dedutiva):
- Baseada em **regras explícitas** e **lógica formal**
- Exemplo: "Se error == 'AttributeError' então verificar inicialização"

**IA Neural** (Indutiva):
- Baseada em **aprendizado por padrões** de dados
- Exemplo: Rede neural treinada para reconhecer tipos de erro por sintomas

**IA Neuro-Simbólica** (Combinação):
- **Combina** regras explícitas com aprendizado de padrões
- **Une** dedução (top-down) com indução (bottom-up)
- **Permite** raciocínio transparente e adaptação contínua

#### 🔄 Analogia com HDC (Hyperdimensional Computing)

O problema statement menciona HDC como referência para unir conceitos:

**HDC**: Representa conceitos como vetores de alta dimensão, permitindo:
- ✅ Associação entre conceitos similares
- ✅ Composição de conceitos complexos
- ✅ Recuperação de memórias por similaridade

**Aplicação em Debugging**:
```
Vetor(Error) = Vetor(Tipo) + Vetor(Contexto) + Vetor(Stacktrace)

Similaridade(Error_Atual, Error_Histórico) → Recuperar Solução
```

#### 🎯 Ciclo Neuro-Simbólico de Debugging

```
1. [Simbólico] Aplicar regras gerais conhecidas (dedução)
                      ↓
2. [Neural] Buscar padrões similares em histórico (associação)
                      ↓
3. [Simbólico] Formular hipótese específica (diagnóstico)
                      ↓
4. [Neural] Validar hipótese com testes (indução)
                      ↓
5. [Simbólico] Aplicar correção baseada em regra
                      ↓
6. [Neural] Aprender novo padrão e atualizar base
```

#### 📊 Exemplo Prático Completo

**Situação**: Erro inesperado ao processar upload de arquivo

**Fase 1 - Dedução (Simbólica)**:
```
Traceback mostra: ValueError em parse_csv()
Regra geral: "ValueError geralmente indica formato de dados incorreto"
Hipótese: Arquivo CSV está malformado
```

**Fase 2 - Associação (Neural)**:
```
Buscar em histórico: erros similares com CSV
Padrão encontrado: 3 casos anteriores com encoding UTF-8/Latin1
Associação: "ValueError em CSV → problema de encoding"
```

**Fase 3 - Diagnóstico (Simbólico)**:
```
Hipótese refinada: Arquivo CSV usa encoding Latin1 mas código assume UTF-8
Teste: Tentar abrir com encoding='latin1'
```

**Fase 4 - Validação (Neural)**:
```
Teste confirma: arquivo abre com Latin1
Indução: "Padrão confirmado - arquivos CSV de sistema legado usam Latin1"
```

**Fase 5 - Correção (Simbólica)**:
```python
# Antes (bugado)
with open(arquivo, 'r') as f:
    dados = csv.reader(f)

# Depois (corrigido)
with open(arquivo, 'r', encoding='latin1') as f:
    dados = csv.reader(f)
```

**Fase 6 - Aprendizado (Neural)**:
```
Adicionar à base de conhecimento:
"CSV + ValueError + parse error → tentar encoding='latin1'"
Reforçar padrão: 4 casos confirmados
Criar regra preventiva: Sempre especificar encoding explicitamente
```

---

### 🔧 Aplicação Prática nos Protocolos

#### 📘 Integração no Protocolo Simplicidade 1

**Etapa 4: Correção de Erros**

Adicionar subsecção "Memória Associativa":

```markdown
### 🧠 Aplicar Memória Associativa

Antes de iniciar correção:

1. **Consultar Base de Conhecimento**
   - [ ] Buscar erros similares em histórico do projeto
   - [ ] Verificar padrões conhecidos para este tipo de erro
   - [ ] Revisar soluções aplicadas anteriormente

2. **Análise Dedutiva** (Geral → Específico)
   - [ ] Aplicar regras gerais do tipo de erro observado
   - [ ] Formular hipótese baseada em conhecimento prévio
   - [ ] Identificar escopo provável (folha/galho/raiz)

3. **Análise Indutiva** (Específico → Geral)
   - [ ] Identificar se erro se repete em múltiplos contextos
   - [ ] Procurar dependências compartilhadas
   - [ ] Verificar se erro é independente de entrada

4. **Correção e Aprendizado**
   - [ ] Aplicar correção baseada em análise
   - [ ] Validar que correção resolve problema
   - [ ] Adicionar caso à base de conhecimento
   - [ ] Atualizar regras gerais se necessário
```

#### 📕 Integração no Protocolo Simplicidade 2

**Etapa de Code Review**

Adicionar checklist de Taxonomia de Defeitos:

```markdown
### 🐛 Checklist de Taxonomia de Defeitos

Durante code review, verificar ausência de:

- [ ] **Fato Incorreto**: Valores, constantes ou comentários desatualizados
- [ ] **Informação Estranha**: Código comentado, TODOs obsoletos, imports não utilizados
- [ ] **Ambiguidade**: Nomes vagos, documentação incompleta
- [ ] **Inconsistência**: Violação de convenções de nomenclatura ou padrões
- [ ] **Omissão**: Falta de validações, tratamento de exceções, ou edge cases
```

#### 📗 Integração no Protocolo Simplicidade 3

**Etapa de Produção - Análise de Logs**

Adicionar seção de análise de padrões:

```markdown
### 📊 Análise de Padrões em Logs de Produção

Ao investigar erros em produção:

1. **Frequência de Ocorrência**
   - [ ] Erro é isolado ou recorrente?
   - [ ] Ocorre com dados específicos ou todos os dados?
   - [ ] Frequência aumentou recentemente? (regressão)

2. **Correlação com Deploy**
   - [ ] Erro começou após deploy específico?
   - [ ] Use git bisect para identificar commit causador
   - [ ] Reverta mudanças suspeitas e valide

3. **Análise de Escopo**
   - [ ] Erro está em módulo específico ou múltiplos?
   - [ ] Múltiplos módulos importam código bugado comum?
   - [ ] Traceback aponta para folha, galho ou raiz?

4. **Base de Conhecimento**
   - [ ] Erro já ocorreu antes? Qual foi a solução?
   - [ ] Padrão é conhecido? Aplicar solução padrão
   - [ ] Novo padrão? Documentar para referência futura
```

---

### ✅ Checklist de Utilização

#### 🎯 Para Inteligências Artificiais

Ao investigar e corrigir erros, a IA deve:

**Fase de Análise**:
- [ ] Examinar Traceback de cima para baixo (raiz → folha)
- [ ] Identificar nível do erro (orquestrador/coordenador/executor)
- [ ] Consultar base de conhecimento para padrões similares
- [ ] Aplicar dedução: regras gerais → hipótese específica
- [ ] Buscar indução: múltiplos casos → padrão geral

**Fase de Investigação**:
- [ ] Verificar se erro é independente de entrada
- [ ] Identificar escopo específico do problema
- [ ] Procurar código compartilhado (imports comuns)
- [ ] Aplicar busca binária se necessário
- [ ] Usar git bisect para regressões

**Fase de Correção**:
- [ ] Validar ausência de Fato Incorreto
- [ ] Remover Informação Estranha
- [ ] Eliminar Ambiguidades
- [ ] Garantir Consistência com padrões do projeto
- [ ] Corrigir Omissões (validações, tratamento de erros)

**Fase de Aprendizado**:
- [ ] Adicionar caso à base de conhecimento
- [ ] Atualizar regras gerais se novo padrão identificado
- [ ] Documentar solução para referência futura
- [ ] Reforçar associações de padrões confirmados

#### 📊 Métricas de Sucesso

**Indicadores de Boa Memória Associativa**:
- ✅ **Tempo de diagnóstico reduzido** (menos tempo para identificar causa)
- ✅ **Taxa de correção aumentada** (mais erros corrigidos na primeira tentativa)
- ✅ **Prevenção efetiva** (menos erros recorrentes)
- ✅ **Base de conhecimento crescente** (mais padrões documentados)
- ✅ **Aplicação consistente** (soluções padronizadas)

---

### 🎓 Conclusão

O **Fator de Memória Associativa** transforma a abordagem de debugging de reativa para proativa:

- 🧠 **Aprende** com erros passados
- 🔍 **Reconhece** padrões recorrentes
- 🎯 **Aplica** soluções validadas
- 📈 **Evolui** continuamente
- 🚀 **Previne** problemas futuros

A integração de abordagens **dedutivas** (top-down) e **indutivas** (bottom-up), combinadas com a análise sistemática da **taxonomia de defeitos**, cria uma IA neuro-simbólica capaz de:

✅ Diagnosticar erros mais rapidamente  
✅ Aplicar soluções mais efetivas  
✅ Prevenir problemas recorrentes  
✅ Melhorar continuamente sua base de conhecimento  
✅ Atender melhor os requisitos de desenvolvedores e clientes

---

## 🌐 Idioma do Código: Nomenclatura de Variáveis e Comentários

> **IMPORTANTE PARA IAs**: A escolha do idioma para nomes de variáveis e comentários deve ser definida logo no início do projeto, preferencialmente na primeira sessão de interação com o programador.

### 📋 Regra Padrão

**Por padrão**, ao programar com inteligência artificial:
- ✅ **Nomes de variáveis**: Devem estar em **português**
- ✅ **Comentários**: Devem estar em **português**
- ✅ **Docstrings**: Devem estar em **português**

**Justificativa**: Facilita a compreensão e manutenção do código para desenvolvedores que falam português como língua nativa, mantendo consistência com a documentação e comunicação do projeto.

### 🤔 Pergunta Obrigatória na Primeira Sessão

**A IA DEVE perguntar ao programador no primeiro momento (ou durante a primeira sessão)**:

```
❓ Preferências de Idioma para o Código

Para manter consistência no projeto, preciso definir o idioma padrão 
para nomes de variáveis e comentários no código:

💡 Sugestão: Português (recomendado para projetos nacionais)

Opções:
A) 🇧🇷 Português - Variáveis e comentários em português (PADRÃO)
B) 🇺🇸 Inglês - Variáveis e comentários em inglês
C) 🌍 Misto - Variáveis em inglês, comentários em português
D) ⚙️ Personalizado - Especificar preferência customizada

Qual sua preferência?
```

### ✅ Opções Disponíveis

#### Opção A: 🇧🇷 Português (PADRÃO RECOMENDADO)
```python
# ✅ Exemplo em Português
def calcular_preco_total(itens: List[Item]) -> float:
    """
    Calcula o preço total de uma lista de itens.
    
    Args:
        itens: Lista de itens a serem somados
        
    Returns:
        Preço total com impostos incluídos
    """
    preco_subtotal = sum(item.preco for item in itens)
    taxa_imposto = 0.15
    preco_final = preco_subtotal * (1 + taxa_imposto)
    return preco_final
```

#### Opção B: 🇺🇸 Inglês
```python
# ✅ Exemplo em Inglês
def calculate_total_price(items: List[Item]) -> float:
    """
    Calculates the total price of a list of items.
    
    Args:
        items: List of items to be summed
        
    Returns:
        Total price with taxes included
    """
    subtotal_price = sum(item.price for item in items)
    tax_rate = 0.15
    final_price = subtotal_price * (1 + tax_rate)
    return final_price
```

#### Opção C: 🌍 Misto (Variáveis em Inglês, Comentários em Português)
```python
# ✅ Exemplo Misto
def calculate_total_price(items: List[Item]) -> float:
    """
    Calcula o preço total de uma lista de itens.
    
    Args:
        items: Lista de itens a serem somados
        
    Returns:
        Preço total com impostos incluídos
    """
    subtotal_price = sum(item.price for item in items)
    tax_rate = 0.15  # Taxa de imposto de 15%
    final_price = subtotal_price * (1 + tax_rate)
    return final_price
```

### 📝 Registrar a Preferência

Após a resposta do programador, a IA deve:

1. **Registrar a preferência** em um local visível (ex: README.md, CONTRIBUTING.md)
2. **Aplicar consistentemente** em todo o código gerado
3. **Lembrar da preferência** em sessões futuras do mesmo projeto

**Exemplo de Registro no README.md**:
```markdown
## 🌐 Convenções de Código

- **Idioma do Código**: Português
- **Variáveis**: Nomes em português (ex: `usuario_ativo`, `calcular_total`)
- **Comentários**: Em português
- **Documentação**: Em português
```

### 🔄 Alteração de Preferência

O programador pode solicitar mudança de idioma a qualquer momento:
- ✅ "Mude para inglês a partir de agora"
- ✅ "Prefiro comentários em português, mas variáveis em inglês"
- ✅ "Use inglês apenas para APIs públicas"

**A IA deve confirmar a mudança** e atualizar a documentação de convenções.

### ⚠️ Exceções Comuns

Independente da escolha do idioma, **mantenha em inglês**:
- ✅ Nomes de bibliotecas e frameworks (ex: `import pandas`, `from flask import`)
- ✅ Palavras-chave da linguagem (ex: `def`, `class`, `if`, `for`)
- ✅ Nomes de APIs públicas (se o código for distribuído internacionalmente)
- ✅ Termos técnicos sem tradução adequada (ex: `callback`, `payload`, `refactoring`)

### 🎯 Rationale

**Por quê perguntar ao programador?**

1. **Contexto do Projeto**: Projetos nacionais vs. internacionais têm necessidades diferentes
2. **Equipe**: Time brasileiro pode preferir português; time internacional precisa inglês
3. **Legibilidade**: Código é lido mais vezes do que escrito - deve ser claro para quem mantém
4. **Consistência**: Definir padrão no início evita mistura confusa de idiomas
5. **Profissionalismo**: Demonstra atenção aos detalhes e respeito pelas preferências do desenvolvedor

**Por quê Português como padrão?**

Para projetos brasileiros/portugueses:
- ✅ Desenvolvedores leem e entendem mais rápido
- ✅ Facilita onboarding de novos membros do time
- ✅ Documentação e código no mesmo idioma = menos tradução mental
- ✅ Variáveis representam conceitos de negócio em português

**Quando preferir Inglês?**

- 🌍 Projeto open-source internacional
- 🌍 Equipe multicultural
- 🌍 Produto voltado para mercado global
- 🌍 Biblioteca/framework para distribuição pública

---

## 🖥️ Importância da Interface de Linha de Comando (CLI)

> **CRÍTICO PARA IAs**: Em muitos casos, senão em todos os casos, é importante implementar uma **CLI (Command-Line Interface)** que pode ser utilizada no terminal para acesso pelo usuário e principalmente para **testes por parte de quem estiver desenvolvendo o software**.

### 🎯 Por Quê o CLI é Essencial?

**Contexto**: Dentro de um determinado contexto relevante, a implementação de CLI é necessária até mesmo em casos de testes, em que a inteligência artificial que estiver auxiliando, **por não poder interagir diretamente com a interface gráfica do usuário**, terá que realizar testes no terminal.

#### ✅ Benefícios do CLI para Desenvolvimento e Testes

1. **🤖 Testabilidade pela IA**
   - ✅ A IA pode executar testes via CLI sem precisar de GUI
   - ✅ Comandos podem ser automatizados em scripts de teste
   - ✅ Saída textual é facilmente validável programaticamente
   - ✅ Não depende de eventos de mouse/teclado complexos

2. **⚡ Velocidade de Desenvolvimento**
   - ✅ Testar funcionalidades rapidamente sem abrir GUI
   - ✅ Debug mais rápido com flags de verbose (`--debug`, `--verbose`)
   - ✅ Iterações mais rápidas durante desenvolvimento
   - ✅ Scripting e automação de tarefas repetitivas

3. **🧪 Alvo Principal de Testes**
   - ✅ **Lógica bem estruturada**: CLI força separação de lógica e apresentação
   - ✅ **Fundamentação sólida**: Se CLI funciona, a lógica está correta
   - ✅ **Cobertura de testes**: Mais fácil testar todas as funcionalidades via CLI
   - ✅ **Módulos de teste independentes**: Podem focar na lógica via CLI
   - ✅ **Validação de requisitos**: CLI demonstra que requisitos são atendidos

4. **🔄 CI/CD e Automação**
   - ✅ Integração contínua pode testar via CLI
   - ✅ Scripts de deploy usam CLI para validar instalação
   - ✅ Testes automatizados são mais confiáveis com CLI
   - ✅ Pipelines podem executar comandos CLI sem ambiente gráfico

5. **👥 Acesso Remoto e Servidores**
   - ✅ Servidores headless (sem GUI) podem usar CLI
   - ✅ SSH permite administração remota via CLI
   - ✅ Scripts podem ser executados em batch jobs
   - ✅ Ferramentas de monitoramento podem usar CLI

### 📐 Arquitetura Recomendada

**Separação Clara de Responsabilidades**:

```
┌─────────────────────────────────────────┐
│          CLI (Interface)                │
│  - Parsing de argumentos                │
│  - Validação de entrada                 │
│  - Formatação de saída                  │
└──────────────┬──────────────────────────┘
               │ chama
               ↓
┌─────────────────────────────────────────┐
│          CORE (Lógica de Negócio)       │ ← TESTAR AQUI!
│  - Algoritmos                           │
│  - Processamento de dados               │
│  - Regras de negócio                    │
└──────────────┬──────────────────────────┘
               │ usa
               ↓
┌─────────────────────────────────────────┐
│          GUI (Interface Gráfica)        │
│  - Widgets visuais                      │
│  - Eventos de usuário                   │
│  - Apresentação visual                  │
└─────────────────────────────────────────┘
```

**Princípio Fundamental**:
> **CLI e GUI devem usar a MESMA lógica de negócio (CORE).**
> 
> Se a lógica está bem estruturada no CORE, tanto CLI quanto GUI funcionarão corretamente.

### 🛠️ Implementação Prática

#### Exemplo em Python

**Estrutura do Projeto**:
```
project/
├── src/
│   ├── core/              # Lógica de negócio
│   │   ├── calculator.py  # Algoritmos puros
│   │   └── validator.py   # Validações
│   ├── cli/               # Interface CLI
│   │   └── main.py        # Parsing + formatação
│   └── gui/               # Interface GUI
│       └── window.py      # Widgets + eventos
└── tests/
    ├── test_core.py       # ✅ Testes da lógica (PRINCIPAL)
    ├── test_cli.py        # ✅ Testes da CLI
    └── test_gui.py        # Testes da GUI (opcional)
```

**Exemplo de CLI**:
```python
# src/cli/main.py
import argparse
from src.core.calculator import Calculator

def main():
    """CLI principal - apenas parsing e formatação."""
    parser = argparse.ArgumentParser(description='Calculadora')
    parser.add_argument('operation', choices=['add', 'sub', 'mul', 'div'])
    parser.add_argument('a', type=float, help='Primeiro número')
    parser.add_argument('b', type=float, help='Segundo número')
    parser.add_argument('--verbose', action='store_true', help='Modo verbose')
    
    args = parser.parse_args()
    
    # ✅ Lógica está no CORE, não no CLI
    calc = Calculator()
    result = calc.calculate(args.operation, args.a, args.b)
    
    # Apenas formatação de saída
    if args.verbose:
        print(f"Operação: {args.operation}")
        print(f"Entrada: {args.a}, {args.b}")
    print(f"Resultado: {result}")

if __name__ == '__main__':
    main()
```

**Exemplo de CORE (lógica testável)**:
```python
# src/core/calculator.py
class Calculator:
    """Lógica de negócio pura - facilmente testável."""
    
    def calculate(self, operation: str, a: float, b: float) -> float:
        """
        Realiza cálculo baseado na operação.
        
        Args:
            operation: Tipo de operação ('add', 'sub', 'mul', 'div')
            a: Primeiro número
            b: Segundo número
            
        Returns:
            Resultado da operação
            
        Raises:
            ValueError: Se operação inválida ou divisão por zero
        """
        if operation == 'add':
            return a + b
        elif operation == 'sub':
            return a - b
        elif operation == 'mul':
            return a * b
        elif operation == 'div':
            if b == 0:
                raise ValueError("Divisão por zero")
            return a / b
        else:
            raise ValueError(f"Operação inválida: {operation}")
```

**Exemplo de Teste (via CORE)**:
```python
# tests/test_core.py
import pytest
from src.core.calculator import Calculator

def test_calculator_add():
    calc = Calculator()
    assert calc.calculate('add', 2, 3) == 5

def test_calculator_division_by_zero():
    calc = Calculator()
    with pytest.raises(ValueError, match="Divisão por zero"):
        calc.calculate('div', 10, 0)

# ✅ Testa a lógica diretamente, sem CLI ou GUI
```

### 🧪 Estratégia de Testes com CLI

#### 1. **Testes da Lógica (CORE) - PRIORIDADE MÁXIMA**
```python
# tests/test_core.py
def test_business_logic():
    """Testa CORE diretamente - mais importante."""
    # Arrange
    calc = Calculator()
    
    # Act
    result = calc.calculate('add', 2, 3)
    
    # Assert
    assert result == 5
```

#### 2. **Testes da CLI (Interface)**
```python
# tests/test_cli.py
import subprocess
import sys

def test_cli_add():
    """Testa CLI via subprocess - testa integração."""
    result = subprocess.run(
        [sys.executable, 'src/cli/main.py', 'add', '2', '3'],
        capture_output=True,
        text=True
    )
    
    assert result.returncode == 0
    assert 'Resultado: 5.0' in result.stdout

def test_cli_invalid_operation():
    """Testa tratamento de erros na CLI."""
    result = subprocess.run(
        [sys.executable, 'src/cli/main.py', 'invalid', '2', '3'],
        capture_output=True,
        text=True
    )
    
    assert result.returncode != 0
    assert 'error' in result.stderr.lower()
```

#### 3. **Testes da GUI (Opcional/Manual)**
```python
# tests/test_gui.py
# Pode usar pytest-qt se necessário, mas não é prioridade
# A GUI deve apenas apresentar o que o CORE já validou
```

### ✅ Checklist de Implementação CLI

**Antes de implementar funcionalidade**:
- [ ] 1. Implementar lógica no CORE (pura, sem I/O)
- [ ] 2. Criar testes para o CORE (100% coverage)
- [ ] 3. Implementar CLI que usa o CORE
- [ ] 4. Testar CLI via subprocess (smoke tests)
- [ ] 5. Implementar GUI que usa o CORE (se necessário)
- [ ] 6. Validar que CLI e GUI usam mesma lógica

**Durante desenvolvimento**:
- [ ] IA deve testar via CLI quando GUI não está disponível
- [ ] Priorizar testes do CORE sobre testes de CLI/GUI
- [ ] Garantir que CLI tem todas as funcionalidades do CORE
- [ ] Documentar comandos CLI em `README.md` ou `docs/CLI.md`

**Estrutura de comando CLI recomendada**:
```bash
# Formato padrão
python -m project.cli <comando> [argumentos] [opções]

# Exemplos
python -m project.cli calculate --operation add --a 2 --b 3
python -m project.cli validate --input data.txt
python -m project.cli process --file data.csv --output result.json --verbose
```

### 📝 Documentação CLI

**Incluir no README.md**:
```markdown
## 🖥️ Command-Line Interface (CLI)

### Instalação
```bash
pip install -e .
```

### Uso Básico
```bash
# Ajuda geral
python -m project.cli --help

# Comando específico
python -m project.cli calculate add 2 3

# Modo verbose
python -m project.cli calculate add 2 3 --verbose
```

### Comandos Disponíveis
- `calculate`: Realiza operações matemáticas
- `validate`: Valida entrada de dados
- `process`: Processa arquivos de dados

### Exemplos
```bash
# Adição
python -m project.cli calculate add 10 5
# Saída: 15.0

# Divisão com tratamento de erro
python -m project.cli calculate div 10 0
# Saída: Error: Divisão por zero
```
```

### 🎯 Rationale

**Por quê CLI é crítico para testes com IA?**

1. **Limitação da IA**: 
   - ❌ IA não pode clicar em botões da GUI
   - ✅ IA pode executar comandos CLI no terminal
   - ✅ IA pode validar saída textual de comandos

2. **Arquitetura Limpa**:
   - ✅ CLI força separação entre lógica e apresentação
   - ✅ Lógica no CORE é testável isoladamente
   - ✅ GUI e CLI compartilham mesma lógica validada

3. **Desenvolvimento Iterativo**:
   - ✅ Implementar CORE primeiro (com CLI)
   - ✅ Testar exaustivamente via CLI
   - ✅ Adicionar GUI depois (sabendo que lógica funciona)

4. **Confiança nos Testes**:
   - ✅ Se CLI funciona → lógica está correta
   - ✅ Se lógica está correta → GUI também funcionará
   - ✅ Testes de GUI podem ser mínimos (smoke tests)

**Mensagem para IAs**:
> "Sempre que implementar funcionalidade, crie CLI primeiro. Teste via CLI antes de criar GUI. Se CLI funciona, você validou que a lógica atende aos requisitos do usuário."

---

## 📧 Meios de Contato para Feedback do Usuário

> **IMPORTANTE PARA IAs**: Durante a primeira sessão de interação com o programador, a inteligência artificial deve perguntar se o desenvolvedor gostaria de incluir meios de contato no projeto para que os usuários possam fornecer feedback aos responsáveis.

### 📋 Contexto e Propósito

Projetos de software se beneficiam enormemente de feedback direto dos usuários. Comentários, sugestões, críticas, reclamações, elogios e opiniões são fundamentais para a evolução e melhoria contínua do projeto.

### 🤔 Pergunta Obrigatória na Primeira Sessão

**A IA DEVE perguntar ao programador no primeiro momento (ou durante a primeira sessão)**:

```
❓ Meios de Contato para Feedback do Usuário

Gostaria de incluir meios de contato no projeto para que os usuários
possam enviar feedback (comentários, sugestões, críticas, reclamações,
elogios e opiniões)?

💡 Sugestão: Sim (recomendado para projetos com usuários finais)

Opções:
A) ✅ Sim, incluir GitHub Issues (PADRÃO RECOMENDADO para projetos versionados)
B) ✅ Sim, incluir email para feedback (alternativa ou complemento)
C) ✅ Sim, incluir formulário de contato na aplicação
D) ✅ Sim, incluir múltiplos canais (GitHub + email + formulário)
E) ❌ Não, não incluir meios de contato

Qual sua preferência?
```

### ✅ Opções Disponíveis

#### Opção A: ✅ GitHub Issues (PADRÃO RECOMENDADO)

**Por quê GitHub Issues como padrão?**
- ✅ **Transparência**: Todos veem feedback e respostas (comunidade se beneficia)
- ✅ **Rastreabilidade**: Histórico completo de discussões e decisões
- ✅ **Organização**: Labels, milestones, assignees, projetos
- ✅ **Integração**: Commits, PRs e Issues conectados
- ✅ **Notificações**: Atualizações automáticas para interessados
- ✅ **Gratuito**: Ilimitado para repositórios públicos e privados
- ✅ **Pesquisável**: Fácil encontrar issues similares antes de abrir nova
- ✅ **Colaborativo**: Comunidade pode ajudar a resolver problemas

**Para projetos com repositório Git (GitHub, GitLab, Bitbucket)**:
```markdown
## 🐛 Reportar Problemas ou Dar Feedback

Use as [GitHub Issues](https://github.com/seu-usuario/seu-projeto/issues) para:

- 🐛 Reportar bugs e problemas
- 💡 Sugerir novas funcionalidades
- 💬 Compartilhar feedback geral
- 🎉 Elogios e reconhecimento
- ❓ Fazer perguntas sobre o projeto
- 📝 Discutir melhorias e mudanças

**Como reportar**:
1. Verifique se já existe issue similar (evita duplicatas)
2. Use os templates disponíveis (Bug Report, Feature Request, Feedback)
3. Seja claro e específico na descrição
4. Inclua prints/logs quando relevante

**Templates disponíveis**:
- 🐛 Bug Report
- 💡 Feature Request  
- 💬 Feedback Geral
- 🎉 Elogios e Reconhecimento

**Tempo de resposta**: Normalmente respondemos em até 48-72 horas.

Valorizamos muito sua contribuição! 🙏
```

**Exemplo completo no README.md**:
```markdown
## 📬 Feedback e Contribuições

### 💬 Reportar Bugs ou Sugerir Melhorias

A melhor forma de contribuir é através das **[GitHub Issues](https://github.com/usuario/projeto/issues)**:

**Reportar Bug** 🐛
- Use o template "Bug Report"
- Descreva o comportamento esperado vs observado
- Inclua passos para reproduzir o problema
- Adicione prints, logs ou vídeos se possível

**Sugerir Funcionalidade** 💡
- Use o template "Feature Request"
- Explique o problema que a feature resolveria
- Descreva a solução proposta
- Considere alternativas já existentes

**Feedback Geral** 💬
- Elogios, sugestões, opiniões sobre UX/UI
- Dúvidas sobre funcionamento
- Compartilhar casos de uso interessantes

### 📧 Contato Alternativo

Prefere email? Também aceitamos feedback em: **contato@projeto.com**

> **Nota**: Para bugs e features, preferimos GitHub Issues pois mantém histórico
> público e permite que outros usuários com problemas similares encontrem soluções.
```

**Issue Templates (criar em `.github/ISSUE_TEMPLATE/`)**:

**1. Bug Report** (`.github/ISSUE_TEMPLATE/bug_report.md`):
```markdown
---
name: Bug Report 🐛
about: Reportar um problema ou comportamento inesperado
title: '[BUG] '
labels: bug
assignees: ''
---

## 🐛 Descrição do Bug
<!-- Descrição clara e concisa do problema -->

## 🔄 Passos para Reproduzir
1. 
2. 
3. 

## ✅ Comportamento Esperado
<!-- O que você esperava que acontecesse -->

## ❌ Comportamento Observado
<!-- O que realmente aconteceu -->

## 📸 Screenshots/Logs
<!-- Se aplicável, adicione prints ou logs -->

## 💻 Ambiente
- OS: [e.g. Windows 11, macOS 14, Ubuntu 22.04]
- Versão do Projeto: [e.g. v1.2.3]
- Navegador (se web): [e.g. Chrome 120, Firefox 121]
```

**2. Feature Request** (`.github/ISSUE_TEMPLATE/feature_request.md`):
```markdown
---
name: Feature Request 💡
about: Sugerir uma nova funcionalidade
title: '[FEATURE] '
labels: enhancement
assignees: ''
---

## 💡 Resumo da Feature
<!-- Breve descrição da funcionalidade proposta -->

## 🎯 Problema que Resolve
<!-- Que problema ou necessidade essa feature atende? -->

## 🔧 Solução Proposta
<!-- Como você imagina que essa feature funcionaria? -->

## 🔀 Alternativas Consideradas
<!-- Outras formas de resolver o mesmo problema -->

## 📊 Benefícios Esperados
<!-- Por que essa feature seria útil para o projeto? -->
```

**3. Feedback Geral** (`.github/ISSUE_TEMPLATE/feedback.md`):
```markdown
---
name: Feedback Geral 💬
about: Compartilhar opinião, elogio, sugestão ou dúvida
title: '[FEEDBACK] '
labels: feedback
assignees: ''
---

## 💬 Seu Feedback

<!-- Compartilhe suas opiniões, sugestões, elogios, dúvidas ou qualquer outro comentário! -->

## 📝 Contexto (Opcional)
<!-- Se relevante, adicione contexto sobre como você usa o projeto -->
```

#### Opção B: ✅ Email para Feedback (Alternativa ou Complemento)

**O que incluir**:
- Email de contato dedicado para feedback
- Todos os tipos de feedback são bem-vindos:
  - 💬 Comentários gerais
  - 💡 Sugestões de melhorias
  - 🐛 Críticas construtivas
  - 😞 Reclamações sobre problemas
  - 🎉 Elogios e reconhecimento
  - 📝 Opiniões sobre funcionalidades

**Onde documentar**:
```markdown
## 📧 Feedback e Contato

Sua opinião é muito importante para nós! Envie seus comentários, 
sugestões, críticas, reclamações, elogios e opiniões para:

**Email**: feedback@seuprojeto.com

Todos os feedbacks são lidos e considerados para melhorias futuras.
```

**Exemplo de implementação (README.md)**:
```markdown
## 📮 Feedback

Adoraríamos ouvir sua opinião! Envie seus comentários, sugestões, 
críticas, reclamações, elogios e opiniões para:

- **Email**: contato@meuprojeto.com.br
- **Resposta**: Normalmente respondemos em até 48 horas

Seu feedback nos ajuda a melhorar continuamente!
```

**Quando usar email**:
- Feedback confidencial ou sensível
- Projetos sem repositório público
- Usuários não-técnicos que preferem email
- Como canal complementar ao GitHub Issues

> **Nota**: Se o projeto tem repositório Git, preferimos GitHub Issues para manter
> histórico público e permitir que a comunidade se beneficie das discussões.

#### Opção C: ✅ Formulário de Contato na Aplicação

**Para aplicações web/desktop**:
- Adicionar seção "Feedback" ou "Contato" na interface
- Formulário com campos:
  - Nome (opcional)
  - Email (para resposta)
  - Tipo: Comentário | Sugestão | Crítica | Reclamação | Elogio | Opinião
  - Mensagem
- Envio via email ou salvo em banco de dados

**Exemplo de implementação (GUI)**:
```python
# Menu: Help → Send Feedback
class FeedbackDialog(QDialog):
    def __init__(self):
        super().__init__()
        self.setWindowTitle("Enviar Feedback")
        
        # Tipo de feedback
        self.tipo_combo = QComboBox()
        self.tipo_combo.addItems([
            "💬 Comentário",
            "💡 Sugestão",
            "🐛 Crítica/Bug",
            "😞 Reclamação",
            "🎉 Elogio",
            "📝 Opinião"
        ])
        
        # Email (opcional)
        self.email_input = QLineEdit()
        self.email_input.setPlaceholderText("seu@email.com (opcional)")
        
        # Mensagem
        self.message_text = QTextEdit()
        self.message_text.setPlaceholderText(
            "Compartilhe seus comentários, sugestões, críticas, "
            "reclamações, elogios ou opiniões..."
        )
        
        # Botão enviar
        self.send_button = QPushButton("Enviar Feedback")
        self.send_button.clicked.connect(self.send_feedback)
```

#### Opção D: ✅ Múltiplos Canais

**Combinar várias opções**:
```markdown
## 📞 Entre em Contato

Valorizamos seu feedback! Você pode nos contatar por:

### 📧 Email
- **Feedback Geral**: feedback@projeto.com
- **Suporte Técnico**: suporte@projeto.com
- Respondemos em até 48 horas

### 💬 GitHub Issues
- Reportar bugs: [Issues](https://github.com/user/projeto/issues)
- Sugerir funcionalidades: [Discussions](https://github.com/user/projeto/discussions)

### 🌐 Formulário de Contato
- Acesse: Menu → Ajuda → Enviar Feedback
- Ou: https://projeto.com/contato

### 📱 Redes Sociais
- Twitter: [@seuprojeto](https://twitter.com/seuprojeto)
- Discord: [Comunidade](https://discord.gg/seuprojeto)
```

#### Opção E: ❌ Não Incluir

**Quando escolher esta opção**:
- ⚠️ Projetos pessoais/internos sem usuários externos
- ⚠️ Protótipos descartáveis
- ⚠️ Scripts de uso único

**Consequência**: Usuários não terão canal direto para feedback, o que pode limitar a evolução do projeto.

### 📝 Registrar a Preferência

Após a resposta do programador, a IA deve:

1. **Adicionar seção de contato/feedback** no README.md
2. **Criar arquivo CONTATO.md** (se necessário) com detalhes
3. **Implementar formulário** (se aplicação com interface)
4. **Documentar** em CONTRIBUTING.md (para projetos open-source)

**Exemplo de registro (README.md)**:
```markdown
## 📬 Feedback e Contato

Este projeto valoriza feedback dos usuários! 

- **Email**: feedback@projeto.com
- **Tipos de feedback bem-vindos**: Comentários, sugestões, críticas, 
  reclamações, elogios e opiniões
- **Tempo de resposta**: Até 48 horas úteis

Seu feedback é essencial para melhorarmos continuamente!
```

### 🎯 Rationale

**Por quê perguntar sobre meios de contato?**

1. **Melhoria Contínua**: Feedback direto ajuda a identificar problemas e oportunidades
2. **Engajamento**: Usuários que podem dar feedback se sentem mais conectados ao projeto
3. **Qualidade**: Críticas e sugestões melhoram a qualidade do software
4. **Priorização**: Feedback ajuda a entender o que é mais importante para os usuários
5. **Reconhecimento**: Elogios motivam a equipe de desenvolvimento
6. **Transparência**: Canal aberto demonstra compromisso com os usuários

**Por quê Email como padrão?**

Para projetos com usuários:
- ✅ **Universal**: Todo mundo tem email
- ✅ **Simples**: Não requer conta ou cadastro adicional
- ✅ **Direto**: Comunicação privada e pessoal
- ✅ **Consolidado**: Todos os tipos de feedback em um único canal
- ✅ **Rastreável**: Histórico completo de comunicações
- ✅ **Profissional**: Canal formal e adequado para qualquer tipo de feedback

**Quando preferir outras opções?**

- 🌍 **GitHub Issues**: Projetos open-source (transparência pública)
- 🌍 **Formulário**: Apps com muitos usuários (organização e categorização)
- 🌍 **Múltiplos canais**: Projetos grandes (diferentes públicos, diferentes necessidades)
- 🌍 **Nenhum**: Projetos internos/pessoais sem usuários externos

### ⚠️ Considerações Importantes

**Gestão de Feedback**:
- ✅ Definir quem responderá aos feedbacks (responsável)
- ✅ Estabelecer tempo de resposta esperado (SLA)
- ✅ Criar processo para triagem e priorização
- ✅ Documentar feedbacks relevantes (issues, backlog)
- ✅ Agradecer sempre, mesmo para críticas

**Privacidade**:
- ✅ Informar como dados de contato serão usados
- ✅ Não compartilhar emails sem permissão
- ✅ Conformidade com LGPD/GDPR se aplicável

**Exemplo de boas práticas**:
```markdown
## 📧 Política de Feedback

**Comprometemos-nos a**:
- ✅ Responder todos os feedbacks em até 48 horas úteis
- ✅ Tratar todas as opiniões com respeito
- ✅ Considerar seriamente críticas e sugestões
- ✅ Manter privacidade dos dados de contato (LGPD)
- ✅ Agradecer contribuições construtivas

**Você pode esperar**:
- Resposta personalizada (não automática)
- Atualizações sobre sugestões implementadas
- Reconhecimento em changelogs (se desejar)
```

---

## 📊 Divisão Recursiva de Tarefas Complexas

> **IMPORTANTE**: Se a tarefa for muito longa ou complexa, e houver limites de tempo ou comprimento de resposta, a inteligência artificial deve dividir a tarefa em partes menores, recursivamente, até conseguir uma tarefa que possa fornecer uma resposta satisfatória e de acordo com o limite de resposta determinado.

### 🔄 Estratégia de Divisão

**Quando Aplicar**:
- ✅ Tarefa estimada em >4 horas (divide em 2+ sprints)
- ✅ Resposta muito longa (>1000 linhas de código)
- ✅ Múltiplas funcionalidades interdependentes
- ✅ Escopo não claro ou ambíguo
- ✅ Risco de timeout ou limite de resposta

**Como Dividir** (Recursivamente):

1. **Nível 1 - Divisão por Funcionalidade**:
   ```
   Tarefa Grande: "Sistema de Autenticação Completo"
   ↓ Dividir em:
   ├── Task 1.1: Login básico (username/password)
   ├── Task 1.2: Recuperação de senha
   ├── Task 1.3: 2FA (autenticação de dois fatores)
   └── Task 1.4: OAuth/Social login
   ```

2. **Nível 2 - Divisão por Componente** (se ainda muito grande):
   ```
   Task 1.1: Login básico
   ↓ Dividir em:
   ├── Task 1.1.1: Backend - API de autenticação
   ├── Task 1.1.2: Frontend - Formulário de login
   ├── Task 1.1.3: Validação e segurança
   └── Task 1.1.4: Testes unitários
   ```

3. **Nível 3 - Divisão por Etapa** (se ainda muito grande):
   ```
   Task 1.1.1: Backend - API de autenticação
   ↓ Dividir em:
   ├── Task 1.1.1.1: Modelo de usuário (database schema)
   ├── Task 1.1.1.2: Hash de senha (bcrypt)
   ├── Task 1.1.1.3: Geração de token JWT
   └── Task 1.1.1.4: Endpoint /api/login
   ```

**Critério de Parada**:
- ⏱️ Tarefa pode ser completada em <3 horas
- 📝 Resposta cabe em limite razoável (arquivo único, <500 linhas)
- ✅ Escopo claro e bem definido
- 🧪 Pode ser testada isoladamente

**Princípios de Divisão**:
1. **Independência**: Cada subtarefa deve ser o mais independente possível
2. **Coesão**: Subtarefas relacionadas devem estar próximas na sequência
3. **Valor Incremental**: Cada subtarefa deve adicionar valor ao projeto
4. **Testabilidade**: Cada subtarefa deve ser testável isoladamente

**Exemplo Prático**:
```markdown
❌ RUIM - Tarefa muito grande:
[ ] Implementar sistema completo de gerenciamento de tarefas (estimado: 20h)

✅ BOM - Dividido recursivamente:
Sprint 1 (3h):
├── [x] Task 1.1: Modelo de Task (database schema)
└── [x] Task 1.2: CRUD básico (create/read)

Sprint 2 (3h):
├── [ ] Task 2.1: Update e Delete
└── [ ] Task 2.2: Filtros e busca

Sprint 3 (3h):
├── [ ] Task 3.1: GUI - Lista de tarefas
└── [ ] Task 3.2: GUI - Formulário de edição

Sprint 4 (2h):
├── [ ] Task 4.1: Testes unitários
└── [ ] Task 4.2: Documentação
```

**Por quê?**: Dividir tarefas grandes garante progresso constante, evita timeouts, facilita debugging, e mantém foco em entregas incrementais.

---

## 🎯 Quando Usar Simplicidade 1?

### ✅ Use Simplicidade 1 SE:
- ✅ Projeto **solo** ou pequena equipe (1-3 devs)
- ✅ Features **simples a médias**
- ✅ **Prototipagem rápida** ou POC
- ✅ Primeiro desenvolvimento de uma funcionalidade
- ✅ **Velocidade** é mais importante que perfeição
- ✅ Projetos **internos não-críticos**
- ✅ **Aprendendo** novas tecnologias ou experimentando
- ✅ Scripts de **uso único** ou ferramentas temporárias

### ❌ NÃO use Simplicidade 1 SE:
- ❌ Aplicação **crítica de produção** → Use **Simplicidade 3** (solo) ou **Simplicidade 2** (equipe)
- ❌ Sistema com **requisitos de segurança** (dados sensíveis, LGPD) → Use **Simplicidade 3**
- ❌ Features de **alto impacto/risco** → Use **Simplicidade 2** ou **3**
- ❌ Equipes **grandes** (>5 devs) → Use **Simplicidade 2**
- ❌ Biblioteca/API **pública** → Use **Simplicidade 2**
- ❌ Sistema com **requisitos de performance** críticos → Use **Simplicidade 2** ou **3**

### 🔄 Quando Migrar para Outros Protocolos?
- **→ Simplicidade 3**: Quando projeto interno virar produção com usuários reais
- **→ Simplicidade 2**: Quando equipe crescer para 3+ desenvolvedores

**Rationale**: Simplicidade 1 é **ágil e pragmático** para desenvolvimento rápido, mas **não tem camadas de segurança críticas para produção** (security checklist, CI/CD, rollback plans). É perfeito para **aprender, prototipar e iterar rapidamente**, mas deve ser **upgradado** quando o código for para produção ou equipe crescer.

---

## 📋 Espinha Dorsal do Protocolo (14 Etapas)

**Resumo Executivo**:
1. 📚 Ler a documentação
   - 1.5 🔍 **Pesquisar tecnologias adequadas ao projeto** (OBRIGATÓRIO NO INÍCIO)
2. ✅ Escolher tarefas mais simples
3. ❓ Fazer perguntas até sanar 100% das dúvidas
4. 🔍 Analisar e estudar o projeto
5. 🎯 Fazer sprints das tarefas mais simples
6. 💻 Implementar com arquitetura profissional (GoF + GRASP)
   - 6.6 🎨 **Ícones do Projeto** (OBRIGATÓRIO)
7. ⌨️ **Verificar Implementação CLI + Revisão de Código (9 critérios)**
8. 🖥️ **Verificar Implementação GUI + Revisão de Código (9 critérios)**
9. 🔗 **Verificar Integração com Programa Principal**
🔟 🧪 Fazer testes (100% cobertura)
1️⃣1️⃣ 🧹 Organizar pasta raiz
1️⃣2️⃣ 📝 Preencher documentação
1️⃣3️⃣ 🚀 Fazer commit e push

### 1️⃣ **Ler a Documentação**

> **🚨 CRÍTICO PARA IAs - PRIMEIRA AÇÃO OBRIGATÓRIA**: Antes de QUALQUER coisa, a IA **DEVE** procurar e ler **100% da documentação markdown local** existente no projeto.

#### 📖 **Etapa 1.0: Busca e Leitura Completa de Documentação** [PRIORITÁRIO]

**ANTES de começar qualquer tarefa**, a IA deve:

**Passo 1: Procurar por toda documentação markdown no projeto**

Buscar recursivamente por todos os arquivos `.md` no workspace:
- 📂 **Raiz do projeto**: `README.md`, `TASKS.md`, `TODO.md`, `CHANGELOG.md`, etc.
- 📂 **Pasta `docs/`**: Toda documentação existente
- 📂 **Subpastas**: `docs/plans/`, `docs/ADR/`, `docs/api/`, etc.
- 📂 **Qualquer outro local**: Arquivos `.md` em qualquer diretório

**Comando sugerido** (para IA com acesso a terminal):
```bash
find . -name "*.md" -type f | grep -v node_modules | grep -v venv
```

**Passo 2: Ler 100% do conteúdo de todos os arquivos markdown encontrados**

A IA **DEVE LER COMPLETAMENTE**:
- ✅ `README.md` - Visão geral do projeto
- ✅ `TASKS.md` ou equivalente - Tarefas pendentes e concluídas
- ✅ `docs/REQUIREMENTS.md` - Requisitos funcionais e não-funcionais
- ✅ `docs/ARCHITECTURE.md` - Decisões arquiteturais e stack tecnológico
- ✅ `docs/vX.Y.Z-SPECIFICATIONS.md` - Especificações de versões anteriores
- ✅ `docs/CHANGELOG.md` - Histórico de mudanças
- ✅ `docs/plans/*.md` - Planos de ação existentes
- ✅ `docs/ADR/*.md` - Architecture Decision Records (se houver)
- ✅ **Qualquer outro arquivo `.md`** encontrado

**Por quê ler 100%?**
- ✅ **Contexto Completo**: Entender todo o histórico e decisões do projeto
- ✅ **Evitar Retrabalho**: Não reimplementar funcionalidades já existentes
- ✅ **Consistência**: Seguir padrões já estabelecidos
- ✅ **Decisões Anteriores**: Entender por quê certas escolhas foram feitas
- ✅ **Tarefas Pendentes**: Saber o que já foi feito e o que falta

**Passo 3: Se NÃO encontrar documentação, perguntar ao usuário**

Se a IA **não encontrar** documentação markdown:

```markdown
❓ **Documentação do Projeto**

Procurei por documentação markdown no projeto mas não encontrei arquivos `.md`.

**Você tem documentação do projeto?**
A) Sim, está em [localização específica]
B) Sim, mas em formato diferente (.txt, .docx, etc.)
C) Não, ainda não existe documentação

**Se C (não existe documentação):**
Preciso criar a documentação inicial do zero. Para isso, preciso:

1. **Requisitos do Projeto**:
   - Qual o objetivo principal deste projeto?
   - Quais funcionalidades devem ser implementadas?
   - Quem são os usuários/clientes?

2. **Tarefas Atuais**:
   - Quais tarefas você precisa que eu realize?
   - Há alguma prioridade específica?

3. **Contexto Técnico**:
   - Stack tecnológico já definido? (linguagens, frameworks)
   - Há código existente? Se sim, onde?
   - Há restrições técnicas?

Com essas informações, vou criar a estrutura de documentação inicial:
- `README.md` (visão geral)
- `docs/REQUIREMENTS.md` (requisitos detalhados)
- `docs/TASKS.md` (tarefas e progresso)
- `docs/ARCHITECTURE.md` (decisões técnicas)
```

**Passo 4: Se documentação não existir, criar do zero**

**A IA deve criar documentação inicial obrigatória**:

**Estrutura Mínima Obrigatória**:
```
📁 Raiz do Projeto
├── README.md                    # Visão geral do projeto
├── TASKS.md                     # Lista de tarefas (ou docs/TASKS.md)
└── 📁 docs/
    ├── REQUIREMENTS.md          # Requisitos funcionais e não-funcionais
    ├── ARCHITECTURE.md          # Stack tecnológico e decisões
    └── v0.1.0-SPECIFICATIONS.md # Primeira especificação
```

**Template de README.md inicial**:
```markdown
# [Nome do Projeto]

**Versão**: 0.1.0  
**Status**: Em desenvolvimento  
**Última Atualização**: [Data]

## 📋 Descrição

[Breve descrição do objetivo do projeto]

## 🎯 Funcionalidades Principais

- [ ] [Funcionalidade 1]
- [ ] [Funcionalidade 2]
- [ ] [Funcionalidade 3]

## 🛠️ Stack Tecnológico

**Linguagem**: [Linguagem principal]  
**Framework**: [Framework utilizado]  
**Banco de Dados**: [Se aplicável]

## 📚 Documentação

- [REQUIREMENTS.md](docs/REQUIREMENTS.md) - Requisitos detalhados
- [ARCHITECTURE.md](docs/ARCHITECTURE.md) - Decisões arquiteturais
- [TASKS.md](TASKS.md) - Gerenciamento de tarefas

## 🚀 Como Executar

[Instruções básicas de instalação e execução]

## 📝 Licença

[Licença do projeto]
```

**Template de docs/REQUIREMENTS.md inicial**:
```markdown
# Requisitos do Projeto - [Nome do Projeto]

**Versão**: 0.1.0  
**Data**: [Data de criação]  
**Autor**: [Nome do desenvolvedor]

## 🎯 Objetivo do Projeto

[Descrição detalhada do que o projeto deve alcançar]

## 👥 Usuários/Clientes

[Quem vai usar este sistema? Qual o perfil?]

## 📋 Requisitos Funcionais

### RF01 - [Nome do Requisito]
**Descrição**: [O que deve fazer]  
**Prioridade**: 🔴 Alta | 🟡 Média | 🟢 Baixa  
**Critérios de Aceitação**:
- [ ] [Critério 1]
- [ ] [Critério 2]

### RF02 - [Outro Requisito]
[...]

## ⚙️ Requisitos Não-Funcionais

### RNF01 - Performance
[Requisitos de performance esperados]

### RNF02 - Segurança
[Requisitos de segurança]

### RNF03 - Usabilidade
[Requisitos de usabilidade]

## 🚫 Restrições Técnicas

- [Restrição 1]
- [Restrição 2]

## 📊 Escopo

**Dentro do Escopo**:
- [Item 1]
- [Item 2]

**Fora do Escopo** (versões futuras):
- [Item 1]
- [Item 2]
```

**Template de TASKS.md inicial**:
```markdown
# Tarefas - [Nome do Projeto]

**Última Atualização**: [Data]

## 🔴 MUST HAVE - v0.1.0

### Infraestrutura
- [ ] Configurar ambiente de desenvolvimento
- [ ] Criar estrutura de diretórios
- [ ] Configurar controle de versão (Git)

### Documentação
- [x] Criar README.md
- [x] Criar REQUIREMENTS.md
- [x] Criar TASKS.md
- [ ] Criar ARCHITECTURE.md

### Desenvolvimento
- [ ] [Primeira funcionalidade a implementar]
- [ ] [Segunda funcionalidade a implementar]

## 🟡 SHOULD HAVE - v0.2.0
[Funcionalidades importantes mas não urgentes]

## 🟢 COULD HAVE - Futuro
[Funcionalidades desejáveis]

## 📊 Progresso
- **Concluídas**: 3 tarefas
- **Em Progresso**: 0 tarefas
- **Pendentes**: X tarefas
- **Total**: X tarefas
```

**Passo 5: Documentar evolução continuamente**

**Durante o desenvolvimento**, a IA deve:
- ✅ **Atualizar TASKS.md**: Marcar tarefas como concluídas
- ✅ **Criar SPECIFICATIONS.md**: Documentar cada versão implementada
- ✅ **Atualizar ARCHITECTURE.md**: Documentar decisões técnicas
- ✅ **Comentar código**: Adicionar comentários explicativos para compreensão

**Comentários no código** devem explicar:
- **Por quê** o código foi escrito daquela forma (não apenas "o que" faz)
- **Decisões não-óbvias**: Por quê escolheu abordagem X ao invés de Y
- **Edge cases**: Por quê certos casos especiais são tratados
- **TODOs**: O que falta implementar ou pode ser melhorado

**Exemplo de comentários úteis**:
```python
# DECISÃO: Usamos cache em memória ao invés de Redis porque:
# 1. Escala do projeto não justifica complexidade de Redis
# 2. Dados são pequenos (<10MB) e não precisam persistir
# 3. Startup rápido é prioridade (Redis adicionaria latência)
cache = {}

# TODO: Se escala ultrapassar 100k registros, migrar para Redis
# Estimativa: ~2h de trabalho, documentar em ADR
```

#### 📋 Checklist de Leitura de Documentação (Para IAs)

**Antes de iniciar QUALQUER tarefa**:

```markdown
[ ] 🔍 Busquei recursivamente por todos arquivos .md no projeto
[ ] 📖 Li 100% do conteúdo de TODOS os arquivos .md encontrados
[ ] 📝 Se não encontrei documentação, perguntei ao usuário se existe
[ ] 📚 Se não existe, criei estrutura mínima (README, REQUIREMENTS, TASKS)
[ ] 🎯 Entendi o objetivo e contexto completo do projeto
[ ] 📋 Sei quais tarefas estão pendentes e quais já foram concluídas
[ ] 🛠️ Conheço o stack tecnológico definido (se aplicável)
[ ] 🏗️ Entendi as decisões arquiteturais anteriores
[ ] ✅ Estou pronto para começar a trabalhar com contexto completo
```

**Somente após completar este checklist, prosseguir para as etapas seguintes.**

#### 🚀 Rationale

**Por quê ler 100% da documentação é PRIMEIRA ação obrigatória?**

1. ✅ **Contexto é Tudo**: Código sem contexto é impossível de manter
2. ✅ **Evita Duplicação**: Não reimplementar o que já existe
3. ✅ **Decisões Anteriores**: Entender por quê escolhas foram feitas
4. ✅ **Consistência**: Seguir padrões já estabelecidos no projeto
5. ✅ **Produtividade**: 10 minutos de leitura economizam horas de retrabalho
6. ✅ **Qualidade**: Código bem documentado desde o início

**Mensagem para IAs**:
> "NUNCA comece a codificar sem ler toda a documentação disponível. É como tentar continuar um livro sem ler os capítulos anteriores - você vai introduzir inconsistências, retrabalho e bugs. Invista 10-30 minutos lendo TUDO antes de escrever a primeira linha de código."

**Regra de Ouro**:
> **"Ler documentação PRIMEIRO, codificar DEPOIS. Sempre."**

---

**Após completar a leitura da documentação**, prosseguir para:
- Consultar `TASKS.md` (ou arquivo equivalente definido pelo usuário) para ver as tarefas pendentes
- Consultar `docs/REQUIREMENTS.md` para entender o contexto do projeto
- Revisar especificações anteriores (`v2.9.X-SPECIFICATIONS.md`)
- Entender dependências e arquitetura existente
- Verificar exemplos em `tests/files/` quando aplicável

**📋 Sobre o Arquivo de Tarefas**:

O arquivo `TASKS.md` é o **arquivo padrão** para gerenciar tarefas do projeto, mas você pode usar qualquer arquivo no formato ASCII (`.txt`, `.md`, etc.) conforme sua preferência.

**Requisitos do Arquivo de Tarefas**:
- ✅ **Formato ASCII obrigatório**: `.md`, `.txt` ou similar (legível como texto plano)
- ❌ **NÃO aceito**: `.docx`, `.pdf`, ou formatos binários
- 📍 **Localização**: Raiz do projeto ou em `docs/` (ex: `TASKS.md`, `TODO.md`, `requirements.md`)
- 🔄 **Alternativo**: Se preferir outro nome/localização, especifique no início do projeto

**Se não existir arquivo de tarefas**:
1. A IA deve perguntar ao usuário: "Qual arquivo você usa para gerenciar tarefas?" 
2. Se não houver, sugerir criação do `TASKS.md` padrão
3. Confirmar localização e nome do arquivo com o usuário

**Por quê?**: Evitar retrabalho e garantir coerência com o código existente. O arquivo de tarefas centraliza o planejamento e progresso do projeto.

**📋 Sobre Planos de Ação**:

Além do `TASKS.md`, você pode criar **Planos de Ação** para tarefas que requerem guia passo a passo detalhado.

**O que são Planos de Ação?**
- 🎯 **Roteiros práticos** com passos intermediários numerados para tarefas complexas
- ⚡ **Mais urgente e detalhado** que items do TASKS.md
- 🔧 **Aplicável a**: Manutenção, Correção, Evolução, Adaptação
- 📋 **Criados ANTES** de iniciar a implementação
- 📖 **Consultados sempre** durante o desenvolvimento

**Diferença entre TASKS.md e Planos de Ação:**
- **TASKS.md**: Lista de tarefas gerais ("O QUE fazer") - ex: `[ ] Implementar autenticação OAuth2`
- **Plano de Ação**: Guia detalhado de execução ("COMO fazer") - ex:
  ```
  PLANO #01: Implementar OAuth2
  ├─ Passo 1: Instalar biblioteca passport.js
  ├─ Passo 2: Configurar estratégia Google OAuth
  ├─ Passo 3: Criar rotas /auth/google
  └─ Passo 4: Adicionar testes
  ```

**Quando usar Planos de Ação:**
- ✅ Tarefa complexa com múltiplas etapas interdependentes
- ✅ Bug crítico que requer diagnóstico passo a passo
- ✅ Refatoração que afeta múltiplos módulos
- ✅ Migração de tecnologia ou atualização de framework

**Organização dos Planos de Ação:**

**Opção 1**: Arquivo consolidado `docs/ACTION_PLANS.md`  
**Opção 2**: Diretório de planos individuais `docs/plans/`
```
docs/
├── TASKS.md
├── ACTION_PLANS.md [opcional - índice]
└── plans/
    ├── plan-001-oauth2.md
    ├── plan-002-migration.md
    └── plan-003-refactoring.md
```

**Recomendação**: Use `docs/plans/` para projetos com múltiplas tarefas complexas.

**Campos Obrigatórios de um Plano de Ação:**
1. **📅 Data** (YYYY-MM-DD): Data de criação do plano
2. **🕐 Horário** (HH:MM): Horário de criação
3. **🎯 Função Principal**: Objetivo principal do plano
4. **📋 Requisito Desejado**: O que precisa ser alcançado
5. **✅ Resultado Esperado**: Critérios de sucesso mensuráveis
6. **📌 ID da Tarefa**: Vínculo com Task do TASKS.md (obrigatório)

**Template básico:**
```markdown
## 🎯 PLANO DE AÇÃO #[ID]: [Título]
**📅 Data**: YYYY-MM-DD
**🕐 Horário**: HH:MM
**⚡ Prioridade**: 🔴 Crítica | 🟡 Alta | 🟢 Normal
**🏷️ Tipo**: Manutenção | Correção | Evolução | Adaptação
**📌 ID da Tarefa**: Task #X do TASKS.md
**🎯 Função Principal**: [Objetivo do plano]
**📋 Requisito Desejado**: [O que deve ser alcançado]
**✅ Resultado Esperado**: [Critérios de sucesso]

### 📝 Contexto
[Por que este plano foi criado?]

### 📋 Passos Intermediários
- [ ] **Passo 1**: [Descrição + critério de conclusão]
- [ ] **Passo 2**: [Descrição + critério de conclusão]
[...]

### ✅ Critérios de Conclusão
- [ ] Todos passos concluídos
- [ ] Testes passando
- [ ] Documentação atualizada
```

**Fluxo de trabalho com Planos de Ação:**
1. Consultar TASKS.md para ver tarefas pendentes
2. Se tarefa complexa → **CRIAR Plano de Ação ANTES de começar**
3. Escolher localização: `docs/ACTION_PLANS.md` ou `docs/plans/plan-[ID]-[nome].md`
4. **ANTES de implementar**: Revisar e validar o plano
5. Executar passo a passo, **consultando o plano sempre que necessário**
6. Marcar progresso no plano durante a implementação
7. Ao concluir → marcar task no TASKS.md como completa
8. Arquivar plano em `docs/plans/archive/` ou seção "Histórico"

**Por quê criar ANTES e consultar SEMPRE?**
- ✅ **Planejamento Antecipado**: Identifica problemas antes de codificar
- ✅ **Evita Retrabalho**: Pensar antes de implementar economiza tempo
- ✅ **Guia Confiável**: Serve como mapa durante toda a implementação
- ✅ **Não se Perder**: Consultar durante o trabalho mantém foco nos passos
- ✅ **Manutenibilidade**: Futuros desenvolvedores entendem o processo

📖 **Detalhes completos sobre Planos de Ação**: Ver README.md do repositório, seção "🎯 Planos de Ação"

---

### 1️⃣.5️⃣ **Pesquisa de Tecnologias Adequadas ao Projeto** [OBRIGATÓRIO NO INÍCIO]

> **CRÍTICO PARA IAs**: No início do projeto (primeira sessão), a IA **DEVE** investigar e recomendar as tecnologias mais adequadas para o projeto com base nos requisitos fornecidos.

#### 🎯 Quando Aplicar

**Momento ideal**: Logo após a primeira leitura do `TASKS.md` e `docs/REQUIREMENTS.md`, **antes de começar a implementação**.

**Aplicável a**:
- ✅ Projetos novos (sem código implementado ainda)
- ✅ Projetos em refatoração completa (mudança de stack tecnológico)
- ✅ Projetos em fase de planejamento (arquitetura ainda não definida)

**NÃO aplicável a**:
- ❌ Projetos com stack já definido e implementação em andamento
- ❌ Manutenção de funcionalidades em código existente
- ❌ Correção de bugs em código já produzido

#### 📋 Como Funciona

**Passo 1: Coletar Requisitos do Desenvolvedor**

A IA deve solicitar ao desenvolvedor:
- 📌 **Tarefas e funcionalidades desejadas** (podem estar em `docs/TASKS.md`)
- 📌 **Requisitos funcionais e não-funcionais** (podem estar em `docs/REQUIREMENTS.md`)
- 📌 **Tipo de aplicação** (web, desktop, mobile, CLI, API, etc.)
- 📌 **Público-alvo e escala esperada** (MVP, pequeno porte, enterprise)
- 📌 **Restrições técnicas** (linguagens preferidas, limitações de infraestrutura)

**Exemplo de solicitação**:
```markdown
Para recomendar as tecnologias mais adequadas, preciso entender:

❓ 1. Qual o tipo de aplicação? (Web, Desktop, Mobile, CLI, API, etc.)
❓ 2. Quais são as funcionalidades principais? (ex: autenticação, CRUD, dashboards, etc.)
❓ 3. Qual a escala esperada? (MVP/protótipo, pequeno porte, médio porte, enterprise)
❓ 4. Há preferência por linguagens/frameworks específicos? (ex: Python, JavaScript, Java)
❓ 5. Há restrições técnicas? (ex: deve rodar offline, baixo consumo de memória)

💡 Sugestão: Se estiver começando, posso recomendar stacks modernas e produtivas.
```

**Passo 2: Investigar Tecnologias Profissionais**

Com base nos requisitos, a IA deve **pesquisar** (online se necessário) quais tecnologias são **amplamente utilizadas de forma profissional** para projetos similares.

**Categorias de tecnologias a investigar**:

1. **🎨 Frontend** (se aplicável):
   - Frameworks: React, Vue, Angular, Next.js, Svelte
   - UI Libraries: Material-UI (MUI), Ant Design, Chakra UI, Bootstrap, Tailwind CSS
   - Estado: Redux, Zustand, Jotai, React Query

2. **⚙️ Backend** (se aplicável):
   - Linguagens: Python, JavaScript/TypeScript (Node.js), Java, Go, C#
   - Frameworks: Django, FastAPI, Express, NestJS, Spring Boot, ASP.NET Core
   - APIs: REST, GraphQL, gRPC

3. **🖥️ Desktop** (se aplicável):
   - Python: PyQt, PySide, Tkinter, Kivy
   - JavaScript: Electron, Tauri
   - C++: Qt, wxWidgets
   - C#: WPF, WinForms

4. **📊 Visualização de Dados** (se aplicável):
   - Web: Chart.js, D3.js, Recharts, Victory
   - Python: Matplotlib, Plotly, Seaborn, pyqtgraph

5. **🤖 Inteligência Artificial/ML** (se aplicável):
   - Frameworks: TensorFlow, PyTorch, scikit-learn, Transformers (Hugging Face)
   - APIs: OpenAI API, Gemini API, Anthropic API, Cohere
   - Processamento de Linguagem Natural: spaCy, NLTK, Transformers

6. **💾 Banco de Dados** (se aplicável):
   - Relacional: PostgreSQL, MySQL, SQLite
   - NoSQL: MongoDB, Redis, Cassandra
   - ORMs: SQLAlchemy, Prisma, TypeORM, Sequelize

7. **🔐 Autenticação e Segurança** (se aplicável):
   - OAuth: Passport.js, Auth0, Keycloak
   - JWT: jsonwebtoken, PyJWT
   - Criptografia: bcrypt, Argon2

8. **🧪 Testes** (se aplicável):
   - Python: pytest, unittest
   - JavaScript: Jest, Vitest, Mocha, Cypress
   - Java: JUnit, TestNG

#### 🌐 **Stack Padrão Recomendado para Sites/Aplicações Web** [NOVO]

> **IMPORTANTE**: Quando se tratar da implementação de um **site ou aplicação web**, e o usuário **NÃO especificar** quais tecnologias deseja, a IA **PODE RECOMENDAR** o seguinte stack padrão moderno e completo:

**📦 Frontend Framework & Runtime**
- **Next.js 15.5.2** - Framework React com App Router e Server Components
- **React 19.1.1** - Biblioteca de UI
- **React DOM 19.1.1** - Renderização do React no navegador
- **TypeScript 5.9.2** - Superset JavaScript com tipagem estática
- **Node.js 18+** - Runtime JavaScript

**🔧 Bundlers & Build Tools**
- **Turbopack** - Bundler de nova geração do Next.js (700x mais rápido)
- **Turbo (turborepo)** - Sistema de build para monorepos
- **PostCSS 8.5.6** - Processamento de CSS
- **Autoprefixer 10.4.21** - Adiciona prefixos CSS automaticamente

**📊 State Management**
- **Zustand 4.5.7** - Gerenciamento de estado minimalista e eficiente
- **Immer 10.1.3** - Manipulação imutável de estado

**🎨 Styling**
- **Tailwind CSS 3.4.17** - Framework CSS utility-first
- **CSS Modules** - Modularização de CSS
- **clsx 2.1.1** - Utilitário para classes CSS condicionais
- **class-variance-authority 0.7.1** - Gerenciamento de variantes de componentes
- **tailwind-merge 3.3.1** - Merge inteligente de classes Tailwind
- **Lucide React 0.542.0** - Biblioteca de ícones

**🎵 Audio & Media** (se aplicável)
- **Cloudinary 1.41.3** - Processamento e armazenamento de mídia
- **@cloudinary/react 1.14.3** - Componentes React do Cloudinary
- **@cloudinary/url-gen 1.22.0** - Geração de URLs do Cloudinary
- **Web Audio API** - API nativa do navegador para gravação de áudio

**💳 Payments & Subscriptions** (se aplicável)
- **Stripe 14.25.0** - Processamento de pagamentos (backend)
- **@stripe/stripe-js 2.4.0** - SDK JavaScript do Stripe (frontend)

**🌐 HTTP & API**
- **Axios 1.11.0** - Cliente HTTP para requisições à API

**📄 PDF & Screenshots** (se aplicável)
- **jsPDF 3.0.3** - Geração de PDFs
- **html2canvas 1.4.1** - Conversão de HTML para canvas/imagem
- **Puppeteer 24.29.1** - Automação de browser headless

**🧪 Testing**
- **Jest** - Framework de testes
- **jsdom** - Ambiente DOM para testes
- **@testing-library** - Utilitários para testes de componentes React

**✅ Code Quality & Linting**
- **ESLint 8.57.1** - Linter JavaScript/TypeScript
- **eslint-config-next 15.5.2** - Configuração ESLint do Next.js
- **Husky 9.1.7** - Git hooks para qualidade de código

**🛠️ Development Tools**
- **npm 10.9.2** - Gerenciador de pacotes
- **Git** - Controle de versão
- **VS Code** - Editor recomendado

**⚙️ Backend** (Repositório Separado)
- **Node.js** - Runtime backend
- **Express** - Framework web
- **MongoDB** - Banco de dados NoSQL
- **JWT** - Autenticação com tokens
- **Heroku** - Hospedagem do backend

**🚀 Infraestrutura & Deploy**
- **Vercel** - Hospedagem frontend (recomendado para Next.js)
- **Cloudinary CDN** - Entrega de conteúdo de áudio/mídia
- **HTTPS** - Protocolo seguro (requerido para gravação de áudio)

**🤖 APIs de IA** (Opcionais)
- **OpenAI API** - IA para feedback e avaliação
- **ElevenLabs API** - Síntese de voz

**✅ Por Quê Este Stack Padrão?**
- ✅ **Next.js 15** com App Router: SSR, SSG, performance otimizada
- ✅ **React 19**: Versão mais recente com Server Components
- ✅ **TypeScript**: Segurança de tipos e melhor DX
- ✅ **Tailwind CSS**: Produtividade e design consistente
- ✅ **Zustand**: State management simples e eficiente
- ✅ **Turbopack**: Build extremamente rápido (700x vs Webpack)
- ✅ **Vercel**: Deploy otimizado para Next.js (mesmo criador)
- ✅ **Ecossistema Completo**: Cobre 90% dos casos de uso web

**⚠️ Quando NÃO Usar Este Stack Padrão**:
- ❌ Usuário especifica **explicitamente** outras tecnologias
- ❌ Projeto requer **Vue/Angular** ao invés de React
- ❌ Necessita de **Python/Django** backend (use FastAPI + React)
- ❌ Aplicação **desktop** ou **mobile nativa** (não é web)
- ❌ Site **estático simples** (HTML/CSS/JS puro pode ser suficiente)

**📋 Exemplo de Apresentação ao Usuário**:
```markdown
❓ Você não especificou tecnologias para o site. Posso recomendar um stack moderno?

**Stack Padrão Recomendado (Next.js 15 + React 19 + TypeScript)**:

**Frontend**:
- Next.js 15.5.2 (framework React SSR/SSG)
- React 19.1.1 + TypeScript 5.9.2
- Tailwind CSS 3.4.17 (styling)
- Zustand 4.5.7 (state management)

**Build & Deploy**:
- Turbopack (bundler 700x mais rápido)
- Vercel (hospedagem otimizada)

**Backend** (opcional):
- Node.js + Express + MongoDB
- Deploy em Heroku

**Por quê?**
- ✅ Stack moderno e profissional
- ✅ Performance excepcional (SSR + Turbopack)
- ✅ SEO otimizado (Next.js App Router)
- ✅ TypeScript garante qualidade
- ✅ Deploy gratuito em Vercel

**Você concorda ou prefere outro stack?** (Vue, Angular, etc.)
```

**🎯 Quando Oferecer Este Stack**:
1. Usuário pediu "criar um site" ou "aplicação web"
2. Usuário NÃO especificou tecnologias específicas
3. Não há restrições técnicas óbvias
4. Projeto é novo (não é manutenção de código existente)

---

**Exemplo de investigação**:
```markdown
Baseado em seus requisitos:
- Aplicação Web com Dashboard e Gráficos
- Autenticação de usuários
- API REST
- Escala média (até 10k usuários)

Pesquisei projetos profissionais similares e identifiquei:

**Stack Recomendada #1 (Python Full-Stack)**:
- Backend: FastAPI (rápido, moderno, tipado)
- Frontend: React + Material-UI (componentes prontos)
- Gráficos: Recharts ou Plotly
- Banco de Dados: PostgreSQL
- Autenticação: JWT + OAuth2
- Testes: pytest + Jest

**Stack Recomendada #2 (JavaScript/TypeScript Full-Stack)**:
- Backend: NestJS (arquitetura escalável)
- Frontend: Next.js + Chakra UI
- Gráficos: Chart.js
- Banco de Dados: PostgreSQL + Prisma ORM
- Autenticação: NextAuth.js
- Testes: Jest + Playwright

**Por quê estas recomendações?**
- ✅ Amplamente utilizadas em produção
- ✅ Grande comunidade e suporte
- ✅ Documentação robusta
- ✅ Performance comprovada
- ✅ Ecossistema maduro de bibliotecas

❓ Qual stack prefere? Ou tem alguma restrição adicional?
```

**Passo 3: Apresentar Recomendações com Justificativas**

A IA deve apresentar **2-3 stacks tecnológicos completos** com:
- ✅ Lista de tecnologias recomendadas
- ✅ Justificativa para cada escolha (por quê é adequada)
- ✅ Casos de uso reais (empresas/projetos que usam)
- ✅ Vantagens e desvantagens
- ✅ Complexidade de aprendizado (iniciante, intermediário, avançado)

**Template de recomendação**:
```markdown
## 🎯 Stack Recomendada: [Nome da Stack]

### 📦 Tecnologias Principais

**Frontend**:
- [Tecnologia X] - [Justificativa: por quê é adequada]
- [Tecnologia Y] - [Justificativa]

**Backend**:
- [Tecnologia Z] - [Justificativa]

**Banco de Dados**:
- [Tecnologia W] - [Justificativa]

### ✅ Vantagens
- [Vantagem 1]
- [Vantagem 2]

### ⚠️ Desvantagens/Desafios
- [Desvantagem 1]
- [Desvantagem 2]

### 🏢 Casos de Uso Reais
- [Empresa/Projeto 1] usa [Tecnologia X] para [Propósito]
- [Empresa/Projeto 2] usa [Tecnologia Y] para [Propósito]

### 📚 Complexidade de Aprendizado
- Iniciante: [Lista de tecnologias fáceis]
- Intermediário: [Lista de tecnologias médias]
- Avançado: [Lista de tecnologias complexas]

### ⏱️ Tempo Estimado de Setup
- Configuração inicial: [X horas]
- Primeira funcionalidade: [Y horas]
- MVP completo: [Z dias/semanas]
```

**Passo 4: Validar com o Desenvolvedor**

Após apresentar as recomendações, a IA **DEVE**:
- ✅ Perguntar ao desenvolvedor qual stack prefere
- ✅ Permitir ajustes e substituições
- ✅ Confirmar decisão final antes de começar
- ✅ Documentar stack escolhido em `docs/REQUIREMENTS.md` ou `docs/ARCHITECTURE.md`

#### 🌐 Pesquisas Online (Se Necessário)

Se a IA tiver dúvidas ou precisar de informações atualizadas, **pode e deve fazer pesquisas online**:

**Fontes recomendadas**:
- 📚 **GitHub**: Repositórios similares, análise de stars/forks, issues
- 📖 **Documentação oficial**: Sites oficiais das tecnologias
- 💬 **Stack Overflow**: Discussões sobre comparações e melhores práticas
- 📊 **Stack Share**: Empresas que usam cada tecnologia
- 📰 **Blogs técnicos**: Medium, Dev.to, blogs de empresas (Netflix, Airbnb, etc.)

**O que pesquisar**:
- "Best [tipo de app] stack 2025"
- "[Linguagem] frameworks for [tipo de app]"
- "[Tecnologia X] vs [Tecnologia Y] comparison"
- "Companies using [Tecnologia Z]"
- "[Framework W] production readiness"

#### 📝 Documentar Stack Tecnológico Escolhido

**Onde documentar**: `docs/ARCHITECTURE.md` ou `docs/REQUIREMENTS.md`

**O que documentar**:
```markdown
## 🛠️ Stack Tecnológico

**Linguagem Principal**: [Python, JavaScript, etc.]

**Frontend**:
- Framework: [React, Vue, etc.]
- UI Library: [MUI, Bootstrap, etc.]
- Gráficos: [Chart.js, etc.]

**Backend**:
- Framework: [FastAPI, Express, etc.]
- API: [REST, GraphQL]

**Banco de Dados**:
- Tipo: [PostgreSQL, MongoDB, etc.]
- ORM: [SQLAlchemy, Prisma, etc.]

**IA/ML** (se aplicável):
- Framework: [TensorFlow, Transformers, etc.]
- APIs: [Gemini API, OpenAI API, etc.]

**Testes**:
- Framework: [pytest, Jest, etc.]

**Infraestrutura** (se relevante):
- Deploy: [Docker, Vercel, AWS, etc.]
- CI/CD: [GitHub Actions, GitLab CI, etc.]

**Justificativa da Escolha**:
[Breve explicação do por quê esta stack foi escolhida para este projeto]
```

#### ✅ Checklist de Pesquisa de Tecnologias

Antes de começar a implementação, a IA deve confirmar:

```markdown
[ ] Requisitos do projeto coletados (funcionalidades, tipo de app, escala)
[ ] Investigação de tecnologias profissionais realizada
[ ] 2-3 stacks completos recomendados com justificativas
[ ] Vantagens e desvantagens apresentadas
[ ] Casos de uso reais citados
[ ] Complexidade de aprendizado avaliada
[ ] Validação com desenvolvedor realizada
[ ] Stack final escolhido e confirmado
[ ] Stack documentado em docs/ARCHITECTURE.md ou docs/REQUIREMENTS.md
[ ] Pesquisas online realizadas (se necessário para dúvidas)
```

#### 🎯 Exemplos Práticos

**Exemplo 1: Dashboard de Análise de Dados**

**Requisitos**:
- Dashboard web interativo
- Gráficos dinâmicos
- API REST para buscar dados
- Autenticação básica

**Stack Recomendada**:
- Frontend: React + Recharts + MUI
- Backend: FastAPI (Python)
- Banco: PostgreSQL
- Auth: JWT

**Justificativa**: Stack moderna, produtiva, com excelente suporte para visualização de dados.

**Exemplo 2: Aplicação Desktop para Processamento de Sinais**

**Requisitos**:
- Interface desktop nativa
- Gráficos em tempo real
- Processamento local (offline)
- Performance crítica

**Stack Recomendada**:
- GUI: PyQt6 ou PySide6
- Gráficos: pyqtgraph (otimizado para tempo real)
- Backend: Python com NumPy/SciPy

**Justificativa**: PyQt oferece performance nativa, pyqtgraph é especializado em plotagem em tempo real.

**Exemplo 3: API com IA Generativa**

**Requisitos**:
- API REST para processamento de linguagem natural
- Integração com modelos de IA (GPT, Gemini)
- Escalabilidade para múltiplas requisições

**Stack Recomendada**:
- Backend: Node.js + NestJS
- IA: Transformers (Hugging Face) + Gemini API
- Banco: MongoDB (documentos não-estruturados)
- Testes: Jest

**Justificativa**: NestJS oferece arquitetura escalável, Node.js tem excelente suporte assíncrono para APIs de IA.

#### 🚀 Rationale

**Por quê esta etapa é obrigatória no início?**

1. ✅ **Evita Retrabalho**: Escolher stack errado no início pode exigir reescrever todo o código
2. ✅ **Qualidade Profissional**: Usar tecnologias adequadas garante código production-ready
3. ✅ **Produtividade**: Stack moderna e bem suportada acelera desenvolvimento
4. ✅ **Manutenibilidade**: Tecnologias populares têm mais recursos, documentação e comunidade
5. ✅ **Escalabilidade**: Stack adequada cresce com o projeto sem necessidade de migração
6. ✅ **Conhecimento Contextual**: IA pode pesquisar e recomendar tecnologias que o desenvolvedor não conhece

**Mensagem para IAs**:
> "Não assuma que o desenvolvedor já conhece todas as opções. Sua pesquisa e recomendação podem introduzir tecnologias modernas e mais adequadas. Investir 30 minutos nesta investigação pode economizar semanas de retrabalho."

**Regra de Ouro**:
> **"Stack tecnológico DEVE ser definido ANTES da primeira linha de código. Mudanças posteriores são custosas."**

---

### 2️⃣ **Escolher as Tarefas Mais Simples**
- **Regra de Ouro**: Sempre começar pelas tarefas **mais fáceis de implementar**
- Mesmo em uma lista de tarefas complexas, **sempre há umas mais simples que outras**
- Proporcionalidade: equilibrar simplicidade vs. impacto

**Critérios de Simplicidade**:
- ✅ Menor número de dependências
- ✅ Escopo bem definido e claro
- ✅ Menor quantidade de arquivos a modificar
- ✅ Menor risco de quebrar funcionalidades existentes
- ✅ Pode ser testada isoladamente

**Exemplo Real**:
```
Lista de tasks complexas restantes:
[ ] Complex Feature Example (MUITO COMPLEXO - 50h)
[ ] Busca com IA semântica (COMPLEXO - 20h)
[ ] Tooltip preview em hover (SIMPLES - 30min) ✅ COMEÇAR POR AQUI!
```

---

### 2️⃣.5️⃣ **Organização Ordinal de Tarefas** [OPCIONAL]

> **NOVO**: Sistema de prefixos ordinais para identificar dependências e paralelização.

**Quando Usar**: Projetos com >10 tarefas interdependentes ou equipes trabalhando em paralelo.

#### 📊 Sistema de Prefixos

**Nível 1: Numeração Simples** (tarefas independentes)
```markdown
1. Tarefa A - Configurar ambiente
2. Tarefa B - Criar documentação
3. Tarefa C - Definir arquitetura
```
→ Podem ser executadas em **qualquer ordem** ou **paralelamente**

**Nível 2: Hierarquia com Letras** (grupos de tarefas)
```markdown
A. Infrastructure
   A.1. Criar estrutura de diretórios
   A.2. Configurar dependências
   
B. Core - Estruturas de Dados
   B.1. Implementar classe Node
   B.2. Implementar ExpressionTree
```
→ Grupos diferentes (A, B) são **PARALELOS**

**Nível 3: Hierarquia Profunda** (dependências complexas)
```markdown
B.C.2. Implementar conversão árvore → RPN
   B.C.2.1. Parser RPN (fazer PRIMEIRO - folha)
   B.C.2.2. Serializer RPN (fazer PRIMEIRO - folha)
   B.C.2. Conversão completa (fazer DEPOIS - pai)
```

**Leitura da hierarquia** (⭐ CRÍTICO): Ler da **DIREITA para ESQUERDA**
```
C.B.1.D.1
   │  │ │ └─ 1: Executar por ÚLTIMO (raiz)
   │  │ └─── D: Executar TERCEIRO
   │  └───── 1: Executar SEGUNDO
   └──────── B: Executar PRIMEIRO (folha)
```

#### 🔄 Paralelização vs Serialização

✅ **PARALLEL** (podem ser simultâneos):
- Tarefas de grupos diferentes (A.x, B.x, C.x)
- Irmãos no mesmo nível (X.1, X.2, X.3)
- Tarefas sem dependências explícitas

❌ **SERIAL** (devem ser sequenciais):
- Relação pai-filho (B.C.2.1, B.C.2.2 → B.C.2)
- Dependências explícitas
- Quando uma tarefa usa resultado de outra

#### 📋 Exemplo Prático

```markdown
A. Autenticação
   🔴🟡 [ ] A.1. Modelo User (1.5h)
   🔴🟡 [ ] A.2. Login JWT (2h) - Depende: A.1
   🔴🔴 [ ] A.3. 2FA (3h) - Depende: A.2

B. Catálogo de Produtos
   🔴🟢 [ ] B.1. Modelo Product (1h)
   🔴🟡 [ ] B.2. CRUD Products (2h) - Depende: B.1

**Análise**:
- A.1 e B.1 são PARALELOS (grupos diferentes)
- A.1 → A.2 → A.3 são SERIAIS (mesmo grupo)
- B.1 → B.2 são SERIAIS (mesmo grupo)

**Estratégia de Branches**:
- Branch feat/auth: A.1 → A.2 → A.3
- Branch feat/catalog: B.1 → B.2 (parallel com auth)
```

#### ✅ Benefícios

Para **Desenvolvedores**:
- ✅ Clareza sobre qual tarefa fazer primeiro
- ✅ Identifica oportunidades de paralelização
- ✅ Minimiza conflitos em controle de versão

Para **IAs**:
- ✅ Cálculo automático de ordem de execução
- ✅ Sugestão de paralelização
- ✅ Detecção de dependências circulares

Para o **Projeto**:
- ✅ Reduz tempo total (paralelização)
- ✅ Evita retrabalho (ordem correta)
- ✅ Timeline mais previsível

📘 **Documentação Completa**: Ver `ORGANIZACAO_ORDINAL_TAREFAS.md` para detalhes completos, exemplos e fluxogramas.

---

### 3️⃣ **Fazer Perguntas e Mais Perguntas ao Programador**
- **CRÍTICO**: Nunca assumir ou adivinhar requisitos
- Fazer **todas as perguntas necessárias** até sanar **100% das dúvidas**
- Validar entendimento antes de começar a implementar
- 🤖 **[NOVO v1.9]** A IA **PODE e É ALTAMENTE RECOMENDADA** fornecer **sugestões e palpites** de resposta para cada pergunta (opcional, mas incentivado)

**Formato Recomendado de Perguntas com Sugestões**:
```
❓ Pergunta: "Como deve se comportar quando [cenário X]?"
💡 Sugestão da IA: "Baseado no código existente, sugiro [opção A] porque [razão Y]."
Opções: A) [opção A] | B) [opção B] | C) [opção C]
```

**Por Quê Sugestões da IA São Importantes**:
- ✅ Acelera decisões quando o programador está indeciso
- ✅ IA tem contexto do código existente e pode sugerir padrões consistentes
- ✅ Reduz carga cognitiva do programador (ele apenas valida, não cria do zero)
- ✅ Mantém qualidade: IA sugere baseado em boas práticas já implementadas

**Categorias de Perguntas**:
1. **Requisitos Funcionais**:
   - "Como deve se comportar quando [cenário X]?"
   - "O que acontece se o usuário [ação Y]?"
   - "Qual é a prioridade entre [opção A] e [opção B]?"

2. **Requisitos Técnicos**:
   - "Devo usar [biblioteca X] ou criar do zero?"
   - "Qual é o formato esperado do output?"
   - "Há alguma restrição de performance?"

3. **Edge Cases**:
   - "E se o arquivo estiver vazio?"
   - "E se houver caracteres especiais?"
   - "Como tratar valores None/null?"

4. **Integração**:
   - "Precisa integrar com [módulo existente]?"
   - "Devo manter compatibilidade com [versão anterior]?"
   - "Onde salvar os resultados?"

5. **Validação de Entendimento**:
   - "Entendi que você quer [X]. Está correto?"
   - "Minha solução proposta é [Y]. Faz sentido?"
   - "Posso começar ou há algo que esqueci?"

**Exemplo de Validação de Requisitos**:
```
❓ "Quantos caracteres/elementos devem ser processados? (default: 30?)"
✅ Resposta: "Default pode ser 30 caracteres"

❓ "Deve aplicar normalização de texto (remover acentos, converter case)?"
✅ Resposta: "Sim, devem ser normalizados"

❓ "Como resolver conflitos quando houver duplicatas?"
✅ Resposta: "Usar critério de prioridade específico (ex: mais antigo vence)"
```

**Por quê?**: Economiza tempo, evita retrabalho, garante que a solução atende exatamente o que foi pedido.

#### 🌐 **Pesquisas Online: Quando a IA Tem Muitas Dúvidas ou Dificuldades**

> **IMPORTANTE PARA IAs**: Se você está com **muitas dúvidas** sobre como resolver um determinado problema, ou tem **dificuldades significativas** para resolver esse mesmo problema, **lembre-se de que você pode efetuar pesquisas online**.

**Quando Realizar Pesquisas Online**:
- ✅ Quando há dúvidas técnicas complexas que não consegue resolver sozinho
- ✅ Quando encontra um problema crítico que não tem solução óbvia no código existente
- ✅ Quando precisa entender como implementar algo completamente novo
- ✅ Quando há um erro ou bug difícil de diagnosticar
- ✅ Quando precisa de exemplos práticos de implementação

**Onde Pesquisar** (em ordem de prioridade):
1. **📚 Documentação Oficial do GitHub de Projetos Relacionados**:
   - Repositórios similares ou que resolvem problemas parecidos
   - Issues e Pull Requests que discutem problemas similares
   - Wiki e documentação técnica de projetos open source relacionados

2. **📖 Plataformas de Documentação Online**:
   - Documentação oficial das bibliotecas e frameworks usados no projeto
   - Tutoriais e guias técnicos especializados
   - Blogs técnicos e artigos de desenvolvedores experientes

3. **💬 Plataformas de Perguntas e Respostas**:
   - **StackOverflow**: Principal plataforma para dúvidas de programação
   - **GitHub Discussions**: Para questões específicas de projetos
   - Outras comunidades técnicas relevantes para a tecnologia do projeto

**Por Quê Pesquisas Online São Importantes**:
- ✅ **Economiza tempo**: Problemas complexos já podem ter soluções documentadas
- ✅ **Melhores práticas**: Aprenda com implementações já validadas pela comunidade
- ✅ **Evita reinventar a roda**: Muitos problemas já foram resolvidos por outros desenvolvedores
- ✅ **Reduz erros**: Soluções testadas e aprovadas pela comunidade têm menos bugs
- ✅ **Atualização**: Descubra as abordagens mais modernas e eficientes

**Exemplo de Fluxo com Pesquisa Online**:
```
1. ❓ Tentei implementar [funcionalidade X] mas encontrei [problema Y]
2. 🔍 Pesquisei no GitHub: "similar implementation [funcionalidade X]"
3. 📚 Encontrei 3 projetos similares que resolvem isso de formas diferentes
4. 💡 Analisei os exemplos e identifiquei a abordagem mais adequada para nosso contexto
5. ✅ Implementei baseado nas melhores práticas encontradas
6. 📝 Documentei a fonte da solução para referência futura
```

**⚠️ Importante**: Sempre cite as fontes consultadas na documentação do projeto para referência futura e rastreabilidade.

---

### 4️⃣ **Analisar e Estudar o Projeto**
- **CRÍTICO**: Após sanar todas as dúvidas, **estudar o código antes de implementar**
- Ler documentação relevante (README, docs/, comentários no código)
- Entender arquitetura existente e padrões utilizados
- Verificar dependências e imports necessários
- Identificar funções/classes reutilizáveis

**Checklist de Análise**:
1. **Leitura de Documentação**:
   - `docs/` - Contexto geral do projeto e especificações
   - Documentos de design e arquitetura
   - `README.md` - Visão geral e instruções de uso
   - Docstrings de módulos relacionados

2. **Análise de Código Existente**:
   - Encontrar módulos similares ao que será implementado
   - Identificar padrões de design já utilizados (GoF, GRASP)
   - Verificar convenções de nomenclatura e estrutura
   - Localizar funções auxiliares reutilizáveis

3. **Mapeamento de Dependências**:
   - Quais módulos precisam ser importados?
   - Há conflitos de nomes ou versões?
   - Quais classes base ou mixins devem ser herdadas?
   - Onde os novos arquivos devem ser criados?

4. **Validação de Compatibilidade**:
   - A solução quebrará código existente?
   - É necessário refatorar algo antes de implementar?
   - Há testes que precisam ser atualizados?
   - A API pública será mantida?

**Por quê?**: Evita refatorações, economiza tempo, garante código consistente com a base existente.

**Exemplo de Análise de Código Existente**:
```
✅ Analisado: Implementações similares existentes no projeto
✅ Identificado: Padrões de classes base e mixins utilizados
✅ Verificado: Widgets e componentes UI reutilizáveis
✅ Estudado: Como outros módulos resolvem problemas semelhantes
✅ Localizado: Onde adicionar novos imports no código principal
✅ Confirmado: Estrutura de integração com sistema existente
→ Resultado: Implementação mais rápida e consistente (economia de 60%)
```

#### 🔀 **Princípio de Opções Paralelas (Multi-Choice)**

> **IMPORTANTE**: Quando há múltiplas opções válidas e **não mutuamente exclusivas**, considere implementar **AMBAS** ao invés de escolher apenas uma, permitindo ao usuário decidir qual usar.

**Conceito**:
Muitas vezes durante a análise identificamos que existem **duas ou mais formas válidas** de apresentar/processar/visualizar algo. Ao invés de escolher arbitrariamente uma opção, implemente ambas e deixe o usuário escolher.

**Exemplos de Opções Paralelas**:

1. **Visualização de Dados**:
   - ❌ **Ruim**: Escolher entre tabela OU árvore
   - ✅ **Bom**: Implementar tabela E árvore (usuário alterna com flag/botão)
   
   ```python
   # Implementar ambas as visualizações
   def display_files(files, mode='table'):
       """
       Exibe arquivos em diferentes formatos.
       
       Args:
           mode: 'table' ou 'tree' (padrão: 'table')
       """
       if mode == 'table':
           display_as_table(files)
       elif mode == 'tree':
           display_as_tree(files)
       else:
           raise ValueError(f"Modo '{mode}' inválido. Use 'table' ou 'tree'")
   
   # CLI: programa --display=table ou --display=tree
   # GUI: Botões "Ver como Tabela" | "Ver como Árvore"
   ```

2. **Formato de Saída**:
   - ❌ **Ruim**: Escolher entre JSON OU CSV
   - ✅ **Bom**: Exportar em JSON E CSV (flag `--format`)
   
   ```python
   def export_data(data, format='json'):
       """Exporta dados em múltiplos formatos."""
       if format == 'json':
           return export_to_json(data)
       elif format == 'csv':
           return export_to_csv(data)
       elif format == 'xml':
           return export_to_xml(data)
   
   # CLI: programa --export=json|csv|xml
   ```

3. **Ordenação**:
   - ❌ **Ruim**: Escolher entre ordenar por nome OU data
   - ✅ **Bom**: Permitir ordenação por nome E data E tamanho
   
   ```python
   def list_files(sort_by='name', reverse=False):
       """
       Lista arquivos com opções de ordenação.
       
       Args:
           sort_by: 'name', 'date', 'size', 'type'
           reverse: True para ordem decrescente
       """
       # Implementa todos os tipos de ordenação
   ```

4. **Nível de Detalhe**:
   - ❌ **Ruim**: Escolher entre resumo OU detalhado
   - ✅ **Bom**: Oferecer resumo E detalhado E verboso
   
   ```python
   def show_info(level='normal'):
       """
       Exibe informações em diferentes níveis.
       
       Args:
           level: 'brief', 'normal', 'detailed', 'verbose'
       """
   ```

**Quando Aplicar Opções Paralelas**:

✅ **SIM - Implemente ambas quando**:
- Ambas as opções são **igualmente válidas**
- Usuários diferentes têm **preferências diferentes**
- O custo de implementação é **razoável** (não duplica esforço significativamente)
- Não há **contradição lógica** entre as opções
- Melhora significativamente a **experiência do usuário**

❌ **NÃO - Escolha uma quando**:
- As opções são **mutuamente exclusivas** (impossível ter ambas)
- Implementar ambas **dobra o trabalho** sem benefício proporcional
- Uma opção é **claramente superior** em 90% dos casos
- Há **restrições técnicas** que impedem ambas
- Adiciona **complexidade excessiva** à interface

**⚠️ CRÍTICO: Notificar o Usuário/Desenvolvedor ANTES**

> **OBRIGATÓRIO**: Antes de implementar opções paralelas, **perguntar ao usuário** para evitar que seja tratado como "feature creep" ou aumento de escopo não solicitado.

**Template de Notificação**:
```markdown
❓ **Sugestão de Opções Paralelas**

Durante a análise, identifiquei que há **duas formas válidas** de [funcionalidade]:

**Opção A**: [Descrição - ex: Exibir como tabela]
- Vantagem: [ex: Compacto, fácil comparação]
- Desvantagem: [ex: Dificulta ver hierarquia]

**Opção B**: [Descrição - ex: Exibir como árvore]
- Vantagem: [ex: Mostra hierarquia claramente]
- Desvantagem: [ex: Ocupa mais espaço vertical]

**Proposta**: Implementar **AMBAS** e permitir usuário escolher via:
- CLI: Flag `--display=table|tree` (padrão: table)
- GUI: Botão de alternância "Tabela ⇄ Árvore"

**Esforço adicional estimado**: ~30 minutos (implementar segunda visualização + controle)

**Benefício**: Usuário escolhe formato que prefere, sem perder funcionalidade.

**Você autoriza implementar ambas as opções?**
A) ✅ Sim, implementar ambas
B) ❌ Não, escolher apenas [Opção A | Opção B]
```

**Exemplo Real - Caso de Uso**:

```python
# Contexto: Usuário pediu "listar arquivos do projeto"
# Análise: Identificamos 2 visualizações possíveis

# ANTES (escolher arbitrariamente):
def list_files():
    """Lista arquivos em formato tabela."""
    # Apenas formato tabela
    display_table(files)

# DEPOIS (opções paralelas):
def list_files(display_mode='table', show_hidden=False):
    """
    Lista arquivos do projeto em múltiplos formatos.
    
    Args:
        display_mode: 'table' (padrão), 'tree', ou 'flat'
        show_hidden: Incluir arquivos ocultos (padrão: False)
    
    Exemplos:
        >>> list_files('table')        # Tabela compacta
        >>> list_files('tree')         # Árvore hierárquica
        >>> list_files('flat')         # Lista simples
    """
    files = get_project_files(show_hidden)
    
    if display_mode == 'table':
        display_as_table(files)
    elif display_mode == 'tree':
        display_as_tree(files)
    elif display_mode == 'flat':
        display_as_flat_list(files)
    else:
        raise ValueError(f"Modo '{display_mode}' inválido")

# CLI suporta: programa list --display=tree
# GUI tem dropdown: [Tabela ▼] [Árvore] [Lista]
```

**Benefícios**:
1. ✅ **Flexibilidade**: Usuário escolhe o que prefere
2. ✅ **Acessibilidade**: Diferentes usuários têm diferentes necessidades
3. ✅ **Profissionalismo**: Software mais completo e maduro
4. ✅ **Evita debates**: Não precisa "escolher o melhor", oferece ambos
5. ✅ **Evolução natural**: Fácil adicionar mais opções depois

**Antipadrões a Evitar**:
- ❌ Implementar opção sem avisar usuário (feature creep)
- ❌ Fazer todas as opções por padrão simultaneamente (confuso)
- ❌ Implementar 10 opções quando 2-3 são suficientes
- ❌ Opções que contradizem entre si
- ❌ Interface complexa demais para escolher opção

**Mensagem para IAs**:
> "Quando identificar múltiplas formas válidas de implementar algo, sempre PERGUNTE ao usuário se deseja implementar opções paralelas antes de escolher arbitrariamente. Apresente os prós/contras de cada opção e o esforço adicional. Deixe o usuário decidir se vale a pena. Isso demonstra análise profunda e evita surpresas."

**Por quê?**: Evita refatorações, economiza tempo, garante código consistente com a base existente.

---

### 5️⃣ **Fazer Sprints das Tarefas Mais Simples**
- Agrupar 2-4 tarefas relacionadas em um sprint
- Estimar tempo total: **máximo 3-4 horas** por sprint
- Manter foco: **uma sprint = uma versão incremental**

**⚠️ Importante - Divisão de Tarefas em Subtasks**:
> Tarefas devem ser divididas em partes menores **somente se realmente necessário**, isto é:
> - ✅ Quando há **maior probabilidade de estourar o tempo máximo** (>4h)
> - ✅ Quando há **maior possibilidade da resposta ser muito longa** (implementação complexa)
> - ❌ **NÃO dividir** se a tarefa é razoavelmente simples e cabe no limite de tempo
> 
> Esta decisão deve ser feita pela **inteligência artificial responsável pela programação** do projeto, baseada na complexidade real da tarefa.

**Estrutura de Sprint**:
```
Sprint vX.Y.Z (Exemplo de Feature):
├── Task: Feature Implementation (3h estimado)
│   ├── Subtask 1: Fazer perguntas ao programador (15min)
│   ├── Subtask 2: Implementar função auxiliar principal (45min)
│   ├── Subtask 3: Implementar função de processamento (45min)
│   ├── Subtask 4: Integração com código existente (30min)
│   ├── Subtask 5: Testes unitários (60min)
│   └── Subtask 6: Documentação (30min)
└── Total: 3h45min ✅
```

---

### 6️⃣ **Implementar do Simples ao Complexo com Arquitetura Profissional**
- **Dentro de cada task**, começar pela parte mais fácil
- Construir incrementalmente: função auxiliar → função principal → integração
- Testar cada parte antes de avançar

**Ordem de Implementação**:
1. **Funções auxiliares** (ex: `extract_all_keys_from_obj()`)
2. **Funções principais** (ex: `build_substitution_map_by_value()`)
3. **Integração** (ex: atualizar `cli_dedupe()`)
4. **GUI/UX** (se aplicável)
5. **Otimizações** (último passo)

**Princípios de Arquitetura (Obrigatórios)**:

#### 🔄 **Reutilização de Código com Módulos**
- Criar módulos separados para cada responsabilidade
- Evitar duplicação (DRY - Don't Repeat Yourself)
- Funções genéricas reutilizáveis em múltiplos contextos

**Exemplo**:
```python
# ✅ BOM: Módulo reutilizável
# src/utils/file_utils.py
def read_file_safe(path: str) -> Optional[str]:
    """Função reutilizada em 10+ lugares"""
    try:
        with open(path, 'r', encoding='utf-8') as f:
            return f.read()
    except Exception as e:
        logger.error(f"Error reading {path}: {e}")
        return None

# ❌ RUIM: Duplicar código em cada módulo
# (repete try/except 20 vezes)
```

#### 💬 **Comentários de Código Obrigatórios**

> **CRÍTICO**: Todo código implementado **DEVE** ser comentado quando a linguagem de programação permitir comentários.

**Regra de Ouro**:
> **"Código sem comentário é código que ninguém mantém. Comente SEMPRE."**

**Quando comentar** (SEMPRE):
- ✅ **Funções e métodos**: O que fazem, parâmetros, retorno
- ✅ **Blocos lógicos importantes**: Por quê aquela abordagem
- ✅ **Variáveis não-óbvias**: O que representam
- ✅ **Algoritmos complexos**: Como funcionam
- ✅ **Decisões técnicas**: Por quê foi feito assim
- ✅ **TODOs e FIXMEs**: O que falta fazer
- ✅ **Casos especiais (edge cases)**: Por quê são tratados
- ✅ **Constantes e configurações**: Significado e uso

**O QUE comentar** (Prioridade):
1. **"Por quê" > "O quê"**: Explique a razão, não apenas o que o código faz
2. **Contexto**: Informação que não está óbvia no código
3. **Consequências**: O que acontece se algo mudar
4. **Restrições**: Limitações e cuidados

**Padrão de comentários por linguagem**:

**Python**:
```python
# Comentário de linha única
"""
Comentário de múltiplas linhas (docstring)
para documentar funções, classes e módulos
"""

def calculate_area(width: float, height: float) -> float:
    """
    Calcula a área de um retângulo.
    
    Args:
        width: Largura do retângulo em metros
        height: Altura do retângulo em metros
    
    Returns:
        Área em metros quadrados
    
    Exemplo:
        >>> calculate_area(5.0, 3.0)
        15.0
    """
    return width * height

# DECISÃO: Usamos multiplicação direta ao invés de loop
# porque é O(1) ao invés de O(n). Performance crítica aqui.
result = width * height

# TODO: Adicionar validação para valores negativos
# FIXME: Bug quando width=0, divisão por zero na linha 150
```

**JavaScript/TypeScript**:
```javascript
// Comentário de linha única
/* Comentário de múltiplas linhas */
/**
 * JSDoc para documentar funções
 * @param {number} width - Largura do retângulo
 * @param {number} height - Altura do retângulo
 * @returns {number} Área em metros quadrados
 */
function calculateArea(width, height) {
    // DECISÃO: Validação inline ao invés de função separada
    // Razão: Performance (evita overhead de chamada de função)
    if (width <= 0 || height <= 0) {
        throw new Error('Dimensões devem ser positivas');
    }
    
    return width * height; // Multiplicação direta: O(1)
}

// TODO: Implementar cálculo para círculos
// @ts-ignore - Ignorar erro temporário (remover após refatoração)
```

**Java**:
```java
// Comentário de linha única
/* Comentário de múltiplas linhas */
/**
 * JavaDoc para documentar classes e métodos
 * @param width Largura do retângulo
 * @param height Altura do retângulo
 * @return Área em metros quadrados
 */
public double calculateArea(double width, double height) {
    // DECISÃO: Usar double ao invés de float para maior precisão
    // Contexto: Cálculos de engenharia requerem precisão de 15 dígitos
    return width * height;
}

// TODO: Adicionar sobrecarga para int
// FIXME: NullPointerException quando dimensions é null (linha 45)
```

**C/C++**:
```cpp
// Comentário de linha única
/* Comentário de múltiplas linhas */
/**
 * Doxygen para documentar funções
 * @param width Largura do retângulo
 * @param height Altura do retângulo
 * @return Área em metros quadrados
 */
double calculateArea(double width, double height) {
    // DECISÃO: Usar double ao invés de float
    // Razão: Precisão crítica para cálculos científicos
    return width * height;
}

// NOTA: Esta função é thread-safe (não usa estado global)
// WARNING: Não chamar com valores negativos (comportamento indefinido)
```

**Exemplo Real Completo** (Python):
```python
def execute_virtual_graph(config: dict) -> None:
    """
    Executa o ambiente gráfico para exibir planos cartesianos.
    
    Este método inicializa o módulo virtualGraph.py e renderiza
    os gráficos configurados. Usa matplotlib para renderização.
    
    Args:
        config: Dicionário com configurações do gráfico
               {'title': str, 'x_range': tuple, 'y_range': tuple}
    
    Raises:
        ValueError: Se config não contém chaves obrigatórias
        RuntimeError: Se matplotlib não está disponível
    
    Exemplo:
        >>> config = {'title': 'Função Linear', 'x_range': (-10, 10)}
        >>> execute_virtual_graph(config)
        # Exibe janela com gráfico
    """
    # VALIDAÇÃO: Verificar chaves obrigatórias
    # Razão: Evitar erro genérico mais tarde (fail-fast principle)
    required_keys = ['title', 'x_range', 'y_range']
    for key in required_keys:
        if key not in config:
            raise ValueError(f"Config faltando chave obrigatória: {key}")
    
    # DECISÃO: Importar matplotlib aqui ao invés de no topo
    # Razão: Import pesado (~200ms), só carregar se realmente usar
    import matplotlib.pyplot as plt
    
    # Criar figura com tamanho otimizado para tela FullHD
    # NOTA: (12, 8) é o tamanho ideal testado com usuários
    fig, ax = plt.subplots(figsize=(12, 8))
    
    # Configurar título
    # FIXME: Título com caracteres especiais causa erro em PDF export
    ax.set_title(config['title'])
    
    # Configurar ranges dos eixos
    ax.set_xlim(config['x_range'])  # Eixo X
    ax.set_ylim(config['y_range'])  # Eixo Y
    
    # DECISÃO: Grid habilitado por padrão
    # Contexto: 95% dos usuários habilitam grid manualmente
    ax.grid(True, alpha=0.3)
    
    # Exibir gráfico
    # NOTA: Bloqueante - aguarda usuário fechar janela
    plt.show()
    
    # TODO: Adicionar opção de export automático para PNG
    # TODO: Implementar zoom interativo (usar mpl_toolkits)

# Executar ambiente gráfico
VirtualGraph.execute()  # Este comando executa funcionalidades do ambiente gráfico para exibir os planos cartesianos do módulo virtualGraph.py
```

**Diretrizes Adicionais**:

✅ **SEMPRE comente**:
- Qualquer código não-óbvio
- Decisões que não são evidentes
- Workarounds e hacks temporários
- Código que você mesmo não entenderia em 6 meses

❌ **NÃO comente**:
- Código auto-explicativo (ex: `x = 5  # atribui 5 a x`)
- Informação já no nome da variável/função
- Código gerado automaticamente que é óbvio

**Benefícios**:
1. ✅ Facilita manutenção futura (por você ou outros)
2. ✅ Reduz tempo de onboarding de novos desenvolvedores
3. ✅ Documenta decisões técnicas importantes
4. ✅ Previne reintrodução de bugs já corrigidos
5. ✅ Código se torna auto-documentado

**Mensagem para IAs**:
> "Ao gerar código, SEMPRE adicione comentários explicativos. Comente o 'por quê', não apenas o 'o quê'. Um código bem comentado vale 10x mais que código limpo sem comentários. Priorize comentários em decisões técnicas, algoritmos complexos e casos especiais."

#### 🌳 **Analogia da Árvore de Importações**

**Conceito**: A estrutura de importações de um programa pode ser visualizada como uma árvore, onde cada módulo importa outros módulos, formando uma hierarquia de dependências.

**Profundidade Ilimitada**: Esta árvore pode alcançar **qualquer nível ou altura** dependendo da complexidade do programa:
- **Programas Simples**: Árvore rasa (2-3 níveis)
  ```
  main.py
  └── utils.py
      └── helpers.py
  ```

- **Programas Médios**: Árvore moderada (4-6 níveis)
  ```
  app.py
  ├── controllers/
  │   └── user_controller.py
  │       └── services/
  │           └── user_service.py
  │               └── models/
  │                   └── user.py
  └── config.py
  ```

- **Programas Complexos**: Árvore profunda (7+ níveis)
  ```
  enterprise_app.py
  ├── api/
  │   ├── routes/
  │   │   └── v1/
  │   │       └── users.py
  │   │           └── handlers/
  │   │               └── authentication.py
  │   │                   └── providers/
  │   │                       └── oauth/
  │   │                           └── google.py
  │   │                               └── scopes.py
  ```

**Aplicação na Refatoração**:

1. **Identificar Profundidade Excessiva**:
   - ✅ Se árvore > 8 níveis → Considerar simplificação
   - ✅ Módulos muito profundos = difícil manutenção

2. **Detectar Dependências Circulares**:
   ```python
   # ❌ RUIM: Dependência circular
   # module_a.py
   from module_b import B
   
   # module_b.py
   from module_a import A  # Circular!
   ```

3. **Reorganizar por Coesão**:
   ```python
   # ✅ BOM: Agrupar imports relacionados
   # antes (disperso):
   from utils.string import normalize
   from helpers.text import clean
   from tools.format import sanitize
   
   # depois (coeso):
   from text_processing import normalize, clean, sanitize
   ```

4. **Reduzir Acoplamento**:
   - ✅ Imports diretos apenas do necessário
   - ✅ Evitar `from module import *` (aumenta acoplamento)
   - ✅ Usar interfaces/abstrações para desacoplar

5. **Visualizar para Entender**:
   - Use ferramentas como `pydeps`, `import-graph` (Python)
   - Identifique "hubs" (módulos muito importados)
   - Refatore módulos centrais para reduzir impacto

**Por quê importante**:
- ✅ **Compreensão**: Árvore clara = código mais fácil de entender
- ✅ **Manutenção**: Dependências organizadas = mudanças localizadas
- ✅ **Performance**: Menos imports desnecessários = startup mais rápido
- ✅ **Testes**: Módulos independentes = testes isolados
- ✅ **Refatoração**: Visualizar árvore ajuda a identificar oportunidades de melhoria

#### 📦 **Hierarquias e Encapsulamento**
- Usar classes quando há estado compartilhado
- Encapsular atributos privados (`_attribute`)
- Expor apenas interface pública necessária

**Exemplo**:
```python
# ✅ BOM: Encapsulamento adequado
class ReferenceUpdater:
    def __init__(self, project_dir: str):
        self._project_dir = project_dir
        self._substitutions = {}
    
    def update_references(self) -> Dict[str, int]:
        """Interface pública clara"""
        self._scan_files()  # Método privado
        self._build_map()   # Método privado
        return self._apply_changes()

# ❌ RUIM: Tudo exposto, sem estrutura
def do_everything(dir, old, new, backup, ext):
    # 200 linhas sem organização
```

#### 🎯 **Alta Coesão e Baixo Acoplamento**
- **Alta Coesão**: Cada módulo/classe tem uma única responsabilidade clara
- **Baixo Acoplamento**: Módulos independentes, comunicação por interfaces

**Exemplo**:
```python
# ✅ ALTA COESÃO: Cada classe faz UMA coisa
class KeyExtractor:
    """Apenas extrai chaves de estruturas"""
    def extract(self, data) -> Dict[str, str]: ...

class SubstitutionMapBuilder:
    """Apenas constrói mapa de substituições"""
    def build(self, old, new) -> Dict[str, str]: ...

class FileUpdater:
    """Apenas atualiza arquivos"""
    def update(self, files, map) -> int: ...

# ✅ BAIXO ACOPLAMENTO: Comunicação por interfaces
class ReferenceUpdater:
    def __init__(self, extractor: KeyExtractor, builder: SubstitutionMapBuilder):
        self._extractor = extractor  # Injeção de dependência
        self._builder = builder

# ❌ RUIM: Baixa coesão, alto acoplamento
class EverythingManager:
    def do_all(self):
        # Faz extração + construção + atualização + logging + GUI
        # Importa 20 módulos diferentes
        # Impossível testar isoladamente
```

#### 🏗️ **Padrões GoF (Gang of Four)**
Aplicar padrões de design quando apropriado:

1. **Strategy Pattern** (escolha de algoritmo em runtime):
```python
class CaseConverter:
    def __init__(self, strategy: CaseStrategy):
        self._strategy = strategy
    
    def convert(self, text: str) -> str:
        return self._strategy.apply(text)

class CamelCaseStrategy(CaseStrategy):
    def apply(self, text: str) -> str: ...

class SnakeCaseStrategy(CaseStrategy):
    def apply(self, text: str) -> str: ...
```

2. **Factory Pattern** (criação de objetos complexos):
```python
class ProcessorFactory:
    @staticmethod
    def create(type: str) -> Processor:
        if type == "type_a":
            return ProcessorA()
        elif type == "type_b":
            return ProcessorB()
```

3. **Observer Pattern** (notificação de eventos):
```python
class ProcessingModal(QDialog):
    cancel_requested = Signal()  # Observer pattern
    
    def _on_cancel_clicked(self):
        self.cancel_requested.emit()  # Notifica observadores
```

4. **Command Pattern** (undo/redo):
```python
class ReplaceCommand:
    def __init__(self, file: str, old: str, new: str):
        self._file = file
        self._old = old
        self._new = new
    
    def execute(self): ...
    def undo(self): ...
```

#### 🎨 **Padrões GRASP (General Responsibility Assignment Software Patterns)**

1. **Information Expert**: Atribua responsabilidade a quem tem a informação
```python
# ✅ BOM: Classe tem a informação, então tem o método
class DataStore:
    def __init__(self, data: dict):
        self._data = data
    
    def get_value(self, key_path: str) -> Optional[str]:
        """Classe conhece sua estrutura"""
        return self._navigate_path(key_path)

# ❌ RUIM: Classe externa manipula estrutura interna
def get_value_from_data(data_store, key_path):
    # Acesso direto à estrutura interna do dict
```

2. **Creator**: Classe A cria B se A contém/agrega B
```python
# ✅ BOM: RewriterDock cria seus próprios widgets
class ComponentB(BaseDock):
    def __init__(self):
        self._create_widgets()  # Creator pattern
        self._setup_layout()
    
    def _create_widgets(self):
        self.ed_input = QLineEdit()  # Cria seus filhos
        self.btn_process = QPushButton()
```

3. **Controller**: Delegar operações do sistema a controlador
```python
# ✅ BOM: Controlador coordena operações
class RewriterController:
    def process_file(self, path: str):
        data = self._reader.read(path)
        processed = self._processor.process(data)
        self._writer.write(path, processed)

# ❌ RUIM: GUI faz tudo diretamente
class RewriterDock:
    def on_button_click(self):
        # 50 linhas de lógica de negócio na GUI
```

4. **Low Coupling**: Minimizar dependências
```python
# ✅ BOM: Interface genérica
def update_references(updater: ReferenceUpdater):
    """Aceita qualquer updater que implemente a interface"""
    updater.update()

# ❌ RUIM: Dependência concreta
def update_references(file_path: str, backup: bool, ext: list):
    """Muitos parâmetros, alto acoplamento"""
```

5. **High Cohesion**: Uma classe, uma responsabilidade
```python
# ✅ BOM: Alta coesão
class FileReader:
    """Apenas lê arquivos"""
    def read(self, path: str) -> str: ...

class DataValidator:
    """Apenas valida dados"""
    def validate(self, data: dict) -> bool: ...

# ❌ RUIM: Baixa coesão
class FileManager:
    def read(self): ...
    def write(self): ...
    def validate(self): ...
    def send_email(self): ...  # ?!
```

**Anti-padrão** ❌:
```python
# NÃO fazer tudo de uma vez:
def complex_function_with_everything():
    # 500 linhas de código
    # Múltiplas responsabilidades
    # Difícil de testar
    # Alto acoplamento
    # Sem reutilização
```

**Padrão Correto** ✅:
```python
# Módulo: src/processor/extractor.py
class DataExtractor:
    """Alta coesão: só extrai dados"""
    def extract_from_source(self, data) -> Dict[str, str]:
        return self._recurse(data, prefix='item')

# Módulo: src/processor/transformer.py
class DataTransformer:
    """Alta coesão: só transforma dados"""
    def transform(self, old, new) -> Dict[str, str]:
        return self._match_values(old, new)

# Módulo: src/processor/updater.py
class DataUpdater:
    """Baixo acoplamento: usa interfaces"""
    def __init__(self, extractor: DataExtractor, transformer: DataTransformer):
        self._extractor = extractor  # Injeção de dependência
        self._transformer = transformer
    
    def update_project(self, dir: str) -> Dict[str, int]:
        """Coordena mas não implementa tudo"""
        old = self._extractor.extract(self._read_old())
        new = self._extractor.extract(self._read_new())
        mapping = self._transformer.transform(old, new)
        return self._apply_to_files(dir, mapping)
```

---

### 6️⃣.6️⃣ **Ícones do Projeto** [OBRIGATÓRIO]

> **CRÍTICO PARA IAs**: Todo projeto deve incluir ícones adequados para garantir profissionalismo e identidade visual.

**Quando Aplicar**: Durante a implementação (Etapa 6), após definir a estrutura básica do projeto.

#### 📋 Requisito Obrigatório

A inteligência artificial **DEVE** produzir ou fazer download de um ícone para o projeto, seja:
- 🌐 Site/Aplicação Web
- 💻 Programa Desktop
- 📱 Aplicativo Mobile
- 🔧 Ferramenta/Utilitário

#### 🎨 Formatos de Ícone por Tecnologia

**Aplicações Web**:
- ✅ **favicon.ico** (16x16, 32x32, 48x48 px) - Compatibilidade universal
- ✅ **icon.svg** - Vetorial, escalável, moderno
- ✅ **icon-192.png** e **icon-512.png** - PWA/Android
- ✅ **apple-touch-icon.png** (180x180 px) - iOS

**Aplicações Desktop**:
- ✅ **icon.png** (256x256, 512x512 px) - Linux
- ✅ **icon.ico** (múltiplos tamanhos) - Windows
- ✅ **icon.icns** - macOS

**Aplicações Mobile**:
- ✅ **icon.png** (1024x1024 px) - iOS App Store
- ✅ **ic_launcher.png** (múltiplas densidades) - Android
- ✅ **adaptive-icon.xml** - Android adaptativo

#### 📁 Estrutura de Pastas (OBRIGATÓRIO)

Os ícones **DEVEM** ser organizados em uma pasta dedicada:

```
projeto/
├── assets/              # ✅ PREFERIDO (padrão para todos)
│   ├── icons/
│   │   ├── favicon.ico
│   │   ├── icon.svg
│   │   ├── icon-192.png
│   │   ├── icon-512.png
│   │   └── apple-touch-icon.png
│   └── ...
│
# OU alternativas conforme tecnologia:
├── public/              # ✅ React, Vue, Next.js
│   ├── favicon.ico
│   └── icons/
├── static/              # ✅ Flask, Django, Svelte
│   └── icons/
├── src/assets/          # ✅ Angular, Ionic
│   └── icons/
├── resources/           # ✅ Electron, Tauri
│   └── icons/
└── res/                 # ✅ Android nativo
    └── drawable/
```

**Regra de Ouro**: Sempre usar uma pasta específica para ícones, nunca arquivos soltos na raiz do projeto.

#### 🔧 Como Obter/Criar Ícones

A IA deve seguir esta ordem de prioridade:

1. **Perguntar ao Programador** (SEMPRE primeiro):
   ```
   ❓ Você já tem um ícone para o projeto?
   
   Opções:
   A) ✅ Sim, tenho (forneça o caminho/arquivo)
   B) 🎨 Não, crie um ícone simples para mim
   C) 🔍 Não, baixe um ícone gratuito adequado
   D) ⏭️ Pular por enquanto (não recomendado)
   ```

2. **Se A (Usuário fornece)**:
   - Validar formato e tamanho
   - Converter para formatos necessários (usar ferramentas como `convert`, `sharp`, `imagemagick`)
   - Organizar na pasta correta

3. **Se B (IA cria ícone simples)**:
   - Criar ícone SVG vetorial com iniciais do projeto
   - Exportar para formatos necessários (PNG, ICO)
   - Usar cores da identidade do projeto (se definidas)

4. **Se C (IA baixa ícone)**:
   - Usar fontes gratuitas e sem copyright:
     - ✅ [Heroicons](https://heroicons.com/) (MIT License)
     - ✅ [Lucide Icons](https://lucide.dev/) (ISC License)
     - ✅ [Tabler Icons](https://tabler-icons.io/) (MIT License)
     - ✅ [Iconoir](https://iconoir.com/) (MIT License)
   - Verificar licença antes de usar
   - Documentar fonte no README

5. **Se D (Pular)**:
   - ⚠️ Avisar que projeto ficará sem identidade visual
   - Adicionar task no TASKS.md para futuro: `[ ] Criar ícone do projeto`

#### 🎨 Exemplo de Ícone SVG Simples (Gerado pela IA)

```svg
<!-- assets/icons/icon.svg -->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100">
  <rect width="100" height="100" rx="20" fill="#4F46E5"/>
  <text x="50" y="65" font-family="Arial, sans-serif" font-size="48" 
        font-weight="bold" fill="white" text-anchor="middle">MP</text>
</svg>
```

#### 🔨 Ferramentas para Conversão de Ícones

**Python** (recomendado para automação):
```bash
# Instalar Pillow
pip install Pillow

# Converter SVG para PNG (via cairosvg)
pip install cairosvg
python -c "import cairosvg; cairosvg.svg2png(url='icon.svg', write_to='icon.png', output_width=512)"

# Criar ICO com múltiplos tamanhos
from PIL import Image
img = Image.open('icon.png')
img.save('favicon.ico', format='ICO', sizes=[(16,16), (32,32), (48,48)])
```

**Node.js** (projetos web):
```bash
# Instalar sharp
npm install sharp

# Script de conversão
node -e "
const sharp = require('sharp');
sharp('icon.svg').resize(192, 192).toFile('icon-192.png');
sharp('icon.svg').resize(512, 512).toFile('icon-512.png');
"
```

**ImageMagick** (universal):
```bash
# Converter SVG para PNG
convert icon.svg -resize 192x192 icon-192.png

# Criar favicon.ico
convert icon.png -define icon:auto-resize=16,32,48 favicon.ico
```

#### 🗂️ Integração com o Projeto

**HTML (Web)**:
```html
<!-- index.html -->
<head>
  <!-- Favicon básico -->
  <link rel="icon" type="image/x-icon" href="/assets/icons/favicon.ico">
  
  <!-- SVG moderno (preferido) -->
  <link rel="icon" type="image/svg+xml" href="/assets/icons/icon.svg">
  
  <!-- PNG para diferentes tamanhos -->
  <link rel="icon" type="image/png" sizes="32x32" href="/assets/icons/icon-32.png">
  <link rel="icon" type="image/png" sizes="192x192" href="/assets/icons/icon-192.png">
  
  <!-- Apple Touch Icon -->
  <link rel="apple-touch-icon" href="/assets/icons/apple-touch-icon.png">
  
  <!-- Android Chrome -->
  <link rel="manifest" href="/manifest.json">
</head>
```

**manifest.json (PWA)**:
```json
{
  "name": "Meu Projeto",
  "short_name": "MP",
  "icons": [
    {
      "src": "/assets/icons/icon-192.png",
      "sizes": "192x192",
      "type": "image/png"
    },
    {
      "src": "/assets/icons/icon-512.png",
      "sizes": "512x512",
      "type": "image/png"
    }
  ]
}
```

**Python (Desktop - PyQt/Tkinter)**:
```python
# PyQt6
from PyQt6.QtGui import QIcon
from PyQt6.QtWidgets import QApplication

app = QApplication([])
app.setWindowIcon(QIcon('assets/icons/icon.png'))

# Tkinter
import tkinter as tk
root = tk.Tk()
root.iconbitmap('assets/icons/icon.ico')  # Windows
# ou
root.iconphoto(True, tk.PhotoImage(file='assets/icons/icon.png'))  # Linux/Mac
```

**Electron (Desktop)**:
```javascript
// main.js
const { app, BrowserWindow } = require('electron');
const path = require('path');

const win = new BrowserWindow({
  icon: path.join(__dirname, 'resources/icons/icon.png')
});
```

**React Native (Mobile)**:
```
// android/app/src/main/res/
mipmap-hdpi/ic_launcher.png      (72x72)
mipmap-mdpi/ic_launcher.png      (48x48)
mipmap-xhdpi/ic_launcher.png     (96x96)
mipmap-xxhdpi/ic_launcher.png    (144x144)
mipmap-xxxhdpi/ic_launcher.png   (192x192)

// ios/ProjectName/Images.xcassets/AppIcon.appiconset/
// Configurado via Xcode ou Contents.json
```

#### ⏰ Melhor Momento para Adicionar Ícones

**Recomendação**: **Durante Etapa 6 (Implementação)**, preferencialmente:

1. **Início do Projeto** (✅ IDEAL):
   - Ao criar estrutura inicial de pastas
   - Antes do primeiro commit
   - Facilita identidade visual desde o início

2. **MVP/Protótipo** (✅ BOM):
   - Após funcionalidades básicas funcionarem
   - Antes de mostrar para usuários/clientes
   - Garante profissionalismo mínimo

3. **Antes de Produção** (⚠️ ACEITÁVEL):
   - Durante preparação para deploy
   - Antes de publicar (App Store, Play Store, web)
   - Mínimo necessário, mas atrasado

4. **❌ NUNCA**: Deixar para "depois" sem data definida

#### 📋 Checklist de Ícones (Validação)

```markdown
## Checklist de Ícones - Projeto [Nome]

### Ícones Criados
- [ ] Ícone principal criado/obtido (fonte: [especificar])
- [ ] Licença verificada (se baixado de fonte externa)
- [ ] Formato vetorial disponível (SVG) ou fonte PNG de alta qualidade

### Formatos Necessários
- [ ] **favicon.ico** (16x16, 32x32, 48x48 px)
- [ ] **icon.svg** (vetorial)
- [ ] **icon-192.png** (192x192 px) - PWA
- [ ] **icon-512.png** (512x512 px) - PWA
- [ ] **apple-touch-icon.png** (180x180 px) - iOS
- [ ] Outros formatos específicos da tecnologia

### Organização
- [ ] Pasta `assets/icons/` criada
- [ ] Todos os ícones organizados na pasta correta
- [ ] Nenhum ícone solto na raiz do projeto

### Integração
- [ ] Ícone referenciado no HTML/código principal
- [ ] manifest.json atualizado (se PWA)
- [ ] Testado em navegador/aplicativo (ícone aparece)
- [ ] Documentado no README (se ícone de terceiros)

### Qualidade
- [ ] Ícone tem boa resolução (não pixelado)
- [ ] Cores adequadas ao projeto
- [ ] Visível em fundos claros E escuros (se aplicável)
- [ ] Reconhecível em tamanhos pequenos (16x16)
```

#### 🎯 Rationale: Por Quê Ícones São Obrigatórios

1. **Profissionalismo**: Projetos sem ícone parecem incompletos/amadores
2. **Identidade Visual**: Usuários reconhecem o app pelo ícone (branding)
3. **Experiência do Usuário**: Ícone ajuda a localizar o app entre várias abas/janelas
4. **Requisitos de Plataforma**: App stores (iOS/Android) EXIGEM ícones
5. **PWA**: Navegadores solicitam ícones para instalação
6. **Organização**: Facilita encontrar e gerenciar assets visuais
7. **Rastreabilidade**: Documentar fonte garante conformidade de licença

#### 🚨 Erros Comuns a Evitar

❌ **Não Fazer**:
- Deixar ícone na raiz do projeto (ex: `favicon.ico` solto)
- Usar ícone de baixa resolução (pixelado quando ampliado)
- Esquecer de referenciar no HTML/código
- Usar ícone com copyright sem permissão
- Criar apenas um tamanho (navegadores precisam de múltiplos)

✅ **Fazer**:
- Organizar em pasta dedicada (`assets/icons/`)
- Gerar múltiplos tamanhos (16, 32, 192, 512 px)
- Validar que ícone aparece corretamente
- Documentar fonte se ícone de terceiros
- Usar formato vetorial (SVG) quando possível

#### 📚 Recursos Úteis

**Geradores de Ícone Online** (gratuitos):
- [Favicon.io](https://favicon.io/) - Gera favicon de texto/imagem/emoji
- [RealFaviconGenerator](https://realfavicongenerator.net/) - Gera todos os formatos
- [Favicon Generator](https://www.favicon-generator.org/) - Simples e rápido

**Bancos de Ícones Gratuitos**:
- [Heroicons](https://heroicons.com/) - MIT License
- [Lucide Icons](https://lucide.dev/) - ISC License
- [Tabler Icons](https://tabler-icons.io/) - MIT License
- [Iconoir](https://iconoir.com/) - MIT License
- [Bootstrap Icons](https://icons.getbootstrap.com/) - MIT License

**Ferramentas de Conversão**:
- [ImageMagick](https://imagemagick.org/) - CLI universal
- [Pillow (Python)](https://pillow.readthedocs.io/) - Biblioteca de imagens
- [Sharp (Node.js)](https://sharp.pixelplumbing.com/) - Alto desempenho

#### 📝 Exemplo de Documentação no README

```markdown
## 🎨 Ícone do Projeto

**Fonte**: Criado pela IA usando iniciais do projeto  
**Licença**: Livre para uso (gerado para este projeto)  
**Localização**: `assets/icons/`

### Formatos Disponíveis
- `icon.svg` - Vetorial (preferido)
- `favicon.ico` - Navegadores (16, 32, 48 px)
- `icon-192.png` - PWA/Android
- `icon-512.png` - PWA/Android
- `apple-touch-icon.png` - iOS

### Cores
- Principal: `#4F46E5` (Azul Índigo)
- Texto: `#FFFFFF` (Branco)
```

#### ⏱️ Tempo Estimado

- **Criar ícone simples (IA)**: 5-10 minutos
- **Baixar e adaptar ícone**: 10-15 minutos
- **Converter para formatos necessários**: 5-10 minutos
- **Integrar no projeto**: 5-10 minutos
- **TOTAL**: 15-30 minutos

**Investimento pequeno, impacto grande na percepção de qualidade do projeto.**

---

### 6️⃣.7️⃣ **Scripts de Execução para Facilitar o Uso** [RECOMENDADO]

> **RECOMENDAÇÃO PARA IAs**: Quando se trata de um aplicativo ou programa escrito com uma linguagem de programação que é executável, é recomendado criar scripts em batch para Windows, Linux e Mac acessíveis na pasta principal ou diretório raiz, a fim de facilitar a execução do aplicativo.

**Quando Aplicar**: Durante a implementação (Etapa 6), especialmente após configurar a estrutura básica do projeto executável.

#### 📋 Contexto e Propósito

Scripts de execução na raiz do projeto facilitam significativamente o uso da aplicação, especialmente:
- ✅ **Desenvolvimento**: Acelera ciclo de desenvolvimento (executar sem configurar ambiente manualmente)
- ✅ **Onboarding**: Novos desenvolvedores conseguem rodar projeto imediatamente
- ✅ **Testes**: Facilita execução de testes e validação
- ✅ **Produção**: Em alguns casos, pode simplificar deployment (se não houver alternativas melhores como Docker, systemd, etc.)

#### 🎯 Quando Criar Scripts de Execução

**✅ CRIAR scripts SE:**
- ✅ Aplicação é executável (não é biblioteca)
- ✅ Requer configuração de ambiente (variáveis, paths, dependências)
- ✅ Tem múltiplos comandos de inicialização
- ✅ Precisa de setup antes de executar (migrations, build, etc.)
- ✅ Time/usuários precisam executar frequentemente

**❌ NÃO criar scripts SE:**
- ❌ Aplicação já tem CLI nativo bem documentado
- ❌ Usa ferramentas padrão da linguagem (npm start, cargo run, etc.)
- ❌ Deployment usa orquestração (Docker, Kubernetes) - scripts ficam no Dockerfile
- ❌ Projeto é biblioteca/framework (não executável)

#### 📝 Estrutura de Pastas Recomendada

```
projeto/
├── run.bat                 # ✅ Windows (execução principal)
├── run.sh                  # ✅ Linux/Mac (execução principal)
├── dev.bat                 # 🔄 Desenvolvimento Windows (opcional)
├── dev.sh                  # 🔄 Desenvolvimento Linux/Mac (opcional)
├── test.bat                # 🧪 Testes Windows (opcional)
├── test.sh                 # 🧪 Testes Linux/Mac (opcional)
├── build.bat               # 🏗️ Build Windows (opcional)
├── build.sh                # 🏗️ Build Linux/Mac (opcional)
└── README.md               # Documentação de uso dos scripts
```

**Regra de Ouro**: Scripts na raiz do projeto = acesso fácil. Scripts complexos podem ficar em `scripts/` com wrappers simples na raiz.

#### 💻 Exemplos de Scripts por Linguagem

##### **Python**

**run.sh (Linux/Mac)**:
```bash
#!/bin/bash
# Script de execução para Linux/Mac

# Cores para output
GREEN='\033[0;32m'
RED='\033[0;31m'
NC='\033[0m' # No Color

echo -e "${GREEN}🚀 Iniciando aplicação Python...${NC}"

# Verificar se ambiente virtual existe
if [ ! -d "venv" ]; then
    echo -e "${RED}❌ Ambiente virtual não encontrado. Criando...${NC}"
    python3 -m venv venv
fi

# Ativar ambiente virtual
source venv/bin/activate

# Instalar/atualizar dependências
if [ -f "requirements.txt" ]; then
    echo -e "${GREEN}📦 Instalando dependências...${NC}"
    pip install -q -r requirements.txt
fi

# Executar aplicação
echo -e "${GREEN}✅ Executando aplicação...${NC}"
python src/main.py "$@"
```

**run.bat (Windows)**:
```batch
@echo off
REM Script de execução para Windows

echo 🚀 Iniciando aplicação Python...

REM Verificar se ambiente virtual existe
if not exist "venv\" (
    echo ❌ Ambiente virtual não encontrado. Criando...
    python -m venv venv
)

REM Ativar ambiente virtual
call venv\Scripts\activate.bat

REM Instalar/atualizar dependências
if exist "requirements.txt" (
    echo 📦 Instalando dependências...
    pip install -q -r requirements.txt
)

REM Executar aplicação
echo ✅ Executando aplicação...
python src\main.py %*
```

##### **Node.js**

**run.sh (Linux/Mac)**:
```bash
#!/bin/bash
# Script de execução para Linux/Mac

GREEN='\033[0;32m'
NC='\033[0m'

echo -e "${GREEN}🚀 Iniciando aplicação Node.js...${NC}"

# Verificar se node_modules existe
if [ ! -d "node_modules" ]; then
    echo -e "${GREEN}📦 Instalando dependências...${NC}"
    npm install
fi

# Executar aplicação
echo -e "${GREEN}✅ Executando aplicação...${NC}"
npm start "$@"
```

**run.bat (Windows)**:
```batch
@echo off
REM Script de execução para Windows

echo 🚀 Iniciando aplicação Node.js...

REM Verificar se node_modules existe
if not exist "node_modules\" (
    echo 📦 Instalando dependências...
    call npm install
)

REM Executar aplicação
echo ✅ Executando aplicação...
npm start %*
```

##### **Java**

**run.sh (Linux/Mac)**:
```bash
#!/bin/bash
# Script de execução para Linux/Mac

GREEN='\033[0;32m'
NC='\033[0m'

echo -e "${GREEN}🚀 Iniciando aplicação Java...${NC}"

# Compilar se necessário
if [ ! -d "target" ]; then
    echo -e "${GREEN}🏗️ Compilando projeto...${NC}"
    mvn clean package -DskipTests
fi

# Executar JAR
echo -e "${GREEN}✅ Executando aplicação...${NC}"
java -jar target/myapp.jar "$@"
```

**run.bat (Windows)**:
```batch
@echo off
REM Script de execução para Windows

echo 🚀 Iniciando aplicação Java...

REM Compilar se necessário
if not exist "target\" (
    echo 🏗️ Compilando projeto...
    call mvn clean package -DskipTests
)

REM Executar JAR
echo ✅ Executando aplicação...
java -jar target\myapp.jar %*
```

##### **Go**

**run.sh (Linux/Mac)**:
```bash
#!/bin/bash
# Script de execução para Linux/Mac

GREEN='\033[0;32m'
NC='\033[0m'

echo -e "${GREEN}🚀 Iniciando aplicação Go...${NC}"

# Baixar dependências se necessário
if [ ! -f "go.sum" ]; then
    echo -e "${GREEN}📦 Baixando dependências...${NC}"
    go mod download
fi

# Executar aplicação
echo -e "${GREEN}✅ Executando aplicação...${NC}"
go run cmd/main.go "$@"
```

**run.bat (Windows)**:
```batch
@echo off
REM Script de execução para Windows

echo 🚀 Iniciando aplicação Go...

REM Baixar dependências se necessário
if not exist "go.sum" (
    echo 📦 Baixando dependências...
    go mod download
)

REM Executar aplicação
echo ✅ Executando aplicação...
go run cmd\main.go %*
```

##### **Rust**

**run.sh (Linux/Mac)**:
```bash
#!/bin/bash
# Script de execução para Linux/Mac

GREEN='\033[0;32m'
NC='\033[0m'

echo -e "${GREEN}🚀 Iniciando aplicação Rust...${NC}"

# Compilar e executar
echo -e "${GREEN}✅ Executando aplicação (cargo run)...${NC}"
cargo run --release "$@"
```

**run.bat (Windows)**:
```batch
@echo off
REM Script de execução para Windows

echo 🚀 Iniciando aplicação Rust...

REM Compilar e executar
echo ✅ Executando aplicação (cargo run)...
cargo run --release %*
```

#### 🔧 Scripts Adicionais Úteis

##### **Script de Desenvolvimento** (modo watch/reload)

**dev.sh**:
```bash
#!/bin/bash
# Modo desenvolvimento com auto-reload

echo "🔄 Iniciando em modo desenvolvimento..."

# Python
# pip install watchdog
# watchmedo auto-restart --directory=./src --pattern=*.py python src/main.py

# Node.js
# npm run dev  # nodemon ou similar

# Go
# go install github.com/cosmtrek/air@latest
# air

# Rust
# cargo install cargo-watch
# cargo watch -x run
```

##### **Script de Testes**

**test.sh**:
```bash
#!/bin/bash
# Executar testes

echo "🧪 Executando testes..."

# Python
# pytest tests/ -v

# Node.js
# npm test

# Java
# mvn test

# Go
# go test ./...

# Rust
# cargo test
```

#### 📋 Checklist de Scripts de Execução

```markdown
## Checklist de Scripts - Projeto [Nome]

### Scripts Criados
- [ ] **run.sh** (Linux/Mac) - Script principal de execução
- [ ] **run.bat** (Windows) - Script principal de execução
- [ ] Permissões de execução configuradas (`chmod +x *.sh`)
- [ ] Scripts testados em cada plataforma

### Scripts Opcionais (conforme necessidade)
- [ ] **dev.sh/dev.bat** - Modo desenvolvimento com auto-reload
- [ ] **test.sh/test.bat** - Executar testes automatizados
- [ ] **build.sh/build.bat** - Compilar/build do projeto
- [ ] **install.sh/install.bat** - Instalar dependências
- [ ] **clean.sh/clean.bat** - Limpar artifacts de build

### Documentação
- [ ] README.md atualizado com instruções de uso dos scripts
- [ ] Exemplos de uso documentados
- [ ] Requisitos de sistema documentados (Python 3.9+, Node 18+, etc.)
- [ ] Troubleshooting básico incluído

### Funcionalidades dos Scripts
- [ ] Verificam se dependências estão instaladas
- [ ] Criam ambiente virtual/diretórios se necessário
- [ ] Mensagens de output claras e informativas
- [ ] Suportam passagem de argumentos (`./run.sh --help`)
- [ ] Tratam erros graciosamente
- [ ] Incluem cores no output (opcional, melhora UX)
```

#### 📝 Exemplo de Documentação no README

```markdown
## 🚀 Como Executar

### Requisitos
- Python 3.9+ (ou Node.js 18+, Java 17+, etc.)
- Git

### Execução Rápida

**Linux/Mac**:
```bash
./run.sh
```

**Windows**:
```batch
run.bat
```

### Scripts Disponíveis

| Script | Descrição | Plataforma |
|--------|-----------|------------|
| `run.sh` / `run.bat` | Executa a aplicação principal | Linux/Mac / Windows |
| `dev.sh` / `dev.bat` | Modo desenvolvimento (auto-reload) | Linux/Mac / Windows |
| `test.sh` / `test.bat` | Executa testes automatizados | Linux/Mac / Windows |
| `build.sh` / `build.bat` | Compila/builda o projeto | Linux/Mac / Windows |

### Argumentos

Passar argumentos para aplicação:
```bash
./run.sh --port 8080 --debug
```

### Troubleshooting

**Erro: Permission denied (Linux/Mac)**
```bash
chmod +x run.sh dev.sh test.sh build.sh
```

**Erro: Dependências não encontradas**
- Scripts instalam dependências automaticamente na primeira execução
- Se falhar, execute manualmente: `pip install -r requirements.txt` (Python) ou `npm install` (Node.js)
```

#### ⏱️ Tempo Estimado

- **Criar scripts básicos (run.sh/run.bat)**: 10-15 minutos
- **Adicionar scripts opcionais (dev, test, build)**: 5-10 minutos cada
- **Documentar no README**: 10-15 minutos
- **Testar em múltiplas plataformas**: 10-20 minutos
- **TOTAL**: 30-60 minutos

**Investimento: ~30-60 minutos. Benefício: Economiza horas de setup para cada desenvolvedor e usuário.**

#### 🎯 Rationale: Por Quê Scripts de Execução São Importantes

1. **Developer Experience (DX)**: Novo desenvolvedor clona repo, executa `./run.sh` e aplicação funciona
2. **Redução de Fricção**: Sem necessidade de ler documentação complexa para rodar projeto
3. **Consistência**: Todos executam da mesma forma, reduz "funciona na minha máquina"
4. **Automação**: Scripts podem configurar ambiente automaticamente (criar venv, instalar deps)
5. **Documentação Viva**: Scripts servem como documentação executável do processo de inicialização
6. **Onboarding**: Acelera entrada de novos membros no time
7. **CI/CD**: Scripts podem ser reutilizados em pipelines
8. **Cross-Platform**: Suporte explícito para Windows, Linux e Mac

#### ⚠️ Quando NÃO Usar Scripts na Raiz

**Use alternativas melhores quando disponíveis:**
- 🐳 **Docker/Docker Compose**: Para apps com múltiplas dependências (bancos, filas, etc.)
- 📦 **Package Managers Nativos**: `npm start`, `cargo run`, `go run` já são suficientes
- 🎯 **Task Runners**: Makefile, Just, Task para projetos complexos
- ☸️ **Orquestração**: Kubernetes, systemd para produção enterprise

**Combinação Recomendada**:
```
projeto/
├── docker-compose.yml      # 🐳 Para ambiente completo
├── Makefile                # 🎯 Para comandos complexos
├── run.sh                  # ✅ Wrapper simples que chama Make/Docker
└── README.md               # 📚 Documenta quando usar cada um
```

**Exemplo de wrapper**:
```bash
#!/bin/bash
# run.sh - Wrapper simples

if command -v docker &> /dev/null; then
    echo "🐳 Docker detectado, usando docker-compose..."
    docker-compose up
else
    echo "⚠️ Docker não encontrado, executando localmente..."
    make run
fi
```

---

### 7️⃣ **Verificar Implementação CLI + Revisão de Código**
- **CRÍTICO**: Verificar se a nova funcionalidade está disponível via **CLI (Command Line Interface)**
- **IMPORTANTE**: Durante a verificação, aplicar os **9 Critérios de Qualidade** ao código CLI
- Não basta implementar GUI, funcionalidades importantes devem ter **interface CLI** para automação
- Verificar subcomandos, argumentos, help text, integração e qualidade do código

**Checklist de Implementação CLI**:

1. **Import Correto no Arquivo Principal**:
   ```python
   # ✅ Verificar se módulo foi importado
   from .modules import (
       ModuleA, ModuleB, ModuleC,
       ModuleD, ModuleE, ModuleF,
       ModuleG, ModuleH, NewModule  # ← NOVO módulo deve estar aqui
   )
   ```

2. **Export no __init__.py do Módulo**:
   ```python
   # src/modules/__init__.py
   from .new_module import NewModule
   
   __all__ = [
       'ModuleA', 'ModuleB', 'ModuleC',
       'ModuleD', 'ModuleE', 'ModuleF',
       'ModuleG', 'ModuleH', 'NewModule'  # ← NOVO módulo exportado
   ]
   ```

3. **Interface/Menu Item Criado e Conectado**:
   ```python
   # Em _build_interface() ou similar
   menu = self.create_menu("Tools")
   
   # Criar ação
   self.action_new_feature = Action("New Feature", self)
   
   # Adicionar ao menu/interface
   menu.add_action(self.action_new_feature)
   
   # Conectar signal
   self.action_new_feature.triggered.connect(lambda: self.new_module.execute())
   ```

4. **Dock Inicializado no __init__() ou método de setup**:
   ```python
   # Em __init__() da MainWindow
   def __init__(self):
       super().__init__()
       # ... outros docks ...
       self._open_new_component()  # ← Inicializar dock
   
   def _open_new_component(self):
       self.dock_new_component = NewComponent(self)
       self.dock_new_component.open_in_other_component_requested.connect(self._load_data_from_source)
       self.addDockWidget(Qt.RightDockWidgetArea, self.dock_new_component)
       self.dock_new_component.hide()
   ```

5. **Signals Conectados** (se aplicável):
   ```python
   # Conectar signals customizados
   self.dock_new_component.open_in_other_component_requested.connect(self._load_data_from_source)
   
   def _load_data_from_source(self, data_str: str):
       """Callback para abrir DATA no editor"""
       if not hasattr(self, 'component_viewer'):
           self._open_component()
       self.component_viewer.load_data_string(data_str)
       self.component_viewer.show()
   ```

6. **Traduções i18n Adicionadas**:
   ```data
   // src/i18n/en.data
   {
     "menu.tools.text_to_data": "Text to DATA Converter"
   }
   
   // src/i18n/pt_BR.data
   {
     "menu.tools.text_to_data": "Conversor de Texto para DATA"
   }
   ```

**Checklist de Teste de Integração**:
- ✅ **Menu acessível**: Verificar se item aparece no menu Tools
- ✅ **Dock abre**: Clicar no menu deve abrir o dock corretamente
- ✅ **Funcionalidade básica**: Testar conversão simples
- ✅ **Signals funcionam**: Testar integração com outros componentes (ex: Open in Editor)
- ✅ **Sem erros no console**: Não deve haver ImportError, AttributeError, etc.
- ✅ **Tradução funcionando**: Menu em PT-BR deve mostrar texto traduzido

**Exemplo Real (Task Example - Text to DATA Converter)**:
```python
✅ Import: from .gui import NewComponent
✅ Export: __all__ = [..., 'NewComponent']
✅ Menu: self.act_open_new_component = QAction(tr("menu.tools.text_to_data"), self)
✅ Init: self._open_new_component() chamado em __init__()
✅ Signal: open_in_other_component_requested.connect(self._load_data_from_source)
✅ i18n: EN "Text to DATA Converter", PT-BR "Conversor de Texto para DATA"
✅ Teste: Menu abre dock, conversão funciona, signal para editor OK
```

**Perguntas para Validar Integração**:
1. ❓ "O novo módulo está importado no arquivo principal (app.py)?"
2. ❓ "O módulo está exportado no __init__.py da pasta?"
3. ❓ "Há um item de menu para acessar a funcionalidade?"
4. ❓ "O item de menu está conectado ao método correto?"
5. ❓ "O dock/componente é inicializado no startup da aplicação?"
6. ❓ "Signals customizados estão conectados?"
7. ❓ "Traduções foram adicionadas (EN e PT-BR)?"
8. ❓ "A funcionalidade está acessível sem erros?"

**Por quê?**: Garantir que o código implementado está **realmente utilizável** pelo usuário final, não apenas "funciona isoladamente".

---

### 8️⃣ **Verificar Implementação GUI + Revisão de Código**
- **CRÍTICO**: Verificar se os componentes estão **integrados ao programa principal** e acessíveis
- **IMPORTANTE**: Durante a verificação, aplicar os **9 Critérios de Qualidade** ao código GUI
- Não basta implementar o módulo/dock, ele precisa estar **acessível e funcional** no app
- Verificar menu, imports, inicialização, conexões e qualidade do código

**Parte A - Verificação Funcional GUI (Integração)**:

1. **Import Correto no app.py**:
   ```python
   # ✅ Verificar se módulo foi importado
   from .gui import (
       ComponentJ, ComponentK, ComponentI,
       ComponentC, ComponentD, ComponentA,
       ComponentB, ComponentF, ComponentG, ComponentH,
       ComponentE, NewComponent  # ← NOVO módulo deve estar aqui
   )
   ```

2. **Export no __init__.py do Módulo**:
   ```python
   # src/gui/__init__.py
   from .text_to_data_dock import NewComponent
   
   __all__ = [
       'ComponentJ', 'ComponentK', 'ComponentI',
       'ComponentC', 'ComponentD', 'ComponentA',
       'ComponentB', 'ComponentF', 'ComponentG', 'ComponentH',
       'ComponentE', 'NewComponent'  # ← NOVO módulo exportado
   ]
   ```

3. **Menu Item Criado e Conectado**:
   ```python
   # Em _build_menu() ou similar
   m_tools = bar.addMenu(tr("menu.tools"))
   
   # Criar QAction
   self.act_open_new_component = QAction(tr("menu.tools.text_to_data"), self)
   
   # Adicionar ao menu
   m_tools.addAction(self.act_open_new_component)
   
   # Conectar signal
   self.act_open_new_component.triggered.connect(lambda: self.dock_new_component.show())
   ```

4. **Dock Inicializado no __init__() ou método de setup**:
   ```python
   # Em __init__() da MainWindow
   def __init__(self):
       super().__init__()
       # ... outros docks ...
       self._open_new_component()  # ← Inicializar dock
   
   def _open_new_component(self):
       self.dock_new_component = NewComponent(self)
       self.dock_new_component.open_in_other_component_requested.connect(self._load_data_from_source)
       self.addDockWidget(Qt.RightDockWidgetArea, self.dock_new_component)
       self.dock_new_component.hide()
   ```

5. **Signals Conectados** (se aplicável):
   ```python
   # Conectar signals customizados
   self.dock_new_component.open_in_other_component_requested.connect(self._load_data_from_source)
   
   def _load_data_from_source(self, data_str: str):
       """Callback para abrir DATA no editor"""
       if not hasattr(self, 'component_viewer'):
           self._open_component()
       self.component_viewer.load_data_string(data_str)
       self.component_viewer.show()
   ```

6. **Traduções i18n Adicionadas**:
   ```data
   // src/i18n/en.data
   {
     "menu.tools.text_to_data": "Text to DATA Converter"
   }
   
   // src/i18n/pt_BR.data
   {
     "menu.tools.text_to_data": "Conversor de Texto para DATA"
   }
   ```

**Checklist de Teste de Integração GUI**:
- ✅ **Menu acessível**: Verificar se item aparece no menu Tools
- ✅ **Dock abre**: Clicar no menu deve abrir o dock corretamente
- ✅ **Funcionalidade básica**: Testar conversão simples
- ✅ **Signals funcionam**: Testar integração com outros componentes (ex: Open in Editor)
- ✅ **Sem erros no console**: Não deve haver ImportError, AttributeError, etc.
- ✅ **Tradução funcionando**: Menu em PT-BR deve mostrar texto traduzido

**Parte B - Revisão de Qualidade do Código GUI (9 Critérios)**:

Durante a verificação do GUI, aplicar simultaneamente os seguintes critérios:

1. **❌ Omissão** - Verificar se GUI está completo:
   - [ ] Todos os widgets/controles necessários implementados?
   - [ ] Tratamento de erros em handlers (ex: FileNotFoundError)?
   - [ ] Cleanup de recursos (fechar arquivos, desconectar signals)?
   - [ ] Feedback visual para operações longas (QProgressBar, cursor busy)?

2. **🤔 Ambiguidade** - GUI deve ser claro:
   - [ ] Labels descritivos e claros?
   - [ ] Tooltips informativos nos controles?
   - [ ] Mensagens de erro descritivas (QMessageBox)?
   - [ ] Nomes de métodos intuitivos (_on_button_clicked vs _handle)?

3. **❗ Fato Incorreto** - Lógica GUI correta:
   - [ ] Signals conectados aos slots corretos?
   - [ ] Layouts corretos (QVBoxLayout, QHBoxLayout, QSplitter)?
   - [ ] Enable/disable de controles conforme estado?
   - [ ] Validação de entrada correta (QValidator)?

4. **♻️ Redundância** - Evitar repetição no GUI:
   - [ ] Widgets criados uma única vez?
   - [ ] Validações centralizadas (não duplicadas)?
   - [ ] Código de inicialização não repetido?

5. **⚠️ Inconsistência** - Padrão GUI consistente:
   - [ ] Nomenclatura uniforme (ed_ para QLineEdit, btn_ para QPushButton)?
   - [ ] Estilo de mensagens consistente?
   - [ ] Layout spacing/margin consistente?

6. **🔗 Falta de Integração** - GUI conectado:
   - [ ] Dock adicionado à MainWindow?
   - [ ] Menu item conectado ao dock.show()?
   - [ ] Signals customizados conectados?
   - [ ] Import presente em app.py?

7. **🧩 Menor Coesão** - Dock focado:
   - [ ] Dock faz apenas UI (não lógica de negócio)?
   - [ ] Lógica complexa em módulo separado?
   - [ ] Cada método tem responsabilidade única?

8. **🔗 Maior Acoplamento** - GUI desacoplado:
   - [ ] Dock não depende de implementação interna de outros docks?
   - [ ] Comunicação via signals/slots (não chamadas diretas)?
   - [ ] GUI testável independentemente (mock de lógica)?

9. **🗑️ Informação Estranha** - Código limpo:
   - [ ] Sem print() debug esquecidos?
   - [ ] Sem TODOs não resolvidos?
   - [ ] Sem widgets não utilizados?

**Exemplo de Revisão GUI Aplicada**:
```python
# ❌ ANTES - Omissão, Ambiguidade, Maior Acoplamento
class NewComponent(QDockWidget):
    def __init__(self):
        self.btn = QPushButton("Convert")  # Label vago
        self.btn.clicked.connect(self.convert)  # Sem tratamento de erro
    
    def convert(self):
        data = open(self.ed_file.text()).read()  # Sem validação, sem fechar
        data_str = my_convert(data)  # Lógica de negócio no GUI
        print(data_str)  # Debug esquecido

# ✅ DEPOIS - Completo, Claro, Desacoplado
class NewComponent(BaseDock):
    """Text to DATA Converter dock widget."""
    
    # Signal para comunicação
    open_in_other_component_requested = Signal(str)
    
    def __init__(self, parent=None):
        super().__init__(parent)
        self._create_widgets()
        self._setup_layout()
        self._connect_signals()
        
        # Controller para lógica de negócio
        self._converter = TextToJsonConverter()
    
    def _create_widgets(self):
        """Create UI widgets."""
        self.ed_file = QLineEdit()
        self.ed_file.setPlaceholderText("Enter file path or paste text")
        
        self.btn_convert = QPushButton("Convert to DATA")
        self.btn_convert.setToolTip("Convert text to DATA format")
        
        self.btn_open_component = QPushButton("Open in Editor")
        self.btn_open_component.setEnabled(False)  # Disabled até converter
    
    def _connect_signals(self):
        """Connect signals to slots."""
        self.btn_convert.clicked.connect(self._on_convert_clicked)
        self.btn_open_component.clicked.connect(self._on_open_component_clicked)
    
    def _on_convert_clicked(self):
        """Handle convert button click."""
        file_path = self.ed_file.text().strip()
        
        if not file_path:
            QMessageBox.warning(self, "Empty Input", "Please enter a file path or text.")
            return
        
        try:
            # Ler arquivo com context manager (garante fechar)
            if Path(file_path).exists():
                with open(file_path, 'r', encoding='utf-8') as f:
                    text = f.read()
            else:
                text = file_path  # Tratar como texto direto
            
            # Converter usando controller (desacoplamento)
            self._data_result = self._converter.convert(text)
            
            # Feedback visual
            QMessageBox.information(self, "Success", "Conversion successful!")
            self.btn_open_component.setEnabled(True)
        
        except FileNotFoundError:
            QMessageBox.critical(self, "File Not Found", f"File not found: {file_path}")
        except Exception as e:
            QMessageBox.critical(self, "Conversion Error", f"Error: {str(e)}")
    
    def _on_open_component_clicked(self):
        """Handle open in editor button click."""
        if hasattr(self, '_data_result'):
            self.open_in_other_component_requested.emit(self._data_result)  # Signal
```

**Ferramentas Recomendadas GUI**:
```bash
# Verificar imports Qt não utilizados
grep -r "from PySide6" src/gui/ | cut -d: -f2 | sort | uniq

# Verificar signals não conectados (manual review)
grep -r "Signal(" src/gui/ | grep -v ".connect("

# Verificar widgets não utilizados (manual review)
grep -r "self\.\w\+ = Q" src/gui/

# Verificar debug prints (CRÍTICO)
grep -r "print(" src/gui/ --exclude="*_test.py"
```

**Perguntas para Validar GUI**:
1. ❓ "O dock está completamente integrado no menu e MainWindow?"
2. ❓ "Todos os signals estão conectados e funcionando?"
3. ❓ "Há tratamento de erros com feedback visual (QMessageBox)?"
4. ❓ "Lógica de negócio está separada do código GUI?"
5. ❓ "Código está livre de debug prints e TODOs não resolvidos?"
6. ❓ "Labels, tooltips e mensagens são claros e descritivos?"
7. ❓ "Recursos (arquivos, conexões) são fechados corretamente?"

**Exemplo Real (Task Example - Text to DATA Converter)**:
```python
✅ Import: from .gui import NewComponent
✅ Export: __all__ = [..., 'NewComponent']
✅ Menu: self.act_open_new_component.triggered.connect(lambda: self.dock_new_component.show())
✅ Init: self._open_new_component() chamado em __init__()
✅ Signal: open_in_other_component_requested.connect(self._load_data_from_source)
✅ i18n: EN "Text to DATA Converter", PT-BR "Conversor de Texto para DATA"
✅ Revisão: Sem debug prints, tratamento de erros OK, lógica desacoplada
✅ Teste: Menu abre dock, conversão funciona, signal para editor OK
```

---

### 9️⃣ **Verificar Integração com Programa Principal**
- **CRÍTICO**: Após implementar CLI e GUI, **verificar se tudo está integrado e funcionando no contexto do programa principal**
- Não basta ter código funcionando isoladamente, precisa estar **acessível e operacional** no aplicativo
- Verificar fluxo completo: menu → ação → resultado
- Testar manualmente a funcionalidade no programa rodando

**Checklist de Integração Completa**:

1. **Teste de Fluxo Completo GUI**:
   ```bash
   # Iniciar aplicativo
   python -m app --gui
   
   # Testar manualmente:
   [ ] Menu item aparece corretamente?
   [ ] Clicar no menu abre o dock?
   [ ] Dock exibe todos os controles?
   [ ] Funcionalidade básica funciona (conversão, busca, etc)?
   [ ] Signals entre componentes funcionam (ex: "Open in Editor")?
   [ ] Mensagens de erro aparecem quando apropriado?
   [ ] Tradução i18n funciona (mudar idioma e verificar)?
   ```

2. **Teste de Fluxo Completo CLI**:
   ```bash
   # Testar help
   python -m app convert --help
   
   # Testar funcionalidade
   python -m app convert test.txt --pretty -o output.data
   
   # Testar pipes
   echo "name: John" | python -m app convert -
   
   # Verificar:
   [ ] Help text aparece?
   [ ] Argumentos são reconhecidos?
   [ ] Funcionalidade executa sem erros?
   [ ] Output está correto?
   [ ] Exit codes corretos (0=success, 1=error)?
   ```

3. **Teste de Integração entre Componentes**:
   ```bash
   # Exemplo: Converter texto → Abrir no editor
   [ ] Clicar em "Open in Editor" no Text to DATA Converter abre o Editor?
   [ ] DATA é carregado corretamente no Editor?
   [ ] Editor pode salvar o resultado?
   
   # Exemplo: Busca → Abrir arquivo
   [ ] Clicar em resultado de busca abre arquivo correto?
   [ ] Posição do cursor vai para linha correta?
   ```

4. **Teste de Robustez**:
   ```bash
   # Cenários de erro
   [ ] Arquivo não encontrado exibe mensagem clara?
   [ ] Input inválido é tratado graciosamente?
   [ ] Operação cancelada não deixa estado inconsistente?
   [ ] Recursos são liberados corretamente (arquivos fechados, memória)?
   ```

5. **Teste de Performance** (se aplicável):
   ```bash
   # Arquivos grandes
   [ ] Processa arquivos >10MB sem travar?
   [ ] Interface permanece responsiva durante operação longa?
   [ ] Progress bar/feedback visual funciona?
   [ ] Cancelamento funciona durante operação longa?
   ```

**Exemplo Real de Problema de Integração**:
```python
# ❌ PROBLEMA ENCONTRADO NA INTEGRAÇÃO:
# Task Example - Text to DATA Converter CLI
# Problema: Extractor() estava sendo chamado sem 3 parâmetros obrigatórios

# ANTES (quebrava na integração):
def main():
    if args.command == 'convert':
        extractor = Extractor()  # ❌ TypeError: missing 3 required arguments

# DEPOIS (corrigido):
def main():
    if args.command == 'convert':
        extractor = Extractor(
            avoid_keys="",
            avoid_keys_parameter="equals",
            with_quotation_marks=False
        )  # ✅ Funciona!
```

**Perguntas para Validar Integração**:
1. ❓ "O usuário final consegue acessar a funcionalidade facilmente?"
2. ❓ "Todos os fluxos de uso funcionam end-to-end?"
3. ❓ "Há algum erro ou warning no console durante uso normal?"
4. ❓ "A funcionalidade está consistente com o resto do aplicativo?"
5. ❓ "Documentação (help text, tooltips) está clara e correta?"

**Por quê esta etapa é crítica?**:
- ✅ Detecta problemas que testes unitários não pegam
- ✅ Valida experiência real do usuário
- ✅ Garante que todo o trabalho é realmente utilizável
- ✅ Evita surpresas após commit (código testado ≠ código integrado)

---

### 🔟 **Fazer Testes**
- **Obrigatório**: Testes unitários para cada função pública
- **Meta**: 100% de cobertura das funcionalidades implementadas
- **Ferramentas**: `unittest` (nativo) ou `pytest`
- **CRÍTICO**: Testar o sistema **após integração** (GUI + CLI integrados)
- **IMPORTANTE**: Executar **APÓS** revisão de código (Etapas 7 e 8)

**Categorias de Testes**:
1. **Happy Path**: Casos normais de uso
2. **Edge Cases**: Valores vazios, None, strings longas
3. **Error Handling**: Exceções esperadas
4. **Integration**: Fluxo completo (incluindo integração GUI/CLI)
5. **Quality Validation**: Testes que validam ausência dos 9 problemas das Etapas 7 e 8

**Exemplo de Suite de Testes**:
```python
✅ test_basic_functionality()
✅ test_with_valid_input()
✅ test_edge_case_empty()
✅ test_edge_case_large_input()
✅ test_error_handling()
✅ test_integration_complete_flow()
# ... testes cobrindo casos normais, edge cases e integração
```

**Por quê testar DEPOIS da integração e revisão?**:
- Garante que testes validam o **sistema integrado**, não componentes isolados
- Detecta problemas de integração durante os testes
- Valida que features realmente funcionam no contexto do aplicativo
- Evita falsos positivos (testes passam mas feature não está acessível)
- Código já foi revisado, então testes validam **código de qualidade**

**Por quê?**: Garantir qualidade, evitar regressões, facilitar manutenção futura.

---

#### 🛡️ **Etapa 9.1 - Segurança em Testes (CRÍTICO)**

**Problema Comum em Testes**:
- Testes GUI podem travar em **loop infinito** sem timeout
- Falta de detecção automática de deadlock ou travamento
- Testes aguardam recursos não disponíveis (ex: display X11 em ambiente headless)

**Soluções Obrigatórias**:

1. **⏱️ Timeout Máximo Obrigatório** (30s por teste):
   ```bash
   # SEMPRE usar timeout em testes
   pytest tests/test_*.py --timeout=30 -v
   
   # Instalar plugin pytest-timeout se necessário
   pip install pytest-timeout
   ```

2. **🚨 Detecção de Loop Infinito** (warning em 10s):
   ```bash
   # Timeout mais agressivo para detectar loops
   timeout 10s pytest tests/test_specific.py || echo "⚠️ TIMEOUT: Possível loop infinito detectado!"
   ```

3. **🖥️ Ambiente Headless Obrigatório** (testes GUI sem display):
   ```bash
   # Usar Qt offscreen platform
   QT_QPA_PLATFORM=offscreen pytest tests/test_gui_*.py -v --timeout=30
   
   # OU usar pytest-xvfb para ambiente virtual X11
   pip install pytest-xvfb
   pytest tests/test_gui_*.py --xvfb-backend xvfb --timeout=30
   ```

4. **✅ Dry-Run Obrigatório** (antes de executar):
   ```bash
   # 1. Verificar sintaxe
   python -m py_compile tests/test_*.py && echo "✅ Sintaxe válida"
   
   # 2. Verificar imports
   python -c "from tests.test_module import *; print('✅ Imports OK')"
   
   # 3. Listar testes sem executar
   pytest tests/test_*.py --collect-only
   ```

5. **⏲️ Monitoramento de Tempo** (registrar duração):
   ```bash
   # Medir tempo total e salvar log
   time pytest tests/test_*.py -v --timeout=30 | tee test_output.log
   
   # Usar pytest-benchmark para métricas
   pytest tests/test_*.py --benchmark-only --timeout=30
   ```

**Por quê?**: Evitar travamentos infinitos, proteger tempo de desenvolvimento, garantir testes confiáveis.

---

### 1️⃣1️⃣ **Organizar Pasta Raiz do Projeto**
- ✅ Imports validados (módulo carrega sem erros)
- 📝 **Limitação documentada**: Testes GUI requerem ambiente headless não configurado

---

#### 🔬 **Etapa 9.2 - Testes em Threads/Processos com Monitoramento (AVANÇADO)**

**Objetivo**: Controle total sobre execução de testes com possibilidade de **interromper**, **monitorar** e **registrar** progresso em tempo real.

**Quando Usar**:
- Testes GUI que podem travar
- Testes de longa duração (>1 min)
- Testes com dependências externas (rede, banco de dados)
- Necessidade de logging em tempo real
- Necessidade de cancelamento manual durante execução

**Implementação com `multiprocessing.Process`**:

```python
# tests/test_runner_monitored.py
import multiprocessing as mp
import time
import sys
from queue import Empty

def run_tests_in_process(test_module: str, queue: mp.Queue, timeout: int = 30):
    """
    Executa testes em processo separado com logging para queue.
    
    Args:
        test_module: Módulo de teste (ex: 'tests.test_file_list_dock')
        queue: Queue para comunicação de progresso
        timeout: Timeout em segundos
    """
    try:
        import pytest
        
        # Configurar logging em tempo real
        class QueueReporter:
            def __init__(self, queue):
                self.queue = queue
            
            def pytest_runtest_logreport(self, report):
                """Hook do pytest para capturar resultados."""
                if report.when == 'call':
                    status = '✅ PASS' if report.passed else '❌ FAIL'
                    self.queue.put({
                        'type': 'test_result',
                        'test': report.nodeid,
                        'status': status,
                        'duration': report.duration
                    })
        
        # Executar pytest com reporter customizado
        queue.put({'type': 'info', 'msg': f'Iniciando testes: {test_module}'})
        
        result = pytest.main([
            test_module,
            '-v',
            f'--timeout={timeout}',
            '--tb=short',
            '-p', 'no:cacheprovider'  # Desabilitar cache
        ])
        
        queue.put({'type': 'info', 'msg': f'Testes finalizados. Exit code: {result}'})
        queue.put({'type': 'exit', 'code': result})
        
    except Exception as e:
        queue.put({'type': 'error', 'msg': str(e)})
        queue.put({'type': 'exit', 'code': 1})

def monitor_test_execution(test_module: str, max_timeout: int = 300):
    """
    Monitora execução de testes com controle total.
    
    Args:
        test_module: Módulo de teste
        max_timeout: Timeout máximo em segundos (padrão: 5 min)
    
    Returns:
        dict: Resultado da execução com estatísticas
    """
    queue = mp.Queue()
    process = mp.Process(
        target=run_tests_in_process,
        args=(test_module, queue, 30)
    )
    
    print(f"🚀 Iniciando testes: {test_module}")
    print(f"⏱️  Timeout máximo: {max_timeout}s")
    print(f"📊 Monitoramento ativo. Pressione Ctrl+C para cancelar.\n")
    
    process.start()
    start_time = time.time()
    results = {'passed': 0, 'failed': 0, 'tests': []}
    
    try:
        while process.is_alive():
            elapsed = time.time() - start_time
            
            # Verificar timeout global
            if elapsed > max_timeout:
                print(f"\n⚠️  TIMEOUT GLOBAL ({max_timeout}s excedido)")
                process.terminate()
                process.join(timeout=5)
                if process.is_alive():
                    process.kill()
                return {'status': 'timeout', 'elapsed': elapsed, 'results': results}
            
            # Ler mensagens da queue (não-bloqueante)
            try:
                msg = queue.get(timeout=0.5)
                
                if msg['type'] == 'test_result':
                    print(f"  {msg['status']} {msg['test']} ({msg['duration']:.2f}s)")
                    results['tests'].append(msg)
                    if '✅' in msg['status']:
                        results['passed'] += 1
                    else:
                        results['failed'] += 1
                
                elif msg['type'] == 'info':
                    print(f"ℹ️  {msg['msg']}")
                
                elif msg['type'] == 'error':
                    print(f"❌ ERRO: {msg['msg']}")
                
                elif msg['type'] == 'exit':
                    process.join(timeout=2)
                    elapsed = time.time() - start_time
                    print(f"\n✅ Testes finalizados em {elapsed:.2f}s")
                    return {
                        'status': 'completed',
                        'exit_code': msg['code'],
                        'elapsed': elapsed,
                        'results': results
                    }
            
            except Empty:
                # Nenhuma mensagem, continuar monitorando
                pass
            
            # Mostrar progresso a cada 10s
            if int(elapsed) % 10 == 0 and int(elapsed) > 0:
                print(f"⏳ Executando... {int(elapsed)}s ({results['passed']} passed, {results['failed']} failed)")
    
    except KeyboardInterrupt:
        print("\n⚠️  Cancelamento manual (Ctrl+C)")
        process.terminate()
        process.join(timeout=5)
        if process.is_alive():
            process.kill()
        elapsed = time.time() - start_time
        return {'status': 'cancelled', 'elapsed': elapsed, 'results': results}
    
    finally:
        if process.is_alive():
            process.terminate()
            process.join(timeout=5)

# Exemplo de uso:
if __name__ == '__main__':
    result = monitor_test_execution('tests/test_advanced_file_search.py', max_timeout=300)
    
    print(f"\n{'='*60}")
    print(f"Status: {result['status']}")
    print(f"Tempo: {result['elapsed']:.2f}s")
    print(f"Passed: {result['results']['passed']}")
    print(f"Failed: {result['results']['failed']}")
    print(f"{'='*60}")
```

**Uso Prático**:

```bash
# 1. Criar runner monitorado
cat > tests/run_tests_monitored.py << 'EOF'
# [código acima]
EOF

# 2. Executar com monitoramento
python tests/run_tests_monitored.py

# 3. Cancelar a qualquer momento (Ctrl+C)
# O processo será terminado graciosamente
```

**Vantagens**:
- ✅ **Controle total**: Pode cancelar testes a qualquer momento
- ✅ **Logging em tempo real**: Vê progresso de cada teste
- ✅ **Timeout global + individual**: Dupla proteção
- ✅ **Estatísticas**: Passa/falha em tempo real
- ✅ **Isolamento**: Testes rodam em processo separado (não travam o terminal)
- ✅ **Cleanup garantido**: `terminate()` + `kill()` forçado se necessário

**Configurações Opcionais**:

1. **Logging em Arquivo** (além de stdout):
   ```python
   # Adicionar ao run_tests_in_process:
   import logging
   logging.basicConfig(
       filename=f'test_{time.time()}.log',
       level=logging.INFO,
       format='%(asctime)s - %(message)s'
   )
   ```

2. **Notificação Sonora** (ao finalizar):
   ```python
   import os
   # No final de monitor_test_execution:
   os.system('paplay /usr/share/sounds/freedesktop/stereo/complete.oga')
   ```

3. **Integração com CI/CD**:
   ```python
   # Retornar exit code correto:
   sys.exit(0 if result['status'] == 'completed' and result['results']['failed'] == 0 else 1)
   ```

**Checklist Adicional (Etapa 9.2 - Opcional)**:
```
[ ] Criar test_runner_monitored.py com multiprocessing
[ ] Definir timeout global (padrão: 5 min)
[ ] Definir timeout individual por teste (padrão: 30s)
[ ] Implementar logging em tempo real (Queue)
[ ] Testar cancelamento manual (Ctrl+C)
[ ] Verificar cleanup de processos (ps aux | grep pytest)
```

**Quando NÃO usar**:
- Testes simples e rápidos (<10s total)
- Testes sem GUI (backend puro)
- CI/CD com timeout nativo configurado
- Primeira execução de testes (overhead desnecessário)

---

### 1️⃣1️⃣ **Organizar Pasta Raiz do Projeto**
- **CRÍTICO**: Antes da documentação e do commit, **organizar a pasta raiz recursivamente**
- **OBRIGATÓRIO**: Arquivos devem estar organizados nas pastas corretas antes do commit
- Remover arquivos temporários, backups desnecessários
- Verificar se todos os arquivos estão nos lugares corretos
- Limpar cache e arquivos gerados (`__pycache__`, `.pyc`)
- Garantir que `.gitignore` está atualizado

**Checklist de Organização**:
1. **Remoção de Arquivos Temporários**:
   ```bash
   # Remover backups antigos
   rm -f *.backup_* *.bak *~
   
   # Limpar cache Python
   find . -type d -name "__pycache__" -exec rm -rf {} +
   find . -type f -name "*.pyc" -delete
   find . -type f -name "*.pyo" -delete
   ```

2. **Verificação de Estrutura de Diretórios (OBRIGATÓRIO)**:
   - `src/` - código-fonte
   - `tests/` - **TODOS os arquivos de teste** (obrigatório)
   - `docs/` - **TODOS os documentos e arquivos markdown** (obrigatório)
   - Arquivos raiz organizados (README, setup.py, etc.)

3. **Organização Recursiva Obrigatória**:
   
   **⚠️ REGRA FUNDAMENTAL**: 
   > Antes do commit, os arquivos devem ser organizados nas pastas recursivamente. Isto é **obrigatório** para manter o ambiente limpo e organizado.

   **Regras Específicas por Tipo de Arquivo**:
   
   a) **Arquivos de Teste** → `tests/`
      - ✅ `test_*.py`, `*_test.py` → `tests/`
      - ✅ Estrutura de testes deve espelhar estrutura do código
      - ✅ Exemplo: `tests/unit/`, `tests/integration/`, `tests/fixtures/`
   
   b) **Documentos e Markdown** → `docs/`
      - ✅ Todos arquivos `.md` (exceto README.md raiz) → `docs/`
      - ✅ Arquivos de documentação → `docs/`
      - ✅ **Organização recursiva dentro de `docs/`**:
        - `docs/api/` - Documentação de API
        - `docs/tutorials/` - Tutoriais
        - `docs/architecture/` - Decisões arquiteturais
        - `docs/user-guide/` - Guias de usuário
        - `docs/dev-guide/` - Guias de desenvolvimento
      - ✅ Criar subpastas que identificam contexto dos arquivos
   
   c) **Código-Fonte** → `src/` ou pasta apropriada
      - ✅ Organizar por módulos/features
      - ✅ Exemplo: `src/core/`, `src/utils/`, `src/api/`

**Exemplo Completo**:
```bash
# ANTES (pasta desorganizada):
├── src/
├── test_utils.py              ❌ teste fora de tests/
├── API_DOCS.md                ❌ doc fora de docs/
├── tutorial.md                ❌ doc fora de docs/
├── apply_v2913_patches.py     ❌ temporário
├── test_temp.py               ❌ teste temporário
├── backup_old/                ❌ backup antigo
├── __pycache__/               ❌ cache
└── file.py.backup_v2913       ❌ backup desnecessário

# DEPOIS (organizado recursivamente):
├── src/
│   ├── core/
│   └── utils/
├── tests/                     ✅ TODOS os testes
│   ├── unit/
│   │   └── test_utils.py     ✅ teste movido
│   └── integration/
├── docs/                      ✅ TODOS os documentos
│   ├── api/
│   │   └── API_DOCS.md       ✅ doc movido
│   └── tutorials/
│       └── tutorial.md       ✅ doc movido
└── README.md                  ✅ README raiz mantido
```

**Por quê?**: Manter repositório limpo, evitar commits de lixo, facilitar navegação, profissionalismo, organização recursiva garante escalabilidade. Documentar o estado **limpo** e **organizado** do projeto.

---

### 1️⃣2️⃣ **Preencher Nova Documentação**
- **Atualizar arquivo de tarefas/requisitos**: Marcar tasks como `[X]` completas
- **Criar SPECIFICATIONS.md**: Documento detalhado da versão
- **Atualizar estatísticas**: Percentual de conclusão do projeto
- **🤖 [OPCIONAL] Gerenciar recomendações de novas tarefas pela IA**

---

### ⚠️ **REQUISITO OBRIGATÓRIO: Documentação Completa de Todas as Implementações da IA**

> **CRÍTICO PARA IAs**: Tudo aquilo que a inteligência artificial faz no projeto, em cada ciclo de implementação, em cada código, cada funcionalidade implementada, **DEVE SER DOCUMENTADO NA PASTA `docs/` COMO REQUISITO OBRIGATÓRIO** para demarcar as novas funcionalidades e novos comportamentos.

#### **🤖 Regra de Ouro para Assistentes de IA**

**Se você é uma IA implementando código:**
- ✅ **VOCÊ DEVE** documentar TODAS as implementações que realizar em cada ciclo
- ✅ **VOCÊ DEVE** criar/atualizar arquivos na pasta `docs/` para cada funcionalidade nova
- ✅ **VOCÊ DEVE** descrever TODOS os comportamentos novos implementados
- ✅ **VOCÊ DEVE** marcar claramente o que foi adicionado, modificado ou removido
- ✅ **VOCÊ DEVE** incluir exemplos de uso das novas funcionalidades
- ✅ **VOCÊ DEVE** documentar decisões técnicas e arquiteturais tomadas

#### **📝 O Que Deve Ser Documentado (OBRIGATÓRIO)**

Para **CADA ciclo de implementação**, a IA deve documentar na pasta `docs/`:

1. **Funcionalidades Implementadas**:
   - Nome e descrição detalhada de cada nova funcionalidade
   - Propósito e casos de uso
   - Comportamento esperado e edge cases

2. **Código Criado/Modificado**:
   - Arquivos novos criados (path completo + descrição)
   - Arquivos modificados (path + o que foi alterado)
   - Funções/classes principais adicionadas ou modificadas

3. **Arquitetura e Decisões Técnicas**:
   - Padrões de design aplicados (GoF, GRASP)
   - Estrutura de módulos e suas responsabilidades
   - Decisões arquiteturais e suas justificativas

4. **Comportamentos e Integrações**:
   - Como a funcionalidade interage com o resto do sistema
   - Dependências criadas ou modificadas
   - Fluxos de dados e controle

5. **Testes Implementados**:
   - Quantidade e tipos de testes criados
   - Cenários de teste cobertos
   - Cobertura de testes alcançada

6. **Exemplos de Uso**:
   - Como utilizar a nova funcionalidade
   - Exemplos de código (CLI, API, GUI)
   - Casos de uso práticos

#### **📂 Estrutura Obrigatória de Documentação**

A pasta `docs/` deve conter no mínimo:

```
docs/
├── REQUIREMENTS.md          # Lista de tarefas e requisitos (atualizado a cada ciclo)
├── vX.Y.Z-SPECIFICATIONS.md # Especificações detalhadas da versão atual
├── CHANGELOG.md             # Histórico de mudanças (o que foi implementado e quando)
├── ARCHITECTURE.md          # Decisões arquiteturais e estrutura do projeto
└── [feature]-GUIDE.md       # Guias específicos para funcionalidades complexas
```

**Criação Automática**:
- Se a pasta `docs/` não existe, ela **DEVE SER CRIADA AUTOMATICAMENTE** pela IA
- Se um arquivo de documentação não existe, ele **DEVE SER CRIADO** pela IA no primeiro ciclo
- Todos os arquivos devem ser atualizados **A CADA CICLO** de implementação

#### **📋 Template Mínimo para SPECIFICATIONS.md**

Cada arquivo de especificações de versão deve conter no mínimo:

```markdown
# [Nome do Projeto] vX.Y.Z - [Nome Descritivo]

**Data**: DD/MM/AAAA
**Sprint**: X tasks em Y horas
**Metodologia**: Protocolo Simplicidade 1

## 📋 Objetivos da Sprint
- Task #X: [descrição]
- Task #Y: [descrição]

## 🎯 Funcionalidades Implementadas

### Task #X: [Nome da Funcionalidade]
**Problema Original**:
- [Descrição do problema ou necessidade]

**Solução Implementada**:
- ✅ [Feature/função 1]: [descrição detalhada]
- ✅ [Feature/função 2]: [descrição detalhada]

**Comportamentos Novos**:
- [Comportamento 1]: [como funciona]
- [Comportamento 2]: [como funciona]

**Arquitetura**:
- Padrão [X] aplicado: [justificativa]
- Módulos criados: [lista com responsabilidades]

**Arquivos Criados/Modificados**:
- `path/to/file.py` (+XXX linhas) - [descrição]
- `path/to/test.py` (NOVO) - [descrição]

**Testes**:
- XX unit tests (YY passing)
- Cenários cobertos: [lista]

**Exemplo de Uso**:
```python
# Exemplo prático de como usar a funcionalidade
```

## ✅ Qualidade (Protocolo Simplicidade 1)
- ✅ Arquitetura Modular
- ✅ Type Hints (100%)
- ✅ Docstrings completas
- ✅ Tratamento de erros
- ✅ Testes (X passing)
- ✅ Commits semânticos
- ✅ **Documentação completa na pasta docs/**
- ✅ Código limpo (PEP8/ESLint/etc)

## 📊 Estatísticas
- TOTAL: X% completo (Y/Z tasks)
- Commits: N pushed
```

#### **🔍 Validação da Documentação**

Antes de finalizar cada ciclo (Etapa 13 - Commit), a IA **DEVE VERIFICAR**:

- [ ] ✅ Pasta `docs/` existe e está atualizada
- [ ] ✅ Arquivo SPECIFICATIONS.md criado/atualizado para este ciclo
- [ ] ✅ TODAS as funcionalidades implementadas estão documentadas
- [ ] ✅ TODOS os comportamentos novos estão descritos
- [ ] ✅ TODOS os arquivos criados/modificados estão listados
- [ ] ✅ Decisões técnicas e arquiteturais estão justificadas
- [ ] ✅ Exemplos de uso estão incluídos
- [ ] ✅ Testes estão documentados

**Se algum item não estiver completo, a IA NÃO DEVE prosseguir para o commit** até completar a documentação.

#### **📌 Rationale: Por Quê Este Requisito é OBRIGATÓRIO**

1. **Rastreabilidade**: Permite entender TUDO que foi implementado ao longo do tempo
2. **Manutenibilidade**: Facilita manutenção futura (pelo mesmo dev ou outros)
3. **Conhecimento Organizacional**: Preserva decisões e contexto do projeto
4. **Onboarding**: Novos desenvolvedores/IAs entendem rapidamente o sistema
5. **Auditoria**: Possibilita revisão e validação de implementações
6. **Continuidade**: Garante que funcionalidades não sejam esquecidas ou perdidas
7. **Profissionalismo**: Projetos sérios têm documentação completa e atualizada

**Este requisito transforma a pasta `docs/` em um histórico vivo e completo de tudo que foi implementado no projeto.**

---

**📋 Gerenciamento do TASKS.md**:

**Regra Geral**:
- Se existe arquivo de tarefas/requisitos (ex: `TASKS.md`, `TODO.md`, `requirements.md`):
  - ✅ **Marcar tasks como completas** após implementação: `[ ]` → `[X]`
  - ✅ **Atualizar estatísticas** (percentuais, contadores)
  - ✅ **Adicionar notas de conclusão** (data, versão, descrição breve)
  - 🤖 **[OPCIONAL] Adicionar novas tarefas recomendadas pela IA** (ver seção abaixo)
  
- Se **NÃO existe** arquivo de tarefas/requisitos:
  - ❓ **Perguntar ao usuário** qual o local/path do arquivo
  - ❓ **Perguntar sobre próximas tarefas e requisitos** caso não haja documento formal
  - ❓ **Sugerir criação** de `TASKS.md` como arquivo padrão

---

### 📊 **Legenda de Classificação de Tarefas**

**Objetivo**: Padronizar a classificação e priorização de tarefas para facilitar a organização pela IA e compreensão entre diferentes sistemas de inteligência artificial.

#### **Status da Tarefa**

As tarefas devem ser marcadas com indicadores de status para rastreamento visual:

- 🔴 **Not Started** (Não Iniciada) - Aguardando início, sem trabalho realizado
- 🟡 **In Progress** (Em Progresso) - Desenvolvimento ativo, trabalho em andamento
- 🟢 **Done** (Concluída) - Implementada, testada e finalizada
- 🔵 **Blocked** (Bloqueada) - Impedida por dependência externa ou problema técnico

**Exemplo de uso**:
```markdown
- 🔴 [ ] Implementar autenticação OAuth2
- 🟡 [ ] Adicionar validação de formulários (50% completo)
- 🟢 [x] Configurar banco de dados PostgreSQL
- 🔵 [ ] Deploy em produção (aguardando aprovação de infra)
```

#### **Complexidade da Tarefa**

Classificação baseada em tempo estimado, risco e quantidade de dependências:

- 🟢 **Simples** (0-1h) - Baixo risco, poucas dependências, escopo claro e bem definido
  - Exemplos: Ajustar texto, corrigir typo, adicionar tooltip, pequeno bugfix
  - Características: Modificação de 1-2 arquivos, sem impacto em outros módulos
  
- 🟡 **Média** (1-2h) - Risco médio, algumas integrações, pode requerer testes adicionais
  - Exemplos: Nova funcionalidade simples, refatoração de módulo, integração com API
  - Características: Modificação de 3-5 arquivos, alguma integração com sistema existente
  
- 🔴 **Complexa** (>2h) - Alto risco, muitas dependências, escopo aberto ou ambíguo
  - Exemplos: Arquitetura nova, migração de banco, feature crítica com muitos edge cases
  - Características: Múltiplos arquivos afetados, alta complexidade algorítmica, requer pesquisa

**Exemplo de uso**:
```markdown
## Backlog por Complexidade

### 🟢 Tarefas Simples (0-1h)
- [ ] Adicionar loading spinner no botão de submit
- [ ] Corrigir alinhamento do header

### 🟡 Tarefas Médias (1-2h)
- [ ] Implementar paginação na listagem
- [ ] Adicionar filtros de busca avançada

### 🔴 Tarefas Complexas (>2h)
- [ ] Migrar autenticação para SSO
- [ ] Implementar sistema de cache distribuído
```

#### **Priorização MoSCoW**

Framework para classificar a importância relativa de cada tarefa:

- 🔴 **Must Have** - Crítico para o funcionamento do sistema, bloqueante para release
  - Sem isso, o produto não funciona ou não atende requisito fundamental
  - Exemplos: Login, salvamento de dados, funcionalidade core do produto
  
- 🟡 **Should Have** - Importante mas não bloqueante, pode ser adiado se necessário
  - Adiciona valor significativo mas sistema funciona sem
  - Exemplos: Exportação de relatórios, notificações por email, dark mode
  
- 🟢 **Could Have** - Desejável se houver tempo, baixa prioridade
  - Nice to have, melhora experiência mas não é essencial
  - Exemplos: Animações, easter eggs, features experimentais
  
- ⚪ **Won't Have** (Later) - Explicitamente fora do escopo atual, para versões futuras
  - Boa ideia mas não para agora, documentar para backlog futuro
  - Exemplos: Versão mobile app, integração com sistema legado

**Exemplo de uso**:
```markdown
## Priorização MoSCoW - Sprint v1.0

### 🔴 MUST HAVE (Obrigatório)
- [ ] Sistema de autenticação funcional
- [ ] CRUD completo de usuários
- [ ] Persistência de dados

### 🟡 SHOULD HAVE (Importante)
- [ ] Recuperação de senha
- [ ] Validação de email
- [ ] Logs de auditoria

### 🟢 COULD HAVE (Desejável)
- [ ] Avatar customizável
- [ ] Tema escuro
- [ ] Atalhos de teclado

### ⚪ WON'T HAVE (Futuro)
- [ ] Integração com redes sociais
- [ ] Aplicativo mobile nativo
```

#### **Frameworks Avançados de Priorização (OPCIONAL)**

Para projetos complexos que requerem análise quantitativa mais sofisticada:

##### **Matriz RICE** (Reach, Impact, Confidence, Effort)

Pontuação: `Score RICE = (Reach × Impact × Confidence) / Effort`

- **Reach** (Alcance): Quantas pessoas serão impactadas? (ex: 100 usuários/mês)
- **Impact** (Impacto): Quanto impacto por pessoa? (0.25=mínimo, 3=massivo)
- **Confidence** (Confiança): Quão certos estamos? (50%=baixa, 100%=alta)
- **Effort** (Esforço): Quantas pessoas-hora? (ex: 2h, 10h, 40h)

**Exemplo**:
```markdown
| Task | Reach | Impact | Confidence | Effort | Score RICE |
|------|-------|--------|------------|--------|-----------|
| Feature A | 1000 | 3 | 100% | 5h | 600 |
| Feature B | 500 | 2 | 80% | 10h | 80 |
| Feature C | 100 | 1 | 50% | 2h | 25 |

Prioridade: A > B > C
```

##### **Matriz de Eisenhower** (Urgente vs Importante)

Classificação em quadrantes para gestão de tempo:

- ⭐ **Q1: Urgente + Importante** → Fazer IMEDIATAMENTE
  - Crises, bugs críticos em produção, deadlines iminentes
  
- 📅 **Q2: Não Urgente + Importante** → PLANEJAR e fazer depois
  - Planejamento estratégico, refatoração, documentação, testes
  
- 🔀 **Q3: Urgente + Não Importante** → DELEGAR ou automatizar
  - Interrupções, algumas reuniões, emails não críticos
  
- 🗑️ **Q4: Não Urgente + Não Importante** → ELIMINAR
  - Distrações, tarefas que não agregam valor real

**Exemplo**:
```markdown
## Matriz de Eisenhower - Sprint Atual

### ⭐ Q1: FAZER AGORA (Urgente + Importante)
- [ ] 🔴 Corrigir bug de segurança reportado
- [ ] 🔴 Implementar feature bloqueante para cliente

### 📅 Q2: PLANEJAR (Importante + Não Urgente)
- [ ] 🟡 Refatorar módulo de autenticação
- [ ] 🟡 Escrever documentação técnica
- [ ] 🟡 Implementar testes unitários faltantes

### 🔀 Q3: DELEGAR (Urgente + Não Importante)
- [ ] 🟢 Responder emails de stakeholders
- [ ] 🟢 Atualizar status report

### 🗑️ Q4: ELIMINAR (Não Urgente + Não Importante)
- [ ] ⚪ Pesquisar nova biblioteca X (não necessária agora)
```

#### **Combinando Indicadores**

Para máxima clareza, combine status + complexidade + priorização:

```markdown
## Sprint v2.3 - Backlog Organizado

### 🔴 MUST HAVE
- 🔴🟢 [ ] Adicionar botão de logout (Not Started, Simples, 0.5h)
- 🟡🟡 [ ] Implementar reset de senha (In Progress, Média, 1.5h, 60% completo)
- 🟢🟢 [x] Configurar HTTPS (Done, Simples, 1h)
- 🔵🔴 [ ] Migrar para PostgreSQL (Blocked, Complexa, 4h, aguardando DBA)

### 🟡 SHOULD HAVE  
- 🔴🟡 [ ] Adicionar filtros de busca (Not Started, Média, 2h)
- 🟡🟢 [ ] Loading states (In Progress, Simples, 0.5h)

### 🟢 COULD HAVE
- 🔴🟡 [ ] Dark mode (Not Started, Média, 1.5h)
```

**Interpretação dos Indicadores Combinados**:
- **Primeiro emoji** = Status (🔴 Not Started, 🟡 In Progress, 🟢 Done, 🔵 Blocked)
- **Segundo emoji** = Complexidade (🟢 Simples, 🟡 Média, 🔴 Complexa)
- **Seção** = Prioridade MoSCoW (Must/Should/Could/Won't)

#### **Recomendações para IA**

**Ao classificar tarefas, a IA deve**:
1. ✅ **Começar pelas tarefas mais simples** dentro de cada categoria de prioridade
2. ✅ **Considerar dependências** antes de marcar como "Bloqueada"
3. ✅ **Atualizar status** proativamente conforme progresso
4. ✅ **Usar MoSCoW** para definir escopo de sprints/releases
5. ✅ **Aplicar RICE/Eisenhower** quando houver 10+ tarefas para priorizar
6. ✅ **Equilibrar complexidade**: Não acumular apenas tarefas complexas no backlog
7. ✅ **Ser consistente**: Manter mesmo padrão de classificação ao longo do projeto

**Exemplo de decisão da IA**:
```
Cenário: 15 tarefas no backlog, todas "MUST HAVE"

Decisão da IA:
1. Filtrar por complexidade → Identificar 5 simples, 7 médias, 3 complexas
2. Ordenar por dependências → 2 tarefas estão bloqueadas
3. Calcular RICE score → Priorizar as 3 com maior impacto/esforço
4. Sugerir ordem: Começar pelas 3 simples + 2 médias independentes
5. Deixar as 3 complexas para depois (quando time estiver aquecido)
```

**Quando usar cada framework**:
- **Apenas Status + Complexidade**: Projetos pequenos (< 20 tarefas)
- **+ MoSCoW**: Projetos médios, definir escopo de releases
- **+ RICE**: Quando há múltiplas features competindo por recursos limitados
- **+ Eisenhower**: Quando há pressão de tempo e muitas "urgências" falsas
- **Matriz de Decisão (Etapa 2.5 do Simplicidade 2/3)**: Quando escolha entre tarefas não é óbvia

---

### 🤖 **Recomendações de Tarefas pela IA (OPCIONAL)**

**Quando Usar**:
- ✅ Após completar implementações ou sprints
- ✅ Quando o projeto está evoluindo e pode se beneficiar de novas funcionalidades
- ✅ Para identificar oportunidades de melhoria e refinamento de requisitos
- ❌ NÃO usar em projetos descartáveis ou protótipos temporários

**Pergunta Inicial ao Usuário** (fazer UMA VEZ no início do projeto):
```
❓ Gostaria que a IA recomende novas tarefas dinamicamente no TASKS.md 
   conforme o projeto evolui?
   
Opções:
A) ✅ Sim, adicionar recomendações de vez em quando
B) ❌ Não, manter apenas tarefas que eu definir manualmente
C) 🔢 Sim, mas com limite máximo de [X] novas tarefas (default: 30)
```

**Se o usuário aceitar (opção A ou C)**:

#### **Dinâmica de Recomendação (Curva Quadrática)**

A IA deve seguir um padrão de recomendação que **cresce, atinge um pico e depois diminui**:

```
Tarefas Recomendadas pela IA ao Longo do Projeto:

Início do Projeto (0-20% completo):
├── 🟢 FASE 1: CRESCIMENTO INICIAL (0-5 tarefas)
│   ├── Recomendações: Poucas e essenciais
│   ├── Foco: Estabelecer base sólida do projeto
│   └── Exemplos: Setup CI/CD, estrutura de testes, documentação básica

Early Development (20-40% completo):
├── 🟢 FASE 2: ACELERAÇÃO (5-15 tarefas)
│   ├── Recomendações: Aumentando gradualmente
│   ├── Foco: Features principais, integrações importantes
│   └── Exemplos: APIs essenciais, funcionalidades core, UX melhorias

Mid Development (40-70% completo):
├── 🟡 FASE 3: PICO MÁXIMO (15-30 tarefas total)
│   ├── Recomendações: Máximo de ideias e oportunidades
│   ├── Foco: Polimento, features secundárias, otimizações
│   └── Exemplos: Performance tuning, acessibilidade, i18n, analytics

Late Development (70-90% completo):
├── 🟠 FASE 4: DESACELERAÇÃO (10-15 tarefas restantes)
│   ├── Recomendações: Diminuindo, apenas críticas
│   ├── Foco: Finalização, bugfixes, estabilidade
│   └── Exemplos: Edge cases, testes de integração, documentação final

Final Stage (90-100% completo):
└── 🔴 FASE 5: EXAUSTÃO (0-5 tarefas finais)
    ├── Recomendações: PARAR de adicionar novas features
    ├── Foco: Release readiness, última revisão
    └── Exemplos: Apenas ajustes críticos ou bugfixes bloqueantes
```

**Fórmula da Curva** (para implementadores da IA):
```
num_tarefas_recomendadas = -4 * (progresso - 0.5)² + 30
onde:
- progresso = percentual completo (0.0 a 1.0)
- num_tarefas_recomendadas = total acumulado de tarefas recomendadas
- Pico máximo em ~50% do projeto (30 tarefas se default não alterado)
```

#### **Limites e Controles**

**Limite Máximo Configurável**:
- 📊 **Default**: 30 novas tarefas/ideias recomendadas pela IA
- ⚙️ **Configurável**: Usuário pode especificar outro valor (ex: 10, 50, 100)
- 🔢 **Pergunta**: "Qual o máximo de tarefas que a IA pode recomendar? (default: 30)"

**Controle de Escopo**:
```markdown
### ✅ CRITÉRIOS para Recomendações da IA

1. **Dentro do Escopo**:
   - ✅ Alinhado com o tema/propósito do projeto
   - ✅ Baseado em feedback de usuários (real ou simulado)
   - ✅ Melhoria de requisitos existentes
   - ✅ Profissionalismo e qualidade do produto

2. **FORA do Escopo** (NÃO recomendar):
   - ❌ Features não relacionadas ao tema principal
   - ❌ Ideias "legais mas desnecessárias" (feature creep)
   - ❌ Tecnologias/frameworks não justificados
   - ❌ Recomendações genéricas sem contexto do projeto

3. **Priorização**:
   - 🔴 MUST HAVE: Crítico para o projeto
   - 🟡 SHOULD HAVE: Importante mas não bloqueante
   - 🟢 COULD HAVE: Nice to have, baixa prioridade
   - ⚪ WON'T HAVE: Explicitamente fora do escopo
```

#### **Formato das Recomendações no TASKS.md**

```markdown
## 🤖 Tarefas Recomendadas pela IA

_Estas tarefas foram sugeridas pela IA com base no progresso do projeto e 
feedback de usuários. Revisar e aprovar antes de implementar._

### 🔴 MUST HAVE (Críticas)
- 🔴🔴 [ ] **[IA-001]** Implementar autenticação de 2 fatores
  - **Status**: 🔴 Not Started
  - **Complexidade**: 🔴 Complexa (8-12h)
  - **Razão**: Segurança crítica para dados de usuários
  - **Impacto**: Alto (requisito de compliance LGPD)
  - **Prioridade MoSCoW**: Must Have

### 🟡 SHOULD HAVE (Importantes)
- 🔴🟡 [ ] **[IA-002]** Adicionar dashboard de analytics
  - **Status**: 🔴 Not Started
  - **Complexidade**: 🟡 Média (4-6h)
  - **Razão**: Stakeholders solicitaram métricas de uso
  - **Impacto**: Médio (melhora tomada de decisão)
  - **Prioridade MoSCoW**: Should Have

### 🟢 COULD HAVE (Melhorias)
- 🔴🟢 [ ] **[IA-003]** Dark mode no tema da aplicação
  - **Status**: 🔴 Not Started
  - **Complexidade**: 🟢 Simples (2-3h)
  - **Razão**: Pedido frequente de usuários finais
  - **Impacto**: Baixo (UX enhancement)
  - **Prioridade MoSCoW**: Could Have

---
**📊 Estatísticas de Recomendações da IA**:
- Total recomendadas: 3/30 (10% do limite)
- Fase atual: FASE 2 - ACELERAÇÃO (progresso: 35%)
- Próxima revisão: Após próxima sprint
```

#### **Frequência de Adição**

**Quando a IA deve adicionar novas tarefas**:
- ✅ **Após cada sprint/milestone** completada
- ✅ **Quando progresso atinge marcos**: 25%, 50%, 75%
- ✅ **Quando usuário solicita** explicitamente: "Sugira novas tarefas"
- ❌ **NUNCA** adicionar tarefas no meio de uma implementação ativa

**Aprovação do Usuário**:
```
❓ Após cada sprint, perguntar:
"Deseja revisar [X] novas tarefas recomendadas pela IA para o TASKS.md?"

A) ✅ Sim, adicionar ao TASKS.md para revisão
B) 📋 Sim, mas mostrar preview antes de adicionar
C) ⏭️ Pular por agora (não adicionar nesta sprint)
D) 🛑 Parar recomendações (desabilitar permanentemente)
```

#### **Exemplo Completo com Sistema de Classificação**

```markdown
# TASKS.md

## 📊 Legenda de Classificação

### Status
- 🔴 **Not Started** - Aguardando início
- 🟡 **In Progress** - Em desenvolvimento
- 🟢 **Done** - Concluído e testado
- 🔵 **Blocked** - Bloqueado por dependência

### Complexidade
- 🟢 **Simples** (0-1h) - Baixo risco, poucas dependências
- 🟡 **Média** (1-2h) - Risco médio, algumas integrações
- 🔴 **Complexa** (>2h) - Alto risco, muitas dependências

### Priorização MoSCoW
- 🔴 **Must Have** - Crítico, bloqueante
- 🟡 **Should Have** - Importante, não bloqueante
- 🟢 **Could Have** - Desejável, baixa prioridade
- ⚪ **Won't Have** - Fora do escopo atual

## 📊 Estatísticas do Projeto
- **Progresso Geral**: 45% completo (18/40 tarefas)
- **Fase Atual**: FASE 3 - PICO MÁXIMO
- **Tarefas IA**: 12/30 recomendadas (40% do limite)

## ✅ Tarefas Concluídas (18)
- 🟢🟢 [x] Setup inicial do projeto (Done, Simples)
- 🟢🟡 [x] Implementar autenticação básica (Done, Média)
- 🟢🟡 [x] CRUD de usuários (Done, Média)
... (15 mais)

## 🔨 Tarefas Pendentes Originais (22)

### 🔴 MUST HAVE
- 🔴🔴 [ ] Integração com API de pagamento (Not Started, Complexa, 5h)
- 🟡🟡 [ ] Sistema de notificações (In Progress, Média, 2h, 40% completo)
- 🔵🟢 [ ] Deploy em produção (Blocked, Simples, 1h, aguardando aprovação)

### 🟡 SHOULD HAVE
- 🔴🟢 [ ] Adicionar tooltips de ajuda (Not Started, Simples, 0.5h)
... (12 mais)

### 🟢 COULD HAVE
- 🔴🟡 [ ] Tema customizável (Not Started, Média, 2h)
... (7 mais)

## 🤖 Tarefas Recomendadas pela IA (12/30 usadas)

### 🔴 MUST HAVE
- 🔴🟡 [ ] **[IA-001]** Rate limiting em endpoints da API
  - **Status**: 🔴 Not Started
  - **Complexidade**: 🟡 Média (3-4h)
  - **Razão**: Prevenir abuso e garantir estabilidade
  - **Impacto**: Alto (segurança e performance)
  - **MoSCoW**: Must Have
  
- 🔴🟢 [ ] **[IA-002]** Logging estruturado para debugging
  - **Status**: 🔴 Not Started
  - **Complexidade**: 🟢 Simples (2-3h)
  - **Razão**: Facilitar troubleshooting em produção
  - **Impacto**: Alto (operacional)
  - **MoSCoW**: Must Have

### 🟡 SHOULD HAVE
- 🔴🟢 [ ] **[IA-003]** Exportar dados em formato CSV
  - **Status**: 🔴 Not Started
  - **Complexidade**: 🟢 Simples (2h)
  - **Razão**: Solicitação de stakeholders para análise
  - **Impacto**: Médio (conveniência)
  - **MoSCoW**: Should Have

... (9 tarefas mais)

---
**🎯 Próxima Revisão de Recomendações**: Após Sprint 8 (quando atingir 60% progresso)
```

#### **Desabilitando Recomendações**

Se o usuário quiser **parar** as recomendações:

```markdown
## 🤖 Recomendações da IA: DESABILITADAS

_O usuário optou por gerenciar tarefas manualmente._

**Para reativar**: Solicitar à IA "Reativar recomendações de tarefas"
```

---

**Por quê esta funcionalidade é valiosa?**:
- ✅ **Criatividade IA**: Identifica oportunidades que desenvolvedores podem não ver
- ✅ **Profissionalismo**: Sugere boas práticas e padrões de qualidade
- ✅ **Refinamento**: Colabora com requisitos para atender expectativas do cliente
- ✅ **Controle**: Usuário tem controle total (limite, aprovação, desabilitar)
- ✅ **Foco**: Curva de crescimento/decrescimento evita feature creep
- ✅ **Escopo**: Recomendações baseadas no contexto e feedback do projeto

**📁 Localização do Arquivo TASKS.md**:
- **Preferência padrão**: O arquivo `TASKS.md`, quando produzido, deve ser colocado em `docs/TASKS.md`
- **Criar pasta docs/**: Se a pasta `docs/` não existe no projeto, ela deve ser criada automaticamente
- **Flexibilidade**: O usuário ou programador pode optar por colocar em outro local se preferir
- **Exemplo de criação**:
  ```bash
  # Criar pasta docs se não existir
  mkdir -p docs
  
  # Criar ou atualizar TASKS.md
  echo "# Tasks" > docs/TASKS.md
  ```

**Exemplo de Marcação (REQUIREMENTS.md)**:
```markdown
## 🟢 COULD HAVE (Prioridade Baixa)

### ✅ Tasks Concluídas

#### Task Example - Editor de Arquivos Integrado (vX.Y.Z)
**Status**: ✅ Completa - 30/11/2025

**Objetivo**: Implementar editor de texto integrado com diferenciação de escopo por cores.

**Implementação**:
1. ✅ ComponentE com QTextEdit e syntax highlighting
2. ✅ Diferenciação de escopo por cores (HTML tags, DATA keys, etc.)
3. ✅ Abrir/salvar arquivos (.txt, .data, .html, .tsx, .py)
4. ✅ Integração com menu File → Open Editor

**Arquivos Criados**:
- `src/gui/editor_dock.py` (500+ linhas)
- `tests/test_editor_dock.py` (15 testes)

### 🔨 Tasks Pendentes
- **[]** Próxima task não implementada...
```

**Estrutura Mínima Recomendada**:
```markdown
# Projeto - Tasks

## Categorias
- MUST HAVE: [X/Y completas] (Z%)
- SHOULD HAVE: [X/Y completas] (Z%)
- COULD HAVE: [X/Y completas] (Z%)
- WOULD HAVE: [X/Y completas] (Z%)

## Estatísticas
- **TOTAL**: [X/Y completas] (Z%)
```

**Estrutura da Documentação de Versão**:
```markdown
# MyProject v2.9.X - [Nome Descritivo]

**Data**: DD/MM/AAAA
**Sprint**: X tasks em Y horas
**Metodologia**: Protocolo Simplicidade 1

## 📋 Objetivos da Sprint
- Task #X: [descrição]
- Task #Y: [descrição]

## 🎯 Tasks Implementadas
### Task #X: [Nome]
- **Problema**: [descrição do problema original]
- **Solução**: [como foi resolvido]
- **Arquivos Modificados**: [lista]
- **Testes**: [quantidade e status]

## ✅ Qualidade (Protocolo Simplicidade 1)
- ✅ Arquitetura Modular
- ✅ Type Hints (100%)
- ✅ Docstrings completas
- ✅ Tratamento de erros
- ✅ Testes (X passing)
- ✅ Commits semânticos
- ✅ Documentação completa
- ✅ Código limpo (PEP8)

## 📊 Estatísticas
- TOTAL: X% completo (Y/Z tasks)
- Commits: N pushed
```

---

### 1️⃣3️⃣ **Fazer Commit e Push**
- **Formato**: Conventional Commits (OBRIGATÓRIO)
- **Idioma**: Todas as mensagens de commit devem ser **EXCLUSIVAMENTE EM INGLÊS** (requisito obrigatório)
- **Mensagem**: Descritiva, completa, com contexto
- **Frequência**: 1 commit por task ou grupo lógico de mudanças

**Tipos de Commit Padronizados** (OBRIGATÓRIOS):
- `feat`: Indica uma nova feature
  - Exemplo: `git commit -m "feat: add Header component"`
- `fix`: Indica uma correção de bug
  - Exemplo: `git commit -m "fix: remove wrong prop in Header"`
- `refactor`: Indica uma refatoração de código
  - Exemplo: `git commit -m "refactor: add title in Header"`
- `test`: Indica alterações em testes
  - Exemplo: `git commit -m "test: add test in title Header"`
- `style`: Indica alterações de estilo/formatação
  - Exemplo: `git commit -m "style: add Header title background"`
- `docs`: Indica alteração na documentação
  - Exemplo: `git commit -m "docs: add get started in readme"`
- `chore`: Indica alteração de ambiente de desenvolvimento
  - Exemplo: `git commit -m "chore: change eslint rules"`
- `build`: Indica alteração de dependências
  - Exemplo: `git commit -m "build: add sass"`
- `revert`: Indica reversão de commit anterior
  - Exemplo: `git commit -m "revert: back to adc1234 commit"`

⚠️ **IMPORTANTE**: Todas as mensagens de commit devem ser escritas **EXCLUSIVAMENTE EM INGLÊS**!

**Estrutura de Commit Message**:
```
<tipo>: <descrição curta> (<versão>)

<PROBLEMA ORIGINAL>:
- [Contexto do problema]
- [Por que era necessário resolver]

<SOLUÇÃO IMPLEMENTADA>:
✅ [Feature/função 1]
   - [Detalhe técnico]
✅ [Feature/função 2]
   - [Detalhe técnico]

✅ [TESTES]:
   - [Quantidade] unit tests ([status])
   - [Categorias testadas]

<ARQUIVOS MODIFICADOS>:
- [arquivo1.py] (+X linhas)
- [arquivo2.py] (~Y linhas)
- [tests/test_X.py] (NOVO - Z linhas)
- [docs/REQUIREMENTS.md] (estatísticas atualizadas)

<ESTATÍSTICAS ATUALIZADAS>:
- [CATEGORIA]: X → Y completas (A% → B%)
- TOTAL: X → Y completas (A% → B%)

<EXEMPLO DE USO>: (se aplicável)
  [Demonstração prática]

Refs: [documentação relacionada]
Closes: Task #X (vX.X.X)
```

**Exemplo Real** (Task Example):
```bash
git add src/ tests/ docs/REQUIREMENTS.md
git commit -m "feat: completar Task Example - Feature Update System (vX.Y.Z)

PROBLEMA ORIGINAL:
- Implementação vX.Y.Z usava string_similarity() (ERRADO)
- Não detectava valores duplicados, apenas similaridade de nomes
...

✅ SOLUÇÃO IMPLEMENTADA:
✅ extract_all_keys_from_obj()
   - Suporta tipo Obj E dict
   - Retorna Dict[str, str] (path → value)
...

Closes: Task Example (vX.Y.Z)"

git push
```

---

## 🏆 Critérios de Qualidade Profissional

Toda implementação deve cumprir **100% destes critérios**:

| # | Critério | Descrição | Validação |
|---|----------|-----------|-----------|
| 1 | **Arquitetura Modular** | Cada feature em módulo separado | Arquivo próprio em `src/` |
| 2 | **Type Hints** | 100% dos parâmetros tipados | `def func(x: int) -> str:` |
| 3 | **Docstrings** | Todas funções públicas documentadas | Args, Returns, Examples |
| 4 | **Tratamento de Erros** | Try/except com mensagens claras | `except Exception as e:` |
| 5 | **Testes** | Unitários + integração (100% coverage) | `tests/test_*.py` passing |
| 6 | **Commits Semânticos** | Conventional Commits | `feat:`, `fix:`, `docs:` |
| 7 | **Documentação** | REQUIREMENTS.md + SPECIFICATIONS.md | Atualizado e completo |
| 8 | **Código Limpo** | PEP8, nomes semânticos, DRY | Funções < 50 linhas |

---

## 📊 Aplicação Prática: Task Example (Exemplo Completo)

### Situação Inicial
```markdown
Tasks pendentes na categoria SHOULD HAVE:
[ ] Complex Feature Example (MUITO COMPLEXO)
[ ] Busca com IA semântica (MUITO COMPLEXO)
[⚠️] Feature Update (PARCIAL - mais simples!) ✅ ESCOLHIDA
[ ] Google Translate API integration (COMPLEXO)
```

### Sprint Planejada
```
vX.Y.Z: Completar Task Example
Estimativa: 3-4 horas
Complexidade: MÉDIA (mais simples que as outras)
```

### Execução (Protocolo Simplicidade 1)

**1. Ler Documentação** ✅
- Lido: `docs/FEATURE_SPEC.md` (662 linhas)
- Entendido: problema de string similarity vs. value equality

**2. Escolher Tarefa Simples** ✅
- Task Example é **mais simples** que editor de texto ou IA
- Escopo claro: 2 funções principais + integração

**3. Fazer Perguntas** ✅
- Perguntado: "Quantas palavras pegar? 3-5?"
- Resposta: "Default 30 caracteres"
- Perguntado: "Converter para camelCase?"
- Resposta: "Sim, remover acentos"
- Perguntado: "Conflitos de nomes?"
- Resposta: "Linha menor vence, não mexer se valores diferentes"

**4. Sprint** ✅
- 6 subtasks planejadas (incluindo perguntas)
- Tempo estimado: 3h45min

**5. Implementar com Arquitetura** ✅
```
Ordem executada:
1. extract_all_keys_from_obj() (função auxiliar - Alta Coesão)
2. build_substitution_map_by_value() (função principal - Baixo Acoplamento)
3. Atualizar cli_dedupe() (integração - Injeção de Dependência)
4. Criar testes (validação)
5. Documentação (finalização)

Padrões Aplicados:
- ✅ Módulos separados (Reutilização)
- ✅ Type hints em todas funções
- ✅ Information Expert (GRASP): cada função tem a info que precisa
- ✅ Baixo acoplamento: funções independentes
- ✅ Alta coesão: cada função faz UMA coisa
```

**6. Fazer Testes** ✅
```
12 unit tests criados:
- 4 testes para extract_all_keys_from_obj()
- 5 testes para build_substitution_map_by_value()
- 2 testes para apply_substitutions_to_file()
- 1 teste para update_references_in_project()
Resultado: 12/12 passing (100%)
```

**7. Documentação** ✅
```
Arquivos criados/atualizados:
- docs/REQUIREMENTS.md (Task Example marcada [X])
- docs/FEATURE_SPEC.md (já existia)
- tests/test_reference_updater.py (NOVO - 350 linhas)
Estatísticas: 59.6% → 60.6% (63 tasks completas)
```

**8. Commit e Push** ✅
```bash
Commit: 903bca4
Mensagem: 60 linhas (completa e detalhada)
Status: pushed para GitHub ✅
```

### Resultado Final
✅ **Task Example 100% completa**  
✅ **Protocolo Simplicidade 1: 10/10 etapas cumpridas** (v1.1 - 10 etapas)  
✅ **Tempo real: ~3h (dentro da estimativa)**  
✅ **Zero bugs detectados**  
✅ **Documentação profissional**

**Nota**: Este exemplo usa v1.1 do protocolo (10 etapas). A v1.2 adiciona mais 2 etapas (integração GUI e CLI).

---

## 🎓 Lições Aprendidas

### ✅ O Que Funciona
1. **Escolher o mais simples**: Task Example era mais fácil que editor de texto
2. **Incrementalidade**: Função auxiliar → principal → integração
3. **Testes primeiro**: Detectou 2 ajustes necessários antes de commitar
4. **Documentação completa**: Facilita manutenção futura

### ❌ Anti-padrões a Evitar
1. **Não começar pela tarefa mais difícil**
   - ❌ "Vou fazer o editor de texto primeiro (50h)"
   - ✅ "Vou fazer o tooltip preview primeiro (30min)"

2. **Não fazer tudo de uma vez**
   - ❌ "Vou implementar tudo em uma função gigante"
   - ✅ "Vou dividir em 3 funções testáveis"

3. **Não pular testes**
   - ❌ "Vou testar manualmente depois"
   - ✅ "Vou criar 12 unit tests agora"

4. **Não fazer commits genéricos**
   - ❌ `git commit -m "updates"`
   - ✅ `git commit -m "feat: Task Example com VALUE EQUALITY (60 linhas)"`

---

## 📚 Referências

- **REQUIREMENTS.md**: Lista completa de tarefas do projeto
- **vX.Y.Z-COMPARISON.md**: Primeiro exemplo do protocolo
- **vX.Y.Z-SPECIFICATIONS.md**: Sprint com 3 tasks simples
- **vX.Y.Z-SPECIFICATIONS.md**: Iterações rápidas
- **vX.Y.Z-SPECIFICATIONS.md**: 4 melhorias de UX
- **FEATURE_SPEC.md**: Exemplo de documentação detalhada

---

## 🔄 Ciclo Contínuo

O Protocolo Simplicidade 1 é um **ciclo iterativo**:

```
┌──────────────────────────────────────────────┐
│  1. Ler Documentação                         │
│  2. Escolher Tarefas Mais Simples            │
│  3. Fazer Perguntas ao Programador           │
│  4. Analisar e Estudar o Projeto             │
│  5. Planejar Sprint (2-4 tasks, 3-4h)        │
│  6. Implementar (arquitetura GoF + GRASP)    │
│  7. Verificar Integração GUI                 │
│  8. Verificar Implementação CLI              │
│  9. Testar (100% coverage)                   │
│  10. Organizar Pasta Raiz                    │
│  11. Documentar (TASKS + vX.X.X-SPECS)       │
│  12. Commit + Push (conventional)            │
└──────────────────────────────────────────────┘
           ↓
    ┌──────────────┐
    │   REPETIR    │ ← Sempre há tarefas mais simples!
    └──────────────┘
```

**Resultado**: Progresso constante, código profissional, zero dívida técnica.

---

## 🎯 Mensagem Final

> "Quero um trabalho completo e profissional!"

**Este protocolo garante**:
- ✅ Qualidade profissional (12 etapas obrigatórias)
- ✅ Progresso incremental (do simples ao complexo)
- ✅ Documentação completa (nunca esquecer o que foi feito)
- ✅ Código testado (100% confiável)
- ✅ Integração verificada (GUI + CLI funcionais)
- ✅ Commits organizados (histórico limpo)

**Releia este documento antes de cada sprint!**

---

## 📊 Organização Ordinal de Tarefas - Protocolos Simplicidade

**Versão**: 1.0  
**Data de Criação**: 27 de Dezembro de 2025  
**Autor**: Josué Amaral  
**Status**: ATIVO

---

### 🎯 Objetivo

Este documento define o sistema de **Organização Ordinal de Tarefas** para os Protocolos Simplicidade, permitindo que desenvolvedores humanos e inteligências artificiais identifiquem rapidamente:

- ✅ **Ordem de execução** das tarefas (do mais simples ao mais complexo)
- ✅ **Dependências** entre tarefas (quais devem ser feitas primeiro)
- ✅ **Paralelização** (quais podem ser executadas simultaneamente)
- ✅ **Organização hierárquica** (estrutura de árvore/grafo)

---

### 📊 Sistema de Prefixos Ordinais

#### Nível 1: Numeração Simples (Tarefas Independentes)

Para tarefas **independentes** que **não têm dependências** entre si:

```markdown
1. Tarefa A - Configurar ambiente de desenvolvimento
2. Tarefa B - Criar documentação inicial
3. Tarefa C - Definir arquitetura do sistema
```

**Características**:
- ✅ Podem ser executadas em **qualquer ordem**
- ✅ Podem ser feitas **paralelamente** em branches separadas
- ✅ Sem conflitos de dependência
- ✅ Numeração sequencial crescente (1, 2, 3...)

---

#### Nível 2: Hierarquia com Letras (Grupos de Tarefas)

Para organizar tarefas em **grupos lógicos** com **subgrupos**:

```markdown
🔴 MUST HAVE - Release v1.0.0

A. Infrastructure e Configuração
   A.1. Criar estrutura de diretórios
   A.2. Configurar dependências do projeto
   
B. Core - Estruturas de Dados
   B.1. Implementar classe Node
   B.2. Implementar ExpressionTree
   
C. Core - Conversões
   C.1. Implementar conversão número → árvore
   C.2. Implementar conversão árvore → RPN
```

**Características**:
- ✅ **Letra maiúscula** = Grupo/Categoria
- ✅ **Número após letra** = Subtarefa dentro do grupo
- ✅ Tarefas de **grupos diferentes** (A, B, C) são **paralelas**
- ✅ Tarefas do **mesmo grupo** podem ter dependências

---

#### Nível 3: Hierarquia Profunda (Dependências Complexas)

Para tarefas com **dependências explícitas** em estrutura de **árvore/grafo**:

```markdown
A.C.1. Implementar conversão número → árvore
   ├─ Deve ser feito DEPOIS de A.1, A.2, C.1
   └─ Estrutura: A (raiz) → C (intermediário) → 1 (folha)

B.C.2. Implementar conversão árvore → RPN
   B.C.2.1. Parser RPN (folha - fazer PRIMEIRO)
   B.C.2.2. Serializer RPN (folha - fazer PRIMEIRO)
   B.C.2. Implementar conversão (pai - fazer DEPOIS de 2.1 e 2.2)
```

**Leitura da hierarquia** (⭐ CRÍTICO):

A hierarquia deve ser lida da **DIREITA para ESQUERDA** (ordem inversa):

```
C.B.1.D.1
   │  │ │ └─ 1: Executar por ÚLTIMO (raiz da árvore)
   │  │ └─── D: Executar TERCEIRO
   │  └───── 1: Executar SEGUNDO
   └──────── B: Executar PRIMEIRO (folha da árvore)

Ordem de execução: B → 1 → D → 1 (da direita para esquerda)
```

**Interpretação**:
- ✅ **Mais à DIREITA** = Ancestrais (executar por ÚLTIMO)
- ✅ **Mais à ESQUERDA** = Descendentes (executar PRIMEIRO)
- ✅ **Organização bottom-up**: Base → Topo

**Exemplo Prático**:

```markdown
C.B.1.D.1 - Integrar Dash com Cytoscape

Ordem de execução (direita → esquerda):
1. PRIMEIRO:  Tarefa D.1 (criar componente básico Cytoscape)
2. SEGUNDO:   Tarefa 1.D (configurar layout)
3. TERCEIRO:  Tarefa B.1 (implementar estrutura de dados)
4. QUARTO:    Tarefa C (integração final Dash + Cytoscape)
```

---

### 🌳 Estrutura de Árvore/Grafo

#### Conceitos Fundamentais

**1. Nós Pai e Filhos**

```
B.C.2 (PAI - executar DEPOIS)
   ├── B.C.2.1 (FILHO - executar ANTES)
   └── B.C.2.2 (FILHO - executar ANTES)
```

**Regra**: 
- ✅ **Filhos devem ser completados ANTES do pai**
- ✅ Filhos são **pré-requisitos** do pai
- ✅ Pai **depende** dos filhos

**2. Irmãos (Parallel)**

```
B.C.2.1 (irmão)
B.C.2.2 (irmão)
```

**Regra**:
- ✅ Irmãos podem ser executados **paralelamente**
- ✅ Sem dependência entre si
- ✅ Podem estar em **branches separadas**

**3. Primos, Tios, Avós (Parallel vs Serial)**

```
A. Grupo A
   A.1. Tarefa A1
   A.2. Tarefa A2
   
B. Grupo B
   B.1. Tarefa B1
   B.2. Tarefa B2
```

**Regra**:
- ✅ **Grupos diferentes** (A, B) = **PARALLEL** (executar simultaneamente)
- ✅ **Primos** (A.1 e B.1) = **PARALLEL**
- ✅ **Tios/Sobrinhos** (A e B.1) = **Avaliar dependências explícitas**

---

### 🔄 Paralelização vs Serialização

#### Tarefas PARALELAS (podem ser simultâneas)

✅ **Quando paralelizar**:
- Tarefas de **grupos diferentes** (A.x, B.x, C.x)
- **Irmãos** no mesmo nível (X.1, X.2, X.3)
- **Primos** (A.1 e B.1)
- Tarefas **sem dependências** explícitas

**Exemplo**:
```markdown
✅ PARALLEL:
   A.1 (Criar modelo User)
   B.1 (Criar modelo Product)
   C.1 (Criar interface gráfica)
   
→ Podem ser feitas em 3 branches simultâneas
→ Zero conflitos
```

---

#### Tarefas SERIAIS (devem ser sequenciais)

❌ **Quando serializar**:
- Tarefas com **relação pai-filho**
- Tarefas com **dependências explícitas**
- Quando uma tarefa **usa o resultado** de outra

**Exemplo**:
```markdown
❌ SERIAL:
   B.C.2.1 (Parser RPN) ─┐
   B.C.2.2 (Serializer)  ├─→ B.C.2 (Conversão completa)
                         ┘
   
→ B.C.2.1 e B.C.2.2 DEVEM ser completadas ANTES de B.C.2
→ B.C.2 depende dos resultados de 2.1 e 2.2
```

---

### 🎯 Integração com Sistema de Classificação Existente

O sistema ordinal **complementa** (não substitui) as classificações existentes:

```markdown
🔴🟡 [ ] #3 B.1. Implementar classe Node (1h)
 │  │  │  │ └─ Prefixo ordinal (dependências)
 │  │  │  └─── ID da issue (#3)
 │  │  └────── Hierarquia (B = Grupo, 1 = Subtarefa)
 │  └───────── Complexidade (🟡 Média)
 └──────────── Prioridade (🔴 Must Have)

Razão: Base para toda manipulação de árvores
Features: Binary tree node com operador/valor
Tests: Unit tests para criação de nós
```

**Legenda Completa**:
- **Prioridade MoSCoW**: 🔴 Must | 🟡 Should | 🟢 Could | ⚪ Won't
- **Complexidade**: 🟢 Simples (0-1h) | 🟡 Média (1-2h) | 🔴 Complexa (>2h)
- **Status**: 🔴 Not Started | 🟡 In Progress | 🟢 Done | 🔵 Blocked
- **Prefixo Ordinal**: Identifica ordem de execução e dependências

---

### 🤖 Instruções para Inteligências Artificiais

**Quando Sugerir Organização Ordinal**

A IA deve sugerir organização ordinal quando:

✅ **Projeto tem >10 tarefas** com interdependências
✅ **Múltiplos desenvolvedores** trabalhando simultaneamente
✅ **Tarefas bloqueantes** (uma depende de outra)
✅ **Risco de conflitos** no controle de versão
✅ **Necessidade de paralelização** para acelerar desenvolvimento

**Como a IA Deve Aplicar**

1. **Analisar dependências**:
   ```python
   # Pseudo-código
   tarefas = ler_tasks_md()
   grafo = construir_grafo_dependencias(tarefas)
   ordem = ordenacao_topologica(grafo)  # Bottom-up
   ```

2. **Identificar grupos paralelos**:
   ```python
   grupos_parallel = identificar_componentes_independentes(grafo)
   ```

3. **Atribuir prefixos ordinais**:
   ```python
   for grupo in grupos_parallel:
       letra = proxima_letra()  # A, B, C...
       for tarefa in grupo:
           tarefa.prefixo = f"{letra}.{tarefa.index}"
   ```

4. **Sugerir estratégia de branches**:
   ```markdown
   Recomendação de branches:
   - Branch feat/auth: A.1 → A.2 → A.3
   - Branch feat/api: B.1 → B.2 (parallel com auth)
   - Branch feat/ui: C.1 (aguardar merge de auth)
   ```

---

## 🌳 Analogia da Árvore de Importações

**Autor:** Josué Amaral  
**Data:** 24 de Dezembro de 2025  
**Contexto:** Phase 3.0 - Refactoring Architecture  
**Aplicável a:** Todas as linguagens de programação

---

### 📚 Visão Geral

Este documento descreve a **Analogia da Árvore de Importações**, um modelo mental para compreender e organizar a arquitetura de dependências em projetos de software. Esta analogia é aplicável a qualquer linguagem de programação que suporte importação/inclusão de módulos.

---

### 🌳 A Árvore de Importações

#### Conceito Fundamental

A estrutura de importações de um projeto pode ser visualizada como uma **árvore hierárquica**, onde:

```
                    📦 A (Raiz)
                   /           \
              📦 B              📦 C
             / | \               |
        📦 D 📦 E 📦 F         📦 G
         |    |    |            |
      [libs] [libs] [libs]   [libs]
```

#### Elementos da Árvore

**🌲 Raiz (Root)**
- **Arquivo Principal** (ex: `app.py`, `main.py`, `index.js`)
- **Características:**
  - Mais complexo e encapsulado
  - Orquestrador do sistema
  - Importa múltiplos módulos do projeto
  - Contém lógica de coordenação entre componentes
  - Decide "o quê" fazer, delegando "como" fazer

**🌿 Galhos (Branches)**
- **Módulos Intermediários** (ex: `gui/`, `core/`, `utils/`)
- **Características:**
  - Complexidade média
  - Importam outros módulos do projeto
  - Fornecem funcionalidade especializada
  - Abstraem detalhes de implementação

**🍃 Folhas (Leaves)**
- **Módulos Terminais** (ex: `button.py`, `validator.py`, `helpers.py`)
- **Características:**
  - Mais simples e específicos
  - **NÃO importam** arquivos do próprio projeto
  - **SIM importam** bibliotecas externas (Numpy, Pandas, etc.)
  - Fornecem funcionalidade atômica
  - São reutilizáveis e testáveis independentemente

---

### 📊 Exemplo Prático

#### Estrutura Hierárquica

```python
# A.py (RAIZ) - Arquivo principal
from B import feature_x
from C import feature_y

def main():
    """Orquestrador - coordena B e C"""
    result_x = feature_x.process()
    result_y = feature_y.process()
    combine(result_x, result_y)
```

```python
# B.py (GALHO) - Módulo intermediário
from D import validator
from E import transformer
from F import calculator

def feature_x():
    """Especialista - coordena D, E, F"""
    data = validator.validate_input()
    transformed = transformer.transform(data)
    return calculator.compute(transformed)
```

```python
# D.py (FOLHA) - Módulo terminal
import re  # Biblioteca padrão
import numpy as np  # Biblioteca externa

def validate_input(data):
    """Função atômica - não importa arquivos do projeto"""
    pattern = re.compile(r'^\d+$')
    return np.array([x for x in data if pattern.match(x)])
```

#### Características por Nível

| Nível | Arquivo | Importa Projeto | Importa Externo | Complexidade | Papel |
|-------|---------|-----------------|-----------------|--------------|-------|
| 0 (Raiz) | A | B, C | Raramente | Alta | Orquestrador |
| 1 (Galho) | B, C | D, E, F, G | Às vezes | Média | Coordenador |
| 2 (Folha) | D, E, F, G | ❌ Nunca | ✅ Sempre | Baixa | Executor |

---

### 🔄 Abordagens de Desenvolvimento

#### 🔽 Top-Down (De Cima para Baixo)

**Começa pela raiz e desce até as folhas**

```
Processo:
1. Definir A (o quê o sistema faz)
2. Identificar necessidades (B, C)
3. Decompor B em (D, E, F)
4. Implementar folhas (D, E, F, G)
```

**Vantagens:**
- ✅ Arquitetura clara desde o início
- ✅ Facilita planejamento de alto nível
- ✅ Identifica dependências cedo

**Desvantagens:**
- ❌ Pode criar interfaces sem implementação
- ❌ Dificulta testes iniciais
- ❌ Risco de over-engineering

---

#### 🔼 Bottom-Up (De Baixo para Cima)

**Começa pelas folhas e sobe até a raiz**

```
Processo:
1. Implementar D, E, F, G (componentes básicos)
2. Combinar em B, C (funcionalidades)
3. Orquestrar em A (sistema completo)
```

**Vantagens:**
- ✅ Componentes testáveis desde o início
- ✅ Reutilização natural
- ✅ Menos desperdício de código

**Desvantagens:**
- ❌ Arquitetura emerge tardiamente
- ❌ Risco de componentes não integráveis
- ❌ Dificuldade em visualizar o todo

---

#### ↔️ Middle-Out (Do Meio para Fora)

**Começa pelos galhos e expande em ambas direções**

```
Processo:
1. Identificar funcionalidade central (B)
2. ↓ Implementar componentes necessários (D, E, F)
3. ↑ Criar orquestrador (A)
4. Repetir para outras funcionalidades (C, G)
```

**Vantagens:**
- ✅ Balanceia visão geral e detalhes
- ✅ Iterativo e adaptável
- ✅ Reduz risco de ambas abordagens extremas

**Desvantagens:**
- ❌ Requer experiência para identificar "o meio"
- ❌ Pode criar inconsistências
- ❌ Exige refatorações frequentes

---

### 🎯 Princípios de Design

#### 1. **Princípio da Profundidade**

> "Quanto mais próximo da raiz, mais complexo e orquestrador.  
> Quanto mais próximo das folhas, mais simples e executor."

```
Raiz (A):     if condition: B.do() else: C.do()  ← Decisão
Galho (B):    return D.compute(E.prepare(data))  ← Coordenação
Folha (D):    return sum(numbers) / len(numbers) ← Execução
```

#### 2. **Princípio da Independência**

> "Folhas não dependem de outras folhas do projeto.  
> Folhas podem depender apenas de bibliotecas externas."

❌ **Errado:**
```python
# D.py (folha)
from E import helper  # Dependência entre folhas!
```

✅ **Correto:**
```python
# B.py (galho)
from D import function_d
from E import helper

def feature():
    return function_d(helper.prepare())  # Galho coordena folhas
```

#### 3. **Princípio da Responsabilidade Única**

> "Cada nível tem seu papel distinto."

| Nível | Responsabilidade | Pergunta que Responde |
|-------|------------------|----------------------|
| Raiz | Orquestração | "O que o sistema faz?" |
| Galho | Coordenação | "Como as partes se conectam?" |
| Folha | Execução | "Como fazer X especificamente?" |

---

### 📏 Métricas de Qualidade

#### Indicadores de Boa Arquitetura

✅ **Árvore Balanceada:**
- Profundidade 2-4 níveis
- Largura proporcional à complexidade
- Sem folhas que importam outras folhas

✅ **Separação Clara:**
```
Raiz:  Alta complexidade + Baixa execução
Folha: Baixa complexidade + Alta execução
```

✅ **Facilidade de Teste:**
- Folhas testáveis isoladamente
- Galhos testáveis com mocks
- Raiz testável com integração

#### Indicadores de Problemas

❌ **Árvore Degenerada (Linear):**
```
A → B → C → D → E → F  # Muito profundo!
```

❌ **Folhas Gordas:**
```python
# D.py - 500 linhas, importa E, F, G  # É galho, não folha!
```

❌ **Raiz Magra:**
```python
# A.py - 10 linhas  # Deveria orquestrar mais!
```

---

### 📖 Conclusão das Seções

A **Organização Ordinal de Tarefas** e a **Analogia da Árvore de Importações** fornecem modelos mentais poderosos para:

1. **Organizar** tarefas do mais simples ao mais complexo
2. **Compreender** arquitetura existente
3. **Planejar** novos módulos
4. **Refatorar** código organicamente
5. **Paralelizar** desenvolvimento para acelerar entregas
6. **Comunicar** decisões de design claramente

---

## 💡 Boas Práticas de Programação para IAs

> **Esta seção contém recomendações específicas para melhorar a qualidade do código gerado por inteligências artificiais.**

### 1. 📖 **Código Legível e Autodocumentado**

**Por quê importante**: IAs devem produzir código que humanos possam entender e manter facilmente.

**Práticas**:
- ✅ **Nomes descritivos**: Use nomes que explicam o propósito
  ```python
  # ❌ RUIM
  def proc(d, x):
      return d[x] if x in d else None
  
  # ✅ BOM
  def get_user_preference(preferences_dict, preference_key):
      """Retorna preferência do usuário ou None se não existir."""
      return preferences_dict.get(preference_key)
  ```

- ✅ **Funções pequenas e focadas**: Uma função = uma responsabilidade
  ```python
  # ❌ RUIM - Função faz múltiplas coisas
  def process_user_data(user):
      # valida
      # transforma
      # salva no banco
      # envia email
      # registra log
      pass  # 150 linhas
  
  # ✅ BOM - Funções especializadas
  def validate_user_data(user): pass
  def transform_user_data(user): pass
  def save_user_to_database(user): pass
  def send_welcome_email(user): pass
  def log_user_registration(user): pass
  ```

- ✅ **Evitar "números mágicos"**: Use constantes nomeadas
  ```python
  # ❌ RUIM
  if user.age > 18 and balance < 1000:
      apply_fee(balance * 0.05)
  
  # ✅ BOM
  MINIMUM_ADULT_AGE = 18
  BALANCE_THRESHOLD = 1000
  SERVICE_FEE_RATE = 0.05
  
  if user.age > MINIMUM_ADULT_AGE and balance < BALANCE_THRESHOLD:
      apply_fee(balance * SERVICE_FEE_RATE)
  ```

### 2. 🎯 **Convenções de Nomenclatura Consistentes**

**Por quê importante**: Consistência facilita navegação e compreensão do código.

**Práticas por linguagem**:

**Python**:
- ✅ `snake_case` para funções e variáveis
- ✅ `PascalCase` para classes
- ✅ `SCREAMING_SNAKE_CASE` para constantes
- ✅ `_private_method` para métodos privados

**JavaScript/TypeScript**:
- ✅ `camelCase` para funções e variáveis
- ✅ `PascalCase` para classes e componentes
- ✅ `SCREAMING_SNAKE_CASE` para constantes
- ✅ `_privateMethod` ou `#privateField` para privados

**Convenções gerais**:
- ✅ Verbos para funções: `get_user()`, `calculate_total()`, `validate_input()`
- ✅ Substantivos para classes: `UserManager`, `PaymentProcessor`
- ✅ Booleanos com prefixos: `is_valid`, `has_permission`, `can_edit`

### 3. 🛡️ **Tratamento de Erros Robusto**

**Por quê importante**: Código em produção deve lidar graciosamente com falhas.

**Práticas**:
- ✅ **Sempre validar entrada**:
  ```python
  def divide(a, b):
      if not isinstance(a, (int, float)) or not isinstance(b, (int, float)):
          raise TypeError("Argumentos devem ser números")
      if b == 0:
          raise ValueError("Divisor não pode ser zero")
      return a / b
  ```

- ✅ **Usar exceções específicas**:
  ```python
  # ❌ RUIM - Exceção genérica
  try:
      process_payment(amount)
  except Exception as e:
      print("Erro")
  
  # ✅ BOM - Exceções específicas
  try:
      process_payment(amount)
  except PaymentDeclinedError as e:
      notify_user("Pagamento recusado")
  except InsufficientFundsError as e:
      notify_user("Saldo insuficiente")
  except NetworkError as e:
      retry_payment(amount)
  ```

- ✅ **Logging adequado**:
  ```python
  import logging
  
  try:
      result = risky_operation()
  except Exception as e:
      logging.error(f"Falha em risky_operation: {e}", exc_info=True)
      raise  # Re-raise para permitir handling em nível superior
  ```

### 4. 🧪 **Estratégias de Teste Eficazes**

**Por quê importante**: Testes garantem que o código funciona e continua funcionando.

**Práticas**:
- ✅ **Testes unitários para lógica de negócio**:
  ```python
  def test_calculate_discount():
      # Arrange
      original_price = 100
      discount_rate = 0.2
      
      # Act
      final_price = calculate_discount(original_price, discount_rate)
      
      # Assert
      assert final_price == 80
  ```

- ✅ **Testar edge cases**:
  ```python
  def test_edge_cases():
      assert calculate_discount(0, 0.5) == 0  # Preço zero
      assert calculate_discount(100, 0) == 100  # Desconto zero
      assert calculate_discount(100, 1.0) == 0  # Desconto 100%
      
      with pytest.raises(ValueError):
          calculate_discount(100, -0.1)  # Desconto negativo
      
      with pytest.raises(ValueError):
          calculate_discount(-100, 0.1)  # Preço negativo
  ```

- ✅ **Mocks para dependências externas**:
  ```python
  from unittest.mock import Mock, patch
  
  def test_send_notification():
      with patch('email_service.send') as mock_send:
          notify_user("user@example.com", "Test message")
          mock_send.assert_called_once()
  ```

### 5. 🔒 **Segurança em Primeiro Lugar**

**Por quê importante**: Vulnerabilidades podem ter consequências graves.

**Práticas**:
- ✅ **Nunca confiar em input do usuário**:
  ```python
  # ❌ RUIM - SQL Injection
  query = f"SELECT * FROM users WHERE id = {user_id}"
  
  # ✅ BOM - Parametrização
  query = "SELECT * FROM users WHERE id = ?"
  cursor.execute(query, (user_id,))
  ```

- ✅ **Secrets em variáveis de ambiente**:
  ```python
  # ❌ RUIM
  API_KEY = "sk-1234567890abcdef"  # Hardcoded
  
  # ✅ BOM
  import os
  API_KEY = os.getenv('API_KEY')
  if not API_KEY:
      raise ValueError("API_KEY não configurada")
  ```

- ✅ **Sanitizar output para prevenir XSS**:
  ```python
  from html import escape
  
  # ❌ RUIM
  html = f"<div>Hello {user_name}</div>"
  
  # ✅ BOM
  html = f"<div>Hello {escape(user_name)}</div>"
  ```

### 6. ⚡ **Otimização de Performance**

**Por quê importante**: Código lento = usuários insatisfeitos.

**Práticas**:
- ✅ **Escolher estrutura de dados correta**:
  ```python
  # ❌ RUIM - Busca em lista O(n)
  if user_id in user_list:  # 1000 comparações
      # ...
  
  # ✅ BOM - Busca em set O(1)
  if user_id in user_set:  # 1 comparação
      # ...
  ```

- ✅ **Evitar loops desnecessários**:
  ```python
  # ❌ RUIM - Loop duplo O(n²)
  for item in list1:
      for item2 in list2:
          if item == item2:
              # ...
  
  # ✅ BOM - Set intersection O(n)
  common_items = set(list1) & set(list2)
  for item in common_items:
      # ...
  ```

- ✅ **Lazy loading quando apropriado**:
  ```python
  # ❌ RUIM - Carrega tudo na memória
  all_users = User.objects.all()  # 1 milhão de registros
  for user in all_users:
      process(user)
  
  # ✅ BOM - Iterator que carrega sob demanda
  for user in User.objects.iterator():
      process(user)
  ```

### 7. 📝 **Documentação Clara e Útil**

**Por quê importante**: Código é lido muito mais vezes do que é escrito.

**Práticas**:
- ✅ **Docstrings completos**:
  ```python
  def calculate_shipping(weight, distance, express=False):
      """
      Calcula o custo de envio baseado em peso e distância.
      
      Args:
          weight (float): Peso do pacote em kg
          distance (float): Distância em km
          express (bool): Se True, usa envio expresso (default: False)
      
      Returns:
          float: Custo de envio em reais
      
      Raises:
          ValueError: Se peso ou distância for negativo
      
      Examples:
          >>> calculate_shipping(2.5, 100)
          25.0
          >>> calculate_shipping(2.5, 100, express=True)
          37.5
      """
      if weight < 0 or distance < 0:
          raise ValueError("Peso e distância devem ser positivos")
      
      base_cost = weight * distance * 0.1
      return base_cost * 1.5 if express else base_cost
  ```

- ✅ **Comentários explicam "por quê", não "o quê"**:
  ```python
  # ❌ RUIM - Comenta o óbvio
  x = x + 1  # Incrementa x
  
  # ✅ BOM - Explica o motivo
  # Incrementa o contador para incluir o elemento atual na contagem
  # pois o range() exclui o último elemento
  x = x + 1
  ```

- ✅ **README com exemplos práticos**:
  ```markdown
  # Como usar
  
  ## Instalação
  ```bash
  pip install mypackage
  ```
  
  ## Exemplo básico
  ```python
  from mypackage import Calculator
  
  calc = Calculator()
  result = calc.add(2, 3)
  print(result)  # Output: 5
  ```
  ```

### 8. 🏗️ **Organização e Modularidade**

**Por quê importante**: Código organizado é mais fácil de manter e escalar.

**Práticas**:
- ✅ **Separação de responsabilidades**:
  ```
  project/
  ├── models/       # Estruturas de dados
  ├── services/     # Lógica de negócio
  ├── controllers/  # Coordenação de fluxo
  ├── views/        # Interface com usuário
  ├── utils/        # Funções auxiliares
  └── tests/        # Testes automatizados
  ```

- ✅ **DRY (Don't Repeat Yourself)**:
  ```python
  # ❌ RUIM - Código duplicado
  def process_order_a():
      validate()
      calculate()
      save()
  
  def process_order_b():
      validate()
      calculate()
      save()
  
  # ✅ BOM - Código reutilizado
  def process_order_common():
      validate()
      calculate()
      save()
  
  def process_order_a():
      process_order_common()
      # lógica específica A
  
  def process_order_b():
      process_order_common()
      # lógica específica B
  ```

- ✅ **Princípio da responsabilidade única**:
  ```python
  # ❌ RUIM - Classe faz muitas coisas
  class User:
      def __init__(self): pass
      def save_to_database(self): pass
      def send_email(self): pass
      def generate_pdf_report(self): pass
  
  # ✅ BOM - Classes especializadas
  class User:
      def __init__(self): pass
  
  class UserRepository:
      def save(self, user): pass
  
  class EmailService:
      def send(self, to, message): pass
  
  class ReportGenerator:
      def generate_pdf(self, user): pass
  ```

### 9. 🔄 **Controle de Versão Efetivo**

**Por quê importante**: Histórico limpo facilita debugging e colaboração.

**Práticas**:
- ✅ **Commits atômicos e descritivos**:
  ```bash
  # ❌ RUIM
  git commit -m "fixes"
  git commit -m "updates"
  
  # ✅ BOM
  git commit -m "feat: adiciona validação de email no formulário de cadastro"
  git commit -m "fix: corrige cálculo de desconto para valores acima de R$ 1000"
  ```

- ✅ **Branches para features**:
  ```bash
  # Criar branch para nova funcionalidade
  git checkout -b feature/user-authentication
  
  # Desenvolver e commitar
  git commit -m "feat: implementa login com JWT"
  
  # Merge após review
  git checkout main
  git merge feature/user-authentication
  ```

- ✅ **.gitignore apropriado**:
  ```gitignore
  # Python
  __pycache__/
  *.pyc
  .env
  venv/
  
  # JavaScript
  node_modules/
  dist/
  .env.local
  
  # IDEs
  .vscode/
  .idea/
  *.swp
  
  # OS
  .DS_Store
  Thumbs.db
  ```

### 10. 📦 **Gerenciamento de Dependências**

**Por quê importante**: Dependências mal gerenciadas causam problemas de compatibilidade.

**Práticas**:
- ✅ **Fixar versões**:
  ```
  # ❌ RUIM - requirements.txt
  flask
  requests
  
  # ✅ BOM - requirements.txt
  flask==2.3.2
  requests==2.31.0
  ```

- ✅ **Usar ambientes virtuais**:
  ```bash
  # Python
  python -m venv venv
  source venv/bin/activate
  pip install -r requirements.txt
  
  # Node.js
  npm install  # Usa package-lock.json
  ```

- ✅ **Verificar vulnerabilidades**:
  ```bash
  # Python
  pip install pip-audit
  pip-audit
  
  # Node.js
  npm audit
  npm audit fix
  ```

### 11. 🔄 **Refatoração Frequente de Código**

**Por quê importante**: Código que não é refatorado regularmente tende a se deteriorar com o tempo, tornando-se difícil de manter, entender e evoluir.

> **CRÍTICO PARA IAs**: Lembre-se **frequentemente** de refatorar o código durante o desenvolvimento para manter a qualidade e evitar acúmulo de dívida técnica.

**Práticas obrigatórias**:

- ✅ **Evitar arquivos excessivamente grandes**:
  ```
  # 🚨 ALERTAS DE TAMANHO
  - Arquivo > 500 linhas → Considere dividir
  - Arquivo > 1000 linhas → DEVE dividir
  - Classe > 300 linhas → Refatore em classes menores
  - Função > 50 linhas → Divida em funções auxiliares
  ```
  
  **Exemplo de refatoração**:
  ```python
  # ❌ RUIM - Arquivo com 1500 linhas
  # user_manager.py (tudo em um arquivo)
  class UserManager:
      def create_user(): pass  # 100 linhas
      def validate_user(): pass  # 150 linhas
      def authenticate_user(): pass  # 200 linhas
      def send_email(): pass  # 100 linhas
      # ... mais 950 linhas
  
  # ✅ BOM - Dividido em módulos especializados
  # user/
  #   __init__.py
  #   manager.py (200 linhas)
  #   validator.py (150 linhas)
  #   authenticator.py (200 linhas)
  #   notifications.py (100 linhas)
  ```

- ✅ **Aumentar coesão (Single Responsibility Principle)**:
  ```python
  # ❌ RUIM - Baixa coesão (faz muitas coisas diferentes)
  class OrderProcessor:
      def process_order(self):
          self.validate_payment()
          self.send_email()
          self.update_inventory()
          self.generate_invoice()
          self.log_analytics()
  
  # ✅ BOM - Alta coesão (cada classe tem uma responsabilidade)
  class PaymentValidator:
      def validate(self): pass
  
  class EmailNotifier:
      def send_order_confirmation(self): pass
  
  class InventoryManager:
      def update_stock(self): pass
  
  class InvoiceGenerator:
      def generate(self): pass
  
  class AnalyticsLogger:
      def log_order(self): pass
  ```

- ✅ **Melhorar legibilidade constantemente**:
  ```python
  # ❌ RUIM - Difícil de entender
  def p(d, x, y):
      return sum([d[i][x] * d[i][y] for i in range(len(d)) if x in d[i] and y in d[i]])
  
  # ✅ BOM - Auto-explicativo
  def calculate_correlation_between_features(dataset, feature_x, feature_y):
      """
      Calcula a correlação entre duas features em um dataset.
      
      Args:
          dataset: Lista de dicionários contendo features
          feature_x: Nome da primeira feature
          feature_y: Nome da segunda feature
      
      Returns:
          float: Soma dos produtos das features quando ambas existem
      """
      correlation_sum = 0
      for data_point in dataset:
          if feature_x in data_point and feature_y in data_point:
              correlation_sum += data_point[feature_x] * data_point[feature_y]
      return correlation_sum
  ```

- ✅ **Eliminar redundâncias e aumentar reutilização**:
  ```python
  # ❌ RUIM - Código duplicado (redundância)
  def get_active_users():
      users = db.query("SELECT * FROM users")
      active = [u for u in users if u.status == 'active' and u.verified == True]
      return active
  
  def get_active_admins():
      users = db.query("SELECT * FROM users")
      active = [u for u in users if u.status == 'active' and u.verified == True and u.role == 'admin']
      return active
  
  # ✅ BOM - Código reutilizável (DRY - Don't Repeat Yourself)
  def get_verified_active_users(role=None):
      """Retorna usuários ativos e verificados, opcionalmente filtrados por role."""
      users = db.query("SELECT * FROM users")
      filtered = [u for u in users if u.status == 'active' and u.verified == True]
      
      if role:
          filtered = [u for u in filtered if u.role == role]
      
      return filtered
  
  def get_active_users():
      return get_verified_active_users()
  
  def get_active_admins():
      return get_verified_active_users(role='admin')
  ```

- ✅ **Hierarquizar código em pastas e diretórios**:
  ```
  # ❌ RUIM - Tudo na raiz (difícil de navegar)
  project/
    main.py
    user_stuff.py
    payment_things.py
    email_sender.py
    validators.py
    helpers.py
    utils.py
    config.py
    constants.py
  
  # ✅ BOM - Hierarquia lógica (fácil de entender e manter)
  project/
    main.py
    config/
      __init__.py
      settings.py
      constants.py
    core/
      __init__.py
      models.py
      exceptions.py
    features/
      users/
        __init__.py
        manager.py
        validator.py
      payments/
        __init__.py
        processor.py
        validator.py
    services/
      email/
        __init__.py
        sender.py
        templates.py
    utils/
      __init__.py
      helpers.py
      formatters.py
  ```

- ✅ **Procurar por código órfão após refatoração** (⭐ **OBRIGATÓRIO**):
  
  > **CRÍTICO**: Após qualquer refatoração, é **OBRIGATÓRIO** procurar por código órfão - código que foi implementado mas não está mais sendo utilizado.
  
  **O que é código órfão?**
  - ❌ Funções não utilizadas (definidas mas nunca chamadas)
  - ❌ Variáveis não utilizadas (declaradas mas nunca referenciadas)
  - ❌ Imports não utilizados (importados mas nunca usados)
  - ❌ Código morto/inalcançável (unreachable code)
  - ❌ Classes não instanciadas (definidas mas nunca criadas)
  - ❌ Métodos não chamados (definidos mas nunca invocados)
  
  **Por quê procurar código órfão?**
  - ✅ **Reduz complexidade**: Menos código = mais fácil entender
  - ✅ **Melhora manutenção**: Não gastar tempo em código não usado
  - ✅ **Evita confusão**: Código órfão pode enganar desenvolvedores
  - ✅ **Performance**: Menos código = startup mais rápido
  - ✅ **Segurança**: Código órfão pode conter vulnerabilidades esquecidas
  
  **Ferramentas para detectar código órfão**:
  ```bash
  # Python - Código não utilizado (funções, classes, variáveis)
  pip install vulture
  vulture src/ --min-confidence 80
  # Saída: funções/classes/variáveis não utilizadas
  
  # Python - Imports não utilizados
  pip install autoflake
  autoflake --remove-all-unused-imports --check -r src/
  # Ou usar pylint
  pylint --disable=all --enable=unused-import src/
  
  # JavaScript/TypeScript - Código não utilizado
  npm install -g ts-prune  # Para TypeScript
  ts-prune
  # Ou ESLint
  npm run lint -- --rule 'no-unused-vars: error'
  
  # Para qualquer linguagem - Buscar definições não usadas
  # 1. Gerar lista de definições (funções, classes)
  # 2. Buscar referências a cada definição no código
  # 3. Se nenhuma referência encontrada → código órfão
  ```
  
  **Exemplo de uso (Python)**:
  ```python
  # Antes da refatoração - arquivo com 500 linhas
  
  # Refatoração: dividiu em 3 arquivos menores
  # Agora procurar código órfão:
  
  $ vulture src/ --min-confidence 80
  src/old_module.py:45: unused function 'process_legacy_format' (100% confidence)
  src/utils.py:123: unused function 'deprecated_helper' (90% confidence)
  src/models.py:67: unused class 'OldDataModel' (100% confidence)
  
  # Ação: Remover ou documentar por que manter
  # Se realmente não usado → DELETAR
  # Se será usado futuro → Marcar com comentário e issue
  ```
  
  **Checklist de código órfão** (executar APÓS refatoração):
  ```markdown
  - [ ] Executar vulture (Python) ou ts-prune (TypeScript)
  - [ ] Revisar funções não utilizadas (confirmar se realmente órfãs)
  - [ ] Remover imports não utilizados (autoflake ou ferramenta similar)
  - [ ] Verificar classes não instanciadas
  - [ ] Procurar código comentado antigo (também é código órfão)
  - [ ] Documentar se algum código "órfão" deve ser mantido (ex: API pública)
  ```
  
  **Quando NÃO remover**:
  - ✅ **APIs públicas**: Mesmo não usadas internamente, clientes externos podem usar
  - ✅ **Hooks/callbacks**: Podem ser chamados por frameworks
  - ✅ **Código de teste**: Helpers de teste podem parecer não usados
  - ✅ **Código planejado**: Se há issue/task para usar em breve, manter (mas documentar)

**Quando refatorar**:

1. **Durante implementação de nova feature**:
   - Antes de adicionar código novo, verifique se os arquivos existentes estão organizados
   - Se encontrar código mal estruturado, refatore ANTES de adicionar nova funcionalidade

2. **Após completar uma funcionalidade**:
   - Revise o código implementado
   - Identifique oportunidades de melhoria (DRY, SRP, nomes melhores)
   - Refatore imediatamente enquanto o contexto está fresco
   - **⭐ OBRIGATÓRIO**: Procure por código órfão (vulture, autoflake, etc.)

3. **Ao revisar código (Etapas 7 e 8)**:
   - Use os 9 critérios de qualidade como guia
   - Se detectar redundância, menor coesão ou maior acoplamento → Refatore

4. **Antes de fazer commit (Etapa 13)**:
   - Último checkpoint: código está o mais limpo possível?
   - Há algo que pode ser simplificado?

5. **Periodicidade mínima**:
   - ⚠️ **NUNCA** deixe passar mais de 3-5 funcionalidades sem refatorar
   - 🚨 Se projeto tem > 10 arquivos com > 500 linhas → PRIORIZE refatoração
   - ⭐ **Sempre procure código órfão após refatorar** (não opcional)

**Benefícios da refatoração frequente**:
- ✅ **Manutenção mais simples**: Código organizado é mais fácil de modificar
- ✅ **Menos bugs**: Código limpo tem menos lugares para bugs se esconderem
- ✅ **Onboarding rápido**: Novos desenvolvedores entendem o código mais rápido
- ✅ **Velocidade**: Paradoxalmente, refatorar frequentemente ACELERA o desenvolvimento
- ✅ **Validação facilitada**: Código modular é mais fácil de testar e verificar

**Ferramentas para identificar necessidade de refatoração**:
```bash
# Python - Complexidade ciclomática
pip install radon
radon cc . -a -nb  # Mostrar funções complexas

# Python - Código duplicado
pip install pylint
pylint --disable=all --enable=duplicate-code .

# Python - Código morto
pip install vulture
vulture .

# JavaScript - Análise de complexidade
npm install -g complexity-report
cr --format json src/
```

### 🎯 **Checklist Rápido para IAs**

Antes de gerar/commitar código, verificar:

- [ ] Nomes são descritivos e seguem convenções da linguagem?
- [ ] Funções têm responsabilidade única e são pequenas?
- [ ] Há tratamento de erros para casos excepcionais?
- [ ] Código está testado (unitários + edge cases)?
- [ ] Não há vulnerabilidades de segurança óbvias?
- [ ] Performance é aceitável (sem algoritmos O(n²) desnecessários)?
- [ ] Há documentação (docstrings, comentários úteis)?
- [ ] Código está organizado em módulos lógicos?
- [ ] **Código foi refatorado recentemente?** (arquivos < 500 linhas, sem duplicação)
- [ ] **Hierarquia de pastas está lógica?** (separação clara de responsabilidades)
- [ ] Commits são descritivos (conventional commits)?
- [ ] Dependências estão com versões fixadas?

### 📚 **Recursos Adicionais**

- **Clean Code** (Robert C. Martin) - Princípios de código limpo
- **SOLID Principles** - Orientação a objetos bem feita
- **Design Patterns** (GoF) - Soluções comuns para problemas comuns
- **OWASP Top 10** - Principais vulnerabilidades de segurança
- **PEP 8** (Python) - Guia de estilo Python
- **Google Style Guides** - Guias de estilo por linguagem

---

**Releia este documento antes de cada sprint!**

---

**Versão**: 2.0  
**Última atualização**: 16 de Dezembro de 2025  
**Mantido por**: Josué Amaral  
**Status**: ATIVO - Protocolo oficial do projeto
