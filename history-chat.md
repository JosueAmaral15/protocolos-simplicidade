# Histórico da conversa

Data inicial: 2026-06-09
Projeto: protocolos-simplicidade
Escopo: atualização dos Protocolos Simplicidade para memória de conversa, sincronização PT/EN e lacunas entre protocolos.

## Pedido do usuário

O usuário pediu para:

- adicionar nos Protocolos Simplicidade a necessidade de manter `history-chat.md` como memória resumida da conversa específica de cada projeto;
- registrar a possibilidade de `global-history-chat.md` em pasta pai ou ancestral quando houver coleção ou árvore de projetos, sempre combinado com o usuário;
- usar como exemplos os modelos reais:
  - `/home/josue/Documents/josue-writter-workspace/books/history-chat.md`;
  - `/home/josue/Documents/josue-writter-workspace/global-history-chat.md`;
- verificar consistência entre versões em português e inglês;
- sincronizar lacunas entre idiomas;
- identificar o que faltava no Protocolo 2 em relação ao Protocolo 3;
- copiar para o Protocolo 2 as lacunas relevantes;
- melhorar a orientação criando templates reutilizáveis para os arquivos de memória.

## Ações realizadas até agora

- Adicionada a exigência de `history-chat.md` e a orientação sobre `global-history-chat.md` nos protocolos e READMEs.
- Feito commit e push do primeiro conjunto de mudanças:
  - `abc8bf1 docs: add conversation history memory guidance`
- Auditada a consistência PT/EN.
- Sincronizadas lacunas encontradas:
  - `en/README.md` recebeu seções que existiam nas versões raiz/PT;
  - `pt/PROTOCOLO_SIMPLICIDADE_3.md` recebeu a Etapa 1.0 de leitura inicial que já existia em EN;
  - `en/SIMPLICITY_PROTOCOL_1.md` passou a citar `history-chat.md` e `global-history-chat.md` no checklist de planejamento.
- Copiadas para o Protocolo 2 lacunas relevantes do Protocolo 3:
  - leitura inicial obrigatória de memórias e documentação;
  - CI/CD Quality Gates como obrigatório em contexto enterprise;
  - Rollback Plans como obrigatório em mudanças enterprise críticas;
  - `docs/ROLLBACK.md` na estrutura de documentação;
  - validações finais para CI/CD e rollback.
- Criados templates reutilizáveis em `docs/templates/`:
  - `history-chat-template.pt.md`;
  - `history-chat-template.en.md`;
  - `global-history-chat-template.pt.md`;
  - `global-history-chat-template.en.md`.
- Adicionadas referências aos templates nos READMEs e nas seções de documentação dos Protocolos 1, 2 e 3 em português e inglês.

## Estado atual verificado

- `git diff --check` foi executado e não retornou problemas.
- Há mudanças locais ainda não commitadas depois do commit `abc8bf1`.
- Arquivos alterados nesta fase incluem READMEs, Protocolos 1/2/3 em PT/EN, os novos templates em `docs/templates/` e este `history-chat.md`.
- Os arquivos de modelo externos informados pelo usuário foram usados apenas como referência estrutural; o conteúdo específico deles não foi copiado.
- Nenhum `global-history-chat.md` externo foi criado ou alterado nesta etapa.

## Próximos passos

- [x] Revisar o diff final.
- [ ] Fazer commit das mudanças.
- [ ] Fazer push depois de confirmar que o commit está correto.
- [ ] Combinar explicitamente com o usuário se este repositório também deve atualizar algum `global-history-chat.md` em pasta pai/ancestral.

## Atualização antes de encerrar a sessão

Data/hora: 2026-06-09

- A melhoria principal foi transformar os modelos de memória em templates versionados no repositório dos protocolos.
- O estado está validado com `git diff --check`.
- O próximo passo prático é fazer commit e, depois de validar o commit, fazer push se o usuário quiser publicar esta rodada de alterações.

