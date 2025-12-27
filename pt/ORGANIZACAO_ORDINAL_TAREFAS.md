# Organização Ordinal de Tarefas - Protocolos Simplicidade

**Versão**: 1.0  
**Data de Criação**: 27 de Dezembro de 2025  
**Autor**: Josué Amaral  
**Status**: ATIVO

---

## 🎯 Objetivo

Este documento define o sistema de **Organização Ordinal de Tarefas** para os Protocolos Simplicidade, permitindo que desenvolvedores humanos e inteligências artificiais identifiquem rapidamente:

- ✅ **Ordem de execução** das tarefas (do mais simples ao mais complexo)
- ✅ **Dependências** entre tarefas (quais devem ser feitas primeiro)
- ✅ **Paralelização** (quais podem ser executadas simultaneamente)
- ✅ **Organização hierárquica** (estrutura de árvore/grafo)

---

## 📊 Sistema de Prefixos Ordinais

### Nível 1: Numeração Simples (Tarefas Independentes)

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

### Nível 2: Hierarquia com Letras (Grupos de Tarefas)

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

### Nível 3: Hierarquia Profunda (Dependências Complexas)

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

## 🌳 Estrutura de Árvore/Grafo

### Conceitos Fundamentais

#### 1. **Nós Pai e Filhos**

```
B.C.2 (PAI - executar DEPOIS)
   ├── B.C.2.1 (FILHO - executar ANTES)
   └── B.C.2.2 (FILHO - executar ANTES)
```

**Regra**: 
- ✅ **Filhos devem ser completados ANTES do pai**
- ✅ Filhos são **pré-requisitos** do pai
- ✅ Pai **depende** dos filhos

#### 2. **Irmãos (Parallel)**

```
B.C.2.1 (irmão)
B.C.2.2 (irmão)
```

**Regra**:
- ✅ Irmãos podem ser executados **paralelamente**
- ✅ Sem dependência entre si
- ✅ Podem estar em **branches separadas**

#### 3. **Primos, Tios, Avós (Parallel vs Serial)**

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

## 🔄 Paralelização vs Serialização

### Tarefas PARALELAS (podem ser simultâneas)

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

### Tarefas SERIAIS (devem ser sequenciais)

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

## 🎨 Exemplos Práticos

### Exemplo 1: Projeto Simples (Flat)

```markdown
# TASKS.md - Projeto de Blog

## 🔴 MUST HAVE

1. 🔴🟢 [ ] Criar modelo de Post (Simples, 1h)
2. 🔴🟢 [ ] Criar modelo de Comentário (Simples, 1h)
3. 🔴🟡 [ ] Implementar CRUD de Posts (Médio, 2h)
4. 🔴🟡 [ ] Implementar CRUD de Comentários (Médio, 2h)

**Análise**:
- Tarefas 1 e 2 são PARALELAS (modelos independentes)
- Tarefa 3 depende de 1 (SERIAL)
- Tarefa 4 depende de 2 (SERIAL)
- Tarefas 3 e 4 são PARALELAS entre si

**Estratégia de Branches**:
- Branch 1: Implementar 1 → 3
- Branch 2: Implementar 2 → 4
```

---

### Exemplo 2: Projeto Médio (Hierárquico)

```markdown
# TASKS.md - Sistema de E-commerce

## 🔴 MUST HAVE - Release v1.0.0

A. Autenticação
   🔴🟡 [ ] A.1. Implementar modelo User (Médio, 1.5h)
   🔴🟡 [ ] A.2. Implementar login JWT (Médio, 2h)
   🔴🔴 [ ] A.3. Implementar 2FA (Complexo, 3h)

B. Catálogo de Produtos
   🔴🟢 [ ] B.1. Modelo Product (Simples, 1h)
   🔴🟡 [ ] B.2. CRUD Products (Médio, 2h)
   🔴🟡 [ ] B.3. Busca e filtros (Médio, 2.5h)

C. Carrinho de Compras
   🔴🟢 [ ] C.1. Modelo Cart (Simples, 1h)
   🔴🟡 [ ] C.2. Adicionar/remover items (Médio, 1.5h)
   🔴🔴 [ ] C.3. Checkout (Complexo, 4h)

**Análise de Dependências**:
- A.2 depende de A.1 (SERIAL: A.1 → A.2)
- A.3 depende de A.2 (SERIAL: A.2 → A.3)
- B.2 depende de B.1 (SERIAL: B.1 → B.2)
- B.3 depende de B.2 (SERIAL: B.2 → B.3)
- C.2 depende de C.1 (SERIAL: C.1 → C.2)
- C.3 depende de C.2 e A.2 (SERIAL: C.2, A.2 → C.3)

**Grupos A, B, C são PARALELOS** (até C.3 que precisa de A.2)

**Estratégia de Branches**:
- Branch feat/auth: A.1 → A.2 → A.3
- Branch feat/catalog: B.1 → B.2 → B.3
- Branch feat/cart: C.1 → C.2
- Branch feat/checkout: C.3 (depois de merge de auth e cart)
```

