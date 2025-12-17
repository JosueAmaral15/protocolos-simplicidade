# 📚 Protocolos Simplicidade

**Coleção de Metodologias de Desenvolvimento de Software**
> *Padronização, Qualidade e Eficiência para Diferentes Contextos.*

Este repositório contém a suíte "Simplicidade", um conjunto de protocolos criados por **Josué Amaral** para guiar o ciclo de vida de desenvolvimento de software, desde a prototipagem rápida até sistemas críticos em produção.

Observação importante para os programadores e desenvolvedores de software: você pode ler os protocolos se quiser, mas você NÃO PRECISA aplicar nada no protocolo ou mesmo ler os protocolos, pois isto é somente para as inteligências artificiais lerem para você e programar para você com base no protocolo (por exemplo, com ferramentas avançadas de programação automática com inteligência artificial, como o Github Copilot Pro +). São as inteligências artificiais que precisam ler todo o protocolo e programar com base nesses protocolos, fornecendo mais produtividade e capacidade técnica para as inteligências artificiais desenvolverem código como se fossem programadores reais, como um pleno ou um sênior, por exemplo, objetivo dos protocolos.

---

## 🚦 Guia Rápido: Qual Protocolo Usar?

Não sabe por onde começar? Utilize a tabela abaixo para escolher o protocolo adequado ao momento atual do seu projeto.

| Protocolo | Cor (Book) | Foco Principal | Público Alvo | Contexto Ideal |
| :--- | :--- | :--- | :--- | :--- |
| **[Simplicidade 1](PROTOCOLO_SIMPLICIDADE_1.md)** | 📘 **Blue** | Agilidade & Base | Iniciantes / Interno | Protótipos, MVPs descartáveis, Estudos, Ferramentas Internas. |
| **[Simplicidade 2](PROTOCOLO_SIMPLICIDADE_2.md)** | 📕 **Red** | Governança & Escala | Equipes (2+) | Ambientes Enterprise, Times grandes, Projetos com Code Review e QA dedicado. |
| **[Simplicidade 3](PROTOCOLO_SIMPLICIDADE_3.md)** | 📗 **Green** | Robustez & Autonomia | **Solo Developer** | **Produção**, Projetos Críticos, SaaS Solo, Longo Prazo. |

---

## 📂 Detalhes dos Protocolos

### 📘 [Protocolo Simplicidade 1: A Base](PROTOCOLO_SIMPLICIDADE_1.md)
*Para quem quer começar rápido, mas do jeito certo.*

O protocolo de entrada. Define as 13 etapas fundamentais para garantir que o código funcione, seja testado e documentado, sem burocracia excessiva.
- **Foco:** Ciclo iterativo (Ler -> Planejar -> Codar -> Testar).
- **Garantia:** Zero dívida técnica inicial.
- **Quando NÃO usar:** Se o projeto for para produção com dados sensíveis de usuários (falta checklist de segurança avançada).

### 📕 [Protocolo Simplicidade 2: Enterprise](PROTOCOLO_SIMPLICIDADE_2.md)
*Para equipes que precisam de processos maduros.*

A versão estendida para o mundo corporativo. Adiciona camadas de verificação cruzada para evitar que erros humanos passem despercebidos em times grandes.
- **Diferenciais:** Code Review por Pares, Retrospectivas de Sprint, ADRs (Registros de Decisão Arquitetural).
- **Overhead:** Alto. Exige reuniões e validações de terceiros.
- **Ideal para:** Consultorias, Departamentos de TI estruturados.

### 📗 [Protocolo Simplicidade 3: Solo em Produção](PROTOCOLO_SIMPLICIDADE_3.md)
*O equilíbrio perfeito para o "Exército de Um Homem Só".*

Criado especificamente para o desenvolvedor que não tem equipe, mas precisa da segurança de uma empresa grande. Remove a burocracia de reuniões (do Simplicidade 2) mas impõe rigor técnico extremo (OWASP, CI/CD, Profiling).
- **Filosofia:** "Automatize o que a equipe faria".
- **Diferenciais:** Matriz de Decisão, Segurança Obrigatória (OWASP), Planos de Rollback.
- **Segurança:** Transforma o desenvolvedor solo em um engenheiro de software sênior responsável.

