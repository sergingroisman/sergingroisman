# Fase 2 — Inventário de conteúdo real (verificado na API do GitHub)

Fonte: `api.github.com` em 06/10/2026, conta `sergingroisman`. **Nada aqui foi inventado** — o que não foi possível verificar está marcado como `[CONFIRMAR: …]` e **não deve ser publicado sem aprovação**.

## 1. Perfil público
| Campo | Valor verificado |
|---|---|
| login | `sergingroisman` |
| name | Sérgio Junior |
| bio | **vazio** (`null`) |
| location | **vazio** (`null`) |
| blog / site | **vazio** |
| company | vazio |
| email público | vazio |
| twitter | vazio |
| criado em | 2024-07-14 |
| seguidores / seguindo | 0 / 0 |
| repos públicos | 16 (2 originais + 14 forks) |
| gists públicos | 0 |
| organizações públicas | **nenhuma** |

> ⚠️ O perfil GitHub está **cru**: sem bio, sem localização, sem links. O site/portfólio real (`sergingroisman.github.io`) **não está linkado no perfil**.

## 2. Repositórios públicos

### Projetos próprios (originais)
| Repo | Lang | Descrição | Estado | Uso no README |
|---|---|---|---|---|
| **`teishoku`** | TypeScript (99,4%) | meal-maker — delivery de comida de bairro (monorepo NestJS + Next.js + …) | ativo (pushed 2026-10-05), 0 stars, 0 releases | ⭐ **Projeto principal (Selected Work)** |
| **`sergingroisman.github.io`** | Stylus/HTML/EJS | Blog e portfólio pessoal — Sérgio Santos | ativo (2026-10-05) | Link de site/portfólio |

### Forks (14) — todos de ferramentas de IA/agentes/CLI
OpenHands (1★), rag-api, openclaude, gsd-2, aider, agentmemory, awesome-ratatui, kimi-cli, agent-skills, compoose/`compozy`, goose, SWE-agent, Qwen3-Coder, OpenKombai.

**Leitura estratégica:** os forks revelam **interesse real em agentes de IA, CLIs e orquestração de LLM** (compatível com sua lista de interesses) — mas **não são contribuições suas**. Não devem ser apresentados como projetos.

## 3. Repositórios fixados ("Popular repositories")
`OpenHands`, `rag-api`, `sergingroisman.github.io`, `openclaude`, `gsd-2`, `aider`.
> **Apenas 1 dos 6 é original** (`sergingroisman.github.io`); 5 são forks de terceiros. `teishoku` **não está fixado**. → Ação recomendada: fixar `teishoku` e reduzir forks na vitrine.

## 4. Linguagens realmente utilizadas
- Público verificável: **TypeScript** (dominante — `teishoku` 99k bytes), depois Stylus/HTML/EJS/JavaScript (`github.io`).
- `[CONFIRMAR: NestJS, Next.js, React, Rust, Docker, Kubernetes, Terraform, Keycloak — aparecem no seu texto/perfil profissional, não em código público verificável]`.

## 5. Contribuições públicas (PRs/issues/releases)
- **Nenhuma contribuição pública a repositórios de terceiros foi encontrada.** `[CONFIRMAR: você tem PRs/issues/documentação em repos de terceiros? (empresa, open source, Avanade, projetos pessoais)]`
- **Zero releases** e **zero packages publicados** (`teishoku` sem releases; sem pacotes npm/NuGet).
- `[CONFIRMAR: publicou algum package CLI/npm? qual?]`
- Organizações públicas: nenhuma. `[CONFIRMAR: participação em org/guild de empresa que possa ser citada?]`

## 6. Blog / base de conhecimento
- Existe repo `sergingroisman.github.io` (Hexo + Butterfly, conforme sua memória) → **é o candidato natural para a "Knowledge Base"**.
- `[CONFIRMAR: o blog tem artigos publicados? URLs exatas dos melhores posts?]` — sem isso, a seção fica em **estado vazio honesto**.

## 7. Links já informados no perfil
- Nenhum (todos os campos de link estão vazios no GitHub).
- Links pessoais que você forneceu fora do GitHub: e-mail **serjota@proton.me**, LinkedIn **sergingroisman**, tel +55 81 984889347.
- `[CONFIRMAR: site pessoal canônico = sergingroisman.github.io? existe domínio próprio?]`

## 8. README atual e assets existentes
- **Não existe** Profile README (repo `sergingroisman/sergingroisman` → 404).
- **Não há** pasta `assets/` nem `docs/` no contexto do perfil.
- Não há banner, sprite ou pixel art pré-existente. → **Será preciso criar os assets** (pixel art própria).

---

## 9. Lista consolidada de informações a CONFIRMAR (não publicar sem aprovação)
1. `[CONFIRMAR: e-mail profissional para o README — usar serjota@proton.me?]`
2. `[CONFIRMAR: site pessoal canônico (sergingroisman.github.io e/ou domínio próprio)]`
3. `[CONFIRMAR: LinkedIn URL exata (linkedin.com/in/sergingroisman)]`
4. `[CONFIRMAR: anos exatos de experiência a declarar ("6+ anos" está ok?)]`
5. `[CONFIRMAR: certificações Microsoft reais e se podem ser citadas publicamente]`
6. `[CONFIRMAR: contribuições públicas/PRs/documentação que possam ser linkadas]`
7. `[CONFIRMAR: features reais do `teishoku` para a tabela de Selected Work (o que já funciona hoje)]`
8. `[CONFIRMAR: artigos publicados no blog (URLs) ou declarar Knowledge Base vazia]`
9. `[CONFIRMAR: publicou packages/CLIs? (npm/crates/etc.)]`
10. `[CONFIRMAR: pode citar a Avanade/empresa no README?]`