## Higiene e limites

- Não registrar segredos, tokens, senhas, chaves privadas ou dados sensíveis desnecessários.
- Manter este histórico objetivo e útil para retomar o projeto.
- Registrar no `global-history-chat.md` apenas aprendizados reutilizáveis e somente por combinação com o usuário.

## Atualização 2026-07-03 - Quality gates, SonarQube e coverage antes de branch principal

O usuário pediu para incluir nos Protocolos Simplicidade 2 e 3 a necessidade de usar SonarQube e outras plataformas de teste/controle de qualidade para controle rigoroso, com análise de coverage antes de deploy ou push para branches principais.

Ações realizadas:

- Pesquisadas fontes oficiais sobre quality gates, coverage checks, code scanning e segurança de dependências.
- Atualizado o Protocolo 2 em português e inglês para exigir:
  - SonarQube/SonarCloud como quality gate principal;
  - plataforma externa de coverage como Codecov, Coveralls ou Codacy Coverage;
  - SAST com CodeQL/GitHub Advanced Security, GitLab SAST ou Semgrep;
  - análise de dependências com Snyk, Dependabot, OWASP Dependency-Check ou equivalente;
  - plataformas complementares como Qodana, Codacy, Code Climate ou DeepSource quando o risco/stack exigir;
  - bloqueio de merge/deploy/push direto em branch principal quando coverage ou quality gate falhar.
- Atualizado o Protocolo 3 em português e inglês com regra equivalente para solo developer em produção.
- Validado com `git diff --check` sem problemas.

Estado final:

- As mudanças foram commitadas e publicadas em `origin/main`.
- Commits enviados:
  - `7590d0a docs: add memory templates and sync protocols`;
  - `72bfc30 docs: require quality gates and coverage checks`.

## Atualização 2026-07-19 - Releitura dos protocolos em Downloads e incorporação seletiva

O usuário pediu para reler `/home/josue/Downloads/SIMPLICITY_PROTOCOL_2.md` e `/home/josue/Downloads/SIMPLICITY_PROTOCOL_3.md`, comparar novamente com os protocolos originais do projeto e incorporar apenas recomendações que fizessem sentido, evitando redundâncias e equívocos.

Ações realizadas:

- Comparado o P2 baixado com `en/SIMPLICITY_PROTOCOL_2.md`.
- Comparado o P3 baixado com `en/SIMPLICITY_PROTOCOL_3.md`.
- Confirmado que o P2 baixado tem uma seção útil ausente no projeto: defesa de qualidade em profundidade, com evidência por risco, SonarQube como prova necessária mas insuficiente, mutation testing, testes de banco/autorização/migração, secret scanning, supply-chain security e governança de flaky tests.
- Confirmado que o P3 baixado não tem títulos novos em relação ao P3 do projeto; o P3 do projeto está mais atualizado em memória de conversa, `global-history-chat.md`, proteção contra saturação de RAM e regras de SonarQube/coverage.
- Incorporada uma versão compacta e não redundante da defesa em profundidade nos Protocolos 2 e 3, em português e inglês.
- Acrescentados itens nos checklists finais para exigir evidência registrável: commit exato, comandos/CI, coverage, scanners, testes ignorados/quarentenados, limitações, expiração de exceções e prontidão de rollback.
- Incorporada no Protocolo 2, em português e inglês, uma regra enterprise condicional para projetos com branch persistente de integração: `COM-[UUID]` integra em `develop`/equivalente, e `main` recebe promoção apenas com aprovação explícita e evidências completas.

Estado atual:

- Há mudanças locais não commitadas nos arquivos:
  - `pt/PROTOCOLO_SIMPLICIDADE_2.md`;
  - `en/SIMPLICITY_PROTOCOL_2.md`;
  - `pt/PROTOCOLO_SIMPLICIDADE_3.md`;
  - `en/SIMPLICITY_PROTOCOL_3.md`;
  - `history-chat.md`.