---

## ⚠️ Regra Fundamental para Todos os Protocolos

> **CRÍTICO**: Antes de implementar novas funcionalidades, **todos os erros no workspace devem ser corrigidos**.

Todos os três protocolos agora incluem uma **Regra de Ouro** que deve ser seguida sem exceção:

### 🚨 Prioridade Absoluta para Erros

Considere a existência de erros no workspace (aba "Problemas" do IDE) como **bloqueante**. Os seguintes tipos de erro devem ser corrigidos ANTES de continuar:

- ❌ Problemas de sintaxe
- ❌ Inconsistências de código
- ❌ Omissões inesperadas
- ❌ Fatos incorretos
- ❌ Ambiguidades
- ❌ Arquivos faltosos
- ❌ Falhas de execução

### ✅ Continue Apenas Quando

- ✅ Zero erros na aba "Problemas"
- ✅ Todos os builds completam com sucesso
- ✅ Todos os testes passam
- ✅ Linter/formatter sem erros críticos

### 🤖 Importante: Esta Regra é Para Assistentes de IA

**Esta regra se aplica especificamente a assistentes de IA (como Cursor, GitHub Copilot, etc.):**

- ✅ **A IA DEVE** corrigir todos os erros existentes ANTES de implementar novas funcionalidades
- ✅ **A IA DEVE** resolver problemas de forma proativa, não esperar que humanos os corrijam
- ✅ **A IA DEVE** tratar a correção de erros como prioridade máxima

**Não significa que:**
- ❌ Desenvolvedores humanos devem parar de implementar quando existem erros
- ❌ O projeto não pode avançar enquanto houver erros
- ❌ Humanos precisam corrigir os erros manualmente

**Mensagem para IAs:**
> "Até que os erros não sejam sanados POR VOCÊ (IA), as tarefas e as funcionalidades não podem continuar sendo implementadas POR VOCÊ (IA). Corrija os erros primeiro, depois continue."

Esta regra está documentada em detalhes em cada protocolo após a seção "Filosofia Central".

---

## 📝 Documentação Obrigatória na Pasta `docs/`

> **CRÍTICO**: Tudo aquilo que a inteligência artificial faz no projeto, em cada ciclo de implementação, em cada código, cada funcionalidade implementada, **DEVE SER DOCUMENTADO NA PASTA `docs/` COMO REQUISITO OBRIGATÓRIO** para demarcar as novas funcionalidades e novos comportamentos.

Todos os três protocolos agora incluem um **Requisito Obrigatório de Documentação** que deve ser seguido em cada ciclo:

### 📚 Regra de Ouro da Documentação

**Para Assistentes de IA:**

A IA **DEVE** documentar **TODAS** as implementações na pasta `docs/`:
- ✅ Funcionalidades implementadas (descrição detalhada + comportamentos)
- ✅ Código criado/modificado (arquivos + mudanças)
- ✅ Decisões arquiteturais (padrões aplicados + justificativas)
- ✅ Integrações e dependências
- ✅ Testes implementados (cobertura + cenários)
- ✅ Exemplos de uso práticos

### 📂 Estrutura Mínima Obrigatória

```
docs/
├── REQUIREMENTS.md          # Tarefas e requisitos (atualizado a cada ciclo)
├── vX.Y.Z-SPECIFICATIONS.md # Especificações detalhadas da versão
├── CHANGELOG.md             # Histórico de todas as mudanças
├── ARCHITECTURE.md          # Decisões arquiteturais
└── [outros arquivos conforme protocolo]
```

### 🎯 Por Protocolo

- **Simplicidade 1**: Documentação básica completa (funcionalidades + arquitetura + testes)
- **Simplicidade 2**: + ADRs formais + OWASP + API docs + Acessibilidade
- **Simplicidade 3**: + OWASP obrigatório + Rollback plans + Notas de decisão

### ⚠️ Validação Antes do Commit

A IA **NÃO DEVE** fazer commit sem:
- [ ] ✅ Pasta `docs/` atualizada
- [ ] ✅ SPECIFICATIONS.md criado/atualizado
- [ ] ✅ Todas funcionalidades documentadas
- [ ] ✅ Todos comportamentos descritos
- [ ] ✅ Decisões técnicas justificadas