---

### Exemplo 3: Projeto Complexo (Grafo Profundo)

```markdown
# TASKS.md - Plataforma de Visualização de Dados

## 🔴 MUST HAVE - Release v1.0.0

A. Infrastructure
   🔴🟢 [ ] A.1. Estrutura de diretórios (Simples, 0.5h)
   🔴🟢 [ ] A.2. Dependências (Simples, 0.5h)

B. Core - Estruturas
   🔴🟡 [ ] B.1. Classe Node (Médio, 1h)
       Depende: A.1, A.2
   🔴🟡 [ ] B.2. ExpressionTree (Médio, 1.5h)
       Depende: B.1

C. Conversões
   🔴🔴 [ ] A.C.1. Número → Árvore (Complexo, 2h)
       Depende: A.1, A.2, B.1, B.2
       Notação: A (infra) → C (conversão) → 1 (específico)
       
   🔴🟡 [ ] B.C.2. Árvore → RPN (Médio, 2.5h)
       🔴🟡 [ ] B.C.2.1. Parser RPN (Médio, 1h)
           Depende: B.1, B.2
       🔴🟡 [ ] B.C.2.2. Serializer RPN (Médio, 1h)
           Depende: B.1, B.2
       🔴🟡 [ ] B.C.2. Conversão completa (Médio, 0.5h)
           Depende: B.C.2.1, B.C.2.2

D. Interface Gráfica
   🔴🔴 [ ] C.B.1.D.1. Integrar Dash com Cytoscape (Complexo, 2.5h)
       Leitura direita→esquerda: D.1 → 1 → B → C
       Depende: B.1, B.2, C (conversões)
       
   🔴🔴 [ ] D.2. Drag-and-drop (Complexo, 2h)
       Depende: C.B.1.D.1

**Ordem de Execução Recomendada**:

1. **Sprint 1** (PARALLEL - 3 branches):
   - Branch infra: A.1, A.2
   - Aguardar merge

2. **Sprint 2** (PARALLEL - 2 branches):
   - Branch core: B.1 → B.2
   - Aguardar merge

3. **Sprint 3** (PARALLEL - 3 branches):
   - Branch conversao-num: A.C.1
   - Branch parser: B.C.2.1
   - Branch serializer: B.C.2.2
   - Aguardar merge dos 3

4. **Sprint 4** (SERIAL):
   - Branch conversao-rpn: B.C.2 (merge 2.1 e 2.2 primeiro)

5. **Sprint 5** (SERIAL):
   - Branch gui-integration: C.B.1.D.1
   - Branch gui-drag: D.2 (depois de C.B.1.D.1)
```

---

## 📋 Como Decidir a Organização

### Fluxograma de Decisão

```
┌─────────────────────────────────────┐
│ A tarefa tem dependências?          │
└─────────────┬───────────────────────┘
              │
        ┌─────┴─────┐
        │           │
       SIM         NÃO
        │           │
        │           ▼
        │     ┌───────────────────────┐
        │     │ Use numeração simples │
        │     │ 1., 2., 3., ...       │
        │     │ (PARALLEL)            │
        │     └───────────────────────┘
        │
        ▼
  ┌─────────────────────────────┐
  │ Múltiplas dependências      │
  │ complexas?                  │
  └─────────────┬───────────────┘
                │
          ┌─────┴─────┐
          │           │
         SIM         NÃO
          │           │
          │           ▼
          │     ┌────────────────────────┐
          │     │ Use hierarquia simples │
          │     │ A.1, A.2, B.1, B.2     │
          │     │ (GRUPOS PARALLEL)      │
          │     └────────────────────────┘
          │
          ▼
    ┌──────────────────────────────┐
    │ Use hierarquia profunda      │
    │ A.C.1, B.C.2.1, C.B.1.D.1    │
    │ (GRAFO - leitura ←)          │
    └──────────────────────────────┘
```

---

## 🎯 Integração com Sistema de Classificação Existente

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

## ✅ Checklist para Desenvolvedores

