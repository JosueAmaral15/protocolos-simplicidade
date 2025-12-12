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

**Mensagem:**
> "Até que os erros não sejam sanados, as tarefas e as funcionalidades não podem continuar sendo implementadas."

Esta regra está documentada em detalhes em cada protocolo após a seção "Filosofia Central".

---

## 🤖 Como usar com IA (Cursor / Github Copilot)

Estes protocolos foram desenhados para serem lidos por Assistentes de IA. Para obter os melhores resultados, configure sua IA da seguinte forma:

### No Cursor (Rules for AI)
Adicione o seguinte prompt nas configurações globais ou do projeto:

> "Sempre analise o contexto do projeto. Se for um projeto novo ou protótipo, siga estritamente o `PROTOCOLO_SIMPLICIDADE_1.md`. Se eu informar que é um projeto em produção e estou sozinho, adote o `PROTOCOLO_SIMPLICIDADE_3.md` e valide cada etapa de segurança comigo."

### No GitHub Copilot
Ao iniciar uma task, invoque o contexto:

> "@workspace Hoje vamos trabalhar na Task #42. Como este é um projeto crítico em produção, leia o `PROTOCOLO_SIMPLICIDADE_3.md` e guie-me passo a passo começando pela Etapa 1."

---

## 📝 Créditos e Versionamento

- **Autor:** Josué Amaral
- **Licença:** Uso interno e educacional.
- **Status:**
    - Simplicidade 1: `v2.0`
    - Simplicidade 2: `v2.2`
    - Simplicidade 3: `v3.1`

> *"Quero um trabalho completo e profissional!"*
