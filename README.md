# 📚 Protocolos Simplicidade

**Coleção de Metodologias de Desenvolvimento de Software**
> *Padronização, Qualidade e Eficiência para Diferentes Contextos.*

Este repositório contém a suíte "Simplicidade", um conjunto de protocolos criados por **Josué Amaral** para guiar o ciclo de vida de desenvolvimento de software, desde a prototipagem rápida até sistemas críticos em produção.

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

## 📋 Gerenciamento de Tarefas (TASKS.md)

Todos os protocolos Simplicidade agora incluem suporte integrado para gerenciamento de tarefas através de um arquivo `TASKS.md` (ou arquivo alternativo de sua escolha).

### Recursos do Sistema de Tarefas:
- ✅ **Arquivo Padrão**: `TASKS.md` na raiz do projeto (formato ASCII: `.md`, `.txt`)
- 🔄 **Flexível**: Use qualquer nome/localização de arquivo (desde que seja ASCII)
- 🤖 **Recomendações IA (Opcional)**: Sistema inteligente de sugestão de novas tarefas
- 📊 **Curva de Crescimento**: Recomendações seguem padrão quadrático (crescem, atingem pico, depois diminuem)
- 🎯 **Controle de Escopo**: Apenas sugestões relevantes ao projeto
- 🔢 **Limite Configurável**: Default de 30 novas tarefas recomendadas (personalizável)

### Como Funciona a IA de Recomendações:
A IA pode sugerir novas tarefas dinamicamente conforme o projeto evolui, seguindo um padrão de 5 fases:
1. **Fase 1 (0-20%)**: Crescimento inicial - poucas tarefas essenciais
2. **Fase 2 (20-40%)**: Aceleração - features principais
3. **Fase 3 (40-70%)**: Pico máximo - máximo de ideias e oportunidades  
4. **Fase 4 (70-90%)**: Desaceleração - apenas críticas
5. **Fase 5 (90-100%)**: Exaustão - parar de adicionar features

📖 **Detalhes completos**: Veja seção "Recomendações de Tarefas pela IA" na Etapa 12 de cada protocolo.

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

## 📝 Créditos e Versionamento

- **Autor:** Josué Amaral
- **Licença:** Uso interno e educacional.
- **Status:**
    - Simplicidade 1: `v2.0`
    - Simplicidade 2: `v2.2`
    - Simplicidade 3: `v3.1`

> *"Quero um trabalho completo e profissional!"*