Ao organizar tarefas com sistema ordinal:

```markdown
- [ ] Identificar tarefas independentes (numeração simples: 1, 2, 3)
- [ ] Agrupar tarefas relacionadas (hierarquia: A.1, A.2, B.1)
- [ ] Mapear dependências explícitas (grafo: A.C.1, B.C.2.1)
- [ ] Definir ordem de execução (folhas → raiz, bottom-up)
- [ ] Identificar oportunidades de paralelização (irmãos, primos)
- [ ] Planejar estratégia de branches (1 branch por grupo parallel)
- [ ] Documentar dependências complexas (comentários no TASKS.md)
- [ ] Validar que ordem está correta (filhos antes de pais)
- [ ] Comunicar claramente aos membros da equipe
- [ ] Atualizar à medida que dependências mudam
```

---

## 🤖 Instruções para Inteligências Artificiais

### Quando Sugerir Organização Ordinal

A IA deve sugerir organização ordinal quando:

✅ **Projeto tem >10 tarefas** com interdependências
✅ **Múltiplos desenvolvedores** trabalhando simultaneamente
✅ **Tarefas bloqueantes** (uma depende de outra)
✅ **Risco de conflitos** no controle de versão
✅ **Necessidade de paralelização** para acelerar desenvolvimento

### Como a IA Deve Aplicar

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

### Exemplo de Sugestão da IA

```markdown
💡 **Sugestão da IA**: Organizei as tarefas com prefixos ordinais

Análise de dependências:
- Grupo A (Autenticação): 3 tarefas SERIAIS
- Grupo B (API): 2 tarefas SERIAIS
- Grupo C (UI): 1 tarefa, depende de A

Oportunidades de paralelização:
✅ Grupos A e B podem ser desenvolvidos simultaneamente
✅ Total de 2 branches paralelas → Redução de 40% no tempo

Estratégia recomendada:
1. Sprint 1 (parallel): Iniciar A.1 e B.1
2. Sprint 2 (parallel): Continuar A.2 e B.2
3. Sprint 3 (serial): A.3 (sem parallel disponível)
4. Sprint 4 (serial): C.1 (aguarda A)

Prefiro essa organização ou prefere ajustar?
```

---

## 📖 Referências e Inspiração

Este sistema foi inspirado em:

- ✅ **Notação Dewey Decimal** (bibliotecas)
- ✅ **Ordenação Topológica** (algoritmo de grafos)
- ✅ **Work Breakdown Structure (WBS)** (gerenciamento de projetos)
- ✅ **Dependency Graphs** (compiladores, build systems)
- ✅ **Estruturas de diretórios** (sistemas de arquivos)

---

## 🎯 Benefícios do Sistema Ordinal

### Para Desenvolvedores Humanos

✅ **Clareza**: Sabe exatamente qual tarefa fazer primeiro
✅ **Autonomia**: Não precisa perguntar "posso começar isso?"
✅ **Eficiência**: Identifica rapidamente tasks paralelas
✅ **Organização**: Estrutura hierárquica facilita navegação
✅ **Comunicação**: Time alinhado sobre ordem de execução

### Para Inteligências Artificiais

✅ **Decisão algorítmica**: Pode calcular ordem automaticamente
✅ **Otimização**: Sugere paralelização para acelerar desenvolvimento
✅ **Validação**: Detecta dependências circulares
✅ **Planejamento**: Estima tempo total considerando parallel tasks
✅ **Priorização**: Combina prefixo ordinal com MoSCoW/Complexidade

### Para o Projeto

✅ **Velocidade**: Paralelização reduz tempo total
✅ **Qualidade**: Ordem correta evita retrabalho
✅ **Previsibilidade**: Cronograma mais preciso
✅ **Redução de conflitos**: Branches isoladas minimizam merge conflicts
✅ **Rastreabilidade**: Histórico de dependências documentado

---

## 📝 Conclusão

O sistema de **Organização Ordinal de Tarefas** é uma ferramenta poderosa para:

1. **Organizar** tarefas do mais simples ao mais complexo
2. **Identificar** dependências e ordem de execução
3. **Paralelizar** desenvolvimento para acelerar entregas
4. **Minimizar** conflitos em controle de versão
5. **Comunicar** claramente a estrutura do projeto

Use este sistema quando o projeto crescer em complexidade e a equipe precisar coordenar esforços de desenvolvimento paralelo.

---

**Versão**: 1.0  
**Status**: ATIVO  
**Mantido por**: Josué Amaral  
**Próxima revisão**: Conforme feedback da comunidade