**Rationale**: Documentação completa garante rastreabilidade, manutenibilidade, continuidade e profissionalismo. É especialmente crítica para projetos em produção e desenvolvimento solo.

📖 **Detalhes completos**: Veja Etapa 12 de cada protocolo para templates, checklists e exemplos.

---

## 📋 Gerenciamento de Tarefas (TASKS.md)

Todos os protocolos Simplicidade agora incluem suporte integrado para gerenciamento de tarefas através de um arquivo `TASKS.md` (ou arquivo alternativo de sua escolha).

### Recursos do Sistema de Tarefas:
- ✅ **Arquivo Padrão**: `TASKS.md` na raiz do projeto (formato ASCII: `.md`, `.txt`)
- 🔄 **Flexível**: Use qualquer nome/localização de arquivo (desde que seja ASCII)
- 📊 **Sistema de Classificação**: Status, Complexidade e Priorização integrados
- 🤖 **Recomendações IA (Opcional)**: Sistema inteligente de sugestão de novas tarefas
- 📊 **Curva de Crescimento**: Recomendações seguem padrão quadrático (crescem, atingem pico, depois diminuem)
- 🎯 **Controle de Escopo**: Apenas sugestões relevantes ao projeto
- 🔢 **Limite Configurável**: Default de 30 novas tarefas recomendadas (personalizável)

### 📊 Sistema de Classificação de Tarefas

Todos os três protocolos incluem um sistema padronizado de classificação para facilitar a organização pela IA:

#### **Status da Tarefa**
- 🔴 **Not Started** - Aguardando início
- 🟡 **In Progress** - Em desenvolvimento
- 🟢 **Done** - Concluído e testado
- 🔵 **Blocked** - Bloqueado por dependência

#### **Complexidade**
- 🟢 **Simples** (0-1h) - Baixo risco, poucas dependências, escopo claro
- 🟡 **Média** (1-2h) - Risco médio, algumas integrações
- 🔴 **Complexa** (>2h) - Alto risco, muitas dependências, escopo aberto

#### **Priorização MoSCoW**
- 🔴 **Must Have** - Crítico para o funcionamento do sistema, bloqueante
- 🟡 **Should Have** - Importante mas não bloqueante
- 🟢 **Could Have** - Desejável se houver tempo, baixa prioridade
- ⚪ **Won't Have** (Later) - Fora do escopo atual, para versões futuras

#### **Frameworks Avançados (Opcional)**
- **Matriz RICE**: Para análise quantitativa (Reach × Impact × Confidence / Effort)
- **Matriz de Eisenhower**: Para gestão de urgências (Urgente × Importante)
- **Matriz de Decisão**: Scoring numérico de 0-35 pontos (Simplicidade 2/3)

**Exemplo de uso combinado**:
```markdown
### 🔴 MUST HAVE
- 🔴🟢 [ ] Implementar autenticação (Not Started, Simples, 1h)
- 🟡🟡 [ ] Adicionar validação (In Progress, Média, 1.5h, 60% completo)
- 🟢🟢 [x] Configurar banco de dados (Done, Simples, 0.5h)
```

### Como Funciona a IA de Recomendações:
A IA pode sugerir novas tarefas dinamicamente conforme o projeto evolui, seguindo um padrão de 5 fases:
1. **Fase 1 (0-20%)**: Crescimento inicial - poucas tarefas essenciais
2. **Fase 2 (20-40%)**: Aceleração - features principais
3. **Fase 3 (40-70%)**: Pico máximo - máximo de ideias e oportunidades  
4. **Fase 4 (70-90%)**: Desaceleração - apenas críticas
5. **Fase 5 (90-100%)**: Exaustão - parar de adicionar features

📖 **Detalhes completos**: Veja seção "Legenda de Classificação de Tarefas" e "Recomendações de Tarefas pela IA" na Etapa 12 de cada protocolo.

---

## 🤖 Como usar com IA (Cursor / Github Copilot)

Estes protocolos foram desenhados para serem lidos por Assistentes de IA. Para obter os melhores resultados, configure sua IA da seguinte forma:

