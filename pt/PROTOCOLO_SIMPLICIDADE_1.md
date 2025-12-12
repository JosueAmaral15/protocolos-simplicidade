# Protocolo Simplicidade 1

**Autor**: Josué Amaral  
**Data de Criação**: 30 de Novembro de 2025  
**Versão**: 2.0  
**Última Atualização**: 10 de Dezembro de 2025  
**Objetivo**: Metodologia profissional para desenvolvimento incremental de qualidade

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

> **CRÍTICO**: Antes de implementar novas funcionalidades ou continuar com tarefas, **todos os erros no workspace devem ser corrigidos**.

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

**Mensagem**: 
> "Até que os erros não sejam sanados, as tarefas e as funcionalidades não podem continuar sendo implementadas."

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

## 📋 Espinha Dorsal do Protocolo (13 Etapas)

**Resumo Executivo**:
1. 📚 Ler a documentação
2. ✅ Escolher tarefas mais simples
3. ❓ Fazer perguntas até sanar 100% das dúvidas
4. 🔍 Analisar e estudar o projeto
5. 🎯 Fazer sprints das tarefas mais simples
6. 💻 Implementar com arquitetura profissional (GoF + GRASP)
7. ⌨️ **Verificar Implementação CLI + Revisão de Código (9 critérios)**
8. 🖥️ **Verificar Implementação GUI + Revisão de Código (9 critérios)**
9. 🔗 **Verificar Integração com Programa Principal**
🔟 🧪 Fazer testes (100% cobertura)
1️⃣1️⃣ 🧹 Organizar pasta raiz
1️⃣2️⃣ 📝 Preencher documentação
1️⃣3️⃣ 🚀 Fazer commit e push

### 1️⃣ **Ler a Documentação**
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

**Por quê?**: Evita refatorações, economiza tempo, garante código consistente com a base existente.

---

### 5️⃣ **Fazer Sprints das Tarefas Mais Simples**
- Agrupar 2-4 tarefas relacionadas em um sprint
- Estimar tempo total: **máximo 3-4 horas** por sprint
- Manter foco: **uma sprint = uma versão incremental**

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
- **CRÍTICO**: Antes da documentação, **organizar a pasta raiz**
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

2. **Verificação de Estrutura de Diretórios**:
   - `src/` - código-fonte
   - `tests/` - testes unitários
   - `docs/` - documentação
   - Arquivos raiz organizados (README, setup.py, etc.)

**Exemplo**:
```bash
# ANTES (pasta bagunçada):
├── src/
├── apply_v2913_patches.py  ❌ temporário
├── test_temp.py           ❌ teste descartável
├── backup_old/            ❌ backup antigo
├── __pycache__/           ❌ cache
└── file.py.backup_v2913   ❌ backup desnecessário

# DEPOIS (organizado):
├── src/          ✅
├── tests/        ✅
├── docs/         ✅
└── README.md     ✅
```

**Por quê?**: Manter repositório limpo, evitar commits de lixo, facilitar navegação, profissionalismo. Documentar o estado **limpo** do projeto.

---

### 1️⃣2️⃣ **Preencher Nova Documentação**
- **Atualizar arquivo de tarefas/requisitos**: Marcar tasks como `[X]` completas
- **Criar SPECIFICATIONS.md**: Documento detalhado da versão
- **Atualizar estatísticas**: Percentual de conclusão do projeto
- **🤖 [OPCIONAL] Gerenciar recomendações de novas tarefas pela IA**

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
- [ ] **[IA-001]** Implementar autenticação de 2 fatores
  - **Razão**: Segurança crítica para dados de usuários
  - **Impacto**: Alto (requisito de compliance LGPD)
  - **Esforço**: 8-12 horas
  - **Prioridade**: ⭐⭐⭐⭐⭐

### 🟡 SHOULD HAVE (Importantes)
- [ ] **[IA-002]** Adicionar dashboard de analytics
  - **Razão**: Stakeholders solicitaram métricas de uso
  - **Impacto**: Médio (melhora tomada de decisão)
  - **Esforço**: 4-6 horas
  - **Prioridade**: ⭐⭐⭐⭐

### 🟢 COULD HAVE (Melhorias)
- [ ] **[IA-003]** Dark mode no tema da aplicação
  - **Razão**: Pedido frequente de usuários finais
  - **Impacto**: Baixo (UX enhancement)
  - **Esforço**: 2-3 horas
  - **Prioridade**: ⭐⭐⭐

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

#### **Exemplo Completo**

```markdown
# TASKS.md

## 📊 Estatísticas do Projeto
- **Progresso Geral**: 45% completo (18/40 tarefas)
- **Fase Atual**: FASE 3 - PICO MÁXIMO
- **Tarefas IA**: 12/30 recomendadas (40% do limite)

## ✅ Tarefas Concluídas (18)
- [x] Setup inicial do projeto
- [x] Implementar autenticação básica
- [x] CRUD de usuários
... (15 mais)

## 🔨 Tarefas Pendentes Originais (22)
- [ ] Integração com API de pagamento
- [ ] Sistema de notificações
... (20 mais)

## 🤖 Tarefas Recomendadas pela IA (12/30 usadas)

### 🔴 MUST HAVE
- [ ] **[IA-001]** Rate limiting em endpoints da API
  - **Razão**: Prevenir abuso e garantir estabilidade
  - **Impacto**: Alto (segurança e performance)
  - **Esforço**: 3-4 horas
  
- [ ] **[IA-002]** Logging estruturado para debugging
  - **Razão**: Facilitar troubleshooting em produção
  - **Impacto**: Alto (operacional)
  - **Esforço**: 2-3 horas

### 🟡 SHOULD HAVE
- [ ] **[IA-003]** Exportar dados em formato CSV
  - **Razão**: Solicitação de stakeholders para análise
  - **Impacto**: Médio (conveniência)
  - **Esforço**: 2 horas

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
# Clarify v2.9.X - [Nome Descritivo]

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
- **Formato**: Conventional Commits (feat/fix/docs/refactor/test)
- **Mensagem**: Descritiva, completa, com contexto
- **Frequência**: 1 commit por task ou grupo lógico de mudanças

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

**Versão**: 1.4  
**Última atualização**: 01 de Dezembro de 2025  
**Mantido por**: Josué Amaral  
**Status**: ATIVO - Protocolo oficial do projeto