### No Cursor (Rules for AI)
Adicione o seguinte prompt nas configurações globais ou do projeto:

> "Sempre analise o contexto do projeto. Se for um projeto novo ou protótipo, siga estritamente o `PROTOCOLO_SIMPLICIDADE_1.md`. Se eu informar que é um projeto em produção e estou sozinho, adote o `PROTOCOLO_SIMPLICIDADE_3.md` e valide cada etapa de segurança comigo. Sempre consulte o TASKS.md para gerenciar tarefas do projeto."

### No GitHub Copilot
Ao iniciar uma task, invoque o contexto:

> "@workspace Hoje vamos trabalhar na Task #42 do TASKS.md. Como este é um projeto crítico em produção, leia o `PROTOCOLO_SIMPLICIDADE_3.md` e guie-me passo a passo começando pela Etapa 1."

---

## 🔍 Pesquisas Online: Capacidade da IA para Resolver Problemas Complexos

**Todos os protocolos Simplicidade agora incluem orientações sobre pesquisas online para a IA:**

### 📋 Quando a IA Deve Pesquisar Online

Se a inteligência artificial está com **muitas dúvidas** sobre como resolver um determinado problema, ou tem **dificuldades significativas** para resolver esse mesmo problema, ela **pode e deve efetuar pesquisas online**.

### 🎯 Onde Pesquisar

As pesquisas podem ser realizadas em:

1. **📚 Documentação do GitHub de Projetos Relacionados**:
   - Repositórios similares ou que resolvem problemas parecidos
   - Issues e Pull Requests relevantes
   - Wiki e documentação técnica de projetos open source

2. **📖 Plataformas de Documentação Online**:
   - Documentação oficial das bibliotecas e frameworks
   - Tutoriais e guias técnicos especializados
   - Blogs técnicos de desenvolvedores experientes

3. **💬 Plataformas de Perguntas e Respostas**:
   - **StackOverflow**: Principal plataforma para dúvidas de programação
   - **GitHub Discussions**: Para questões específicas de projetos
   - Outras comunidades técnicas relevantes

### ✅ Por Quê Isso é Importante

- ✅ **Economiza tempo**: Problemas complexos já podem ter soluções documentadas
- ✅ **Melhores práticas**: Aprenda com implementações já validadas pela comunidade
- ✅ **Evita reinventar a roda**: Muitos problemas já foram resolvidos por outros
- ✅ **Reduz erros**: Soluções testadas pela comunidade têm menos bugs
- ✅ **Mantém atualizado**: Descubra as abordagens mais modernas

**Detalhes completos**: Veja seção "🌐 Pesquisas Online" na Etapa 3 de cada protocolo.

---

## 🌐 Idioma do Código: Nomenclatura de Variáveis e Comentários

**Todos os protocolos Simplicidade agora incluem diretrizes sobre o idioma do código:**

### 📋 Regra Padrão
- **Por padrão**: Nomes de variáveis e comentários devem estar em **português** para projetos nacionais
- **Alternativa**: Inglês pode ser usado para projetos internacionais ou de código aberto
- **Flexibilidade**: Permite opção mista (variáveis em inglês, comentários em português)

### 🤔 Pergunta Obrigatória
**A IA deve perguntar ao programador na primeira sessão** qual idioma preferir para:
- Nomes de variáveis
- Comentários no código
- Docstrings

Esta preferência será registrada e aplicada consistentemente em todo o projeto.

### 🎯 Rationale
- **Projetos Nacionais**: Português facilita compreensão e manutenção para times brasileiros
- **Projetos Internacionais**: Inglês facilita colaboração com desenvolvedores de todo o mundo
- **Consistência**: Definir padrão no início evita mistura confusa de idiomas

**Detalhes completos**: Veja seção "🌐 Idioma do Código" em cada protocolo.

---

## 📝 Créditos e Versionamento

- **Autor:** Josué Amaral
- **Licença:** Uso interno e educacional.
- **Status:**
    - Simplicidade 1: `v2.0`
    - Simplicidade 2: `v2.2`
    - Simplicidade 3: `v3.1`

> *"Quero um trabalho completo e profissional!"*
