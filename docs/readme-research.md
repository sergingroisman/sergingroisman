# Fase 1 — Resumo da planilha, READMEs validados e análise das referências

## 1. Resumo da planilha `devs-br-github.xlsx`

**Abas:** `Leia primeiro`, `Portfólios`, `Critérios`.

### Como interpreto os dados
- **Fonte de triagem, não verdade absoluta.** O próprio arquivo diz: prioridade é classificação de inspiração de bio/portfólio, "não é ranking de competência profissional", e "Área aparente" é aproximação automática.
- A planilha lista **sites/portfólios**, não Profile READMEs. **Não presumo que bom site ⇒ bom Profile README** — validei cada README separadamente pela API.

### Estrutura da aba `Portfólios` (94 linhas)
| Coluna | Uso |
|---|---|
| Ordem | Ordenação de leitura |
| **Prioridade** | Alta (13) / Média (23) / Exploratória (58) |
| Nome | Identificação do dev |
| **GitHub** | Username → usei para localizar o repo de perfil `<user>/<user>` |
| Site / portfólio | Site público (não usado como prova de README) |
| Código-fonte | Repo do site, quando localizado ("vazio = não identificado") |
| Hospedagem | GitHub Pages / domínio próprio |
| Área aparente | Filtro inicial (Frontend, Cloud/DevOps, IA/Dados, Backend/Arquitetura, Mobile, Cybersecurity, Full Stack) |
| Senioridade declarada | Sênior / Staff / Júnior / "Não informado" |
| Padrões encontrados | Pistas de seções |
| O que observar | Resumo/tagline |
| Status HTTP / Verificado em | 200 em 06/10/2026 |

### Aba `Critérios` (pontos que mudam a interpretação)
- Inclusão = pessoa brasileira/ligada ao Brasil **com site acessível** — logo, a lista é **enviesada para quem tem site**, não para quem tem Profile README.
- "Código-fonte" vazio significa "não identificado", não "fechado".

### Aba `Leia primeiro`
- Instrui a usar a lista como referência de **bio/hero/navegação/estudos de caso** (contexto Kombai), com no máximo 3–5 screenshots por rodada — **nunca clonar**.
- Números declarados: 94 sites, 13 Alta, 23 Média, 58 com código-fonte.

### Varredura de Profile README (feita por mim, além da planilha)
Dos 94 usernames, **59 têm Profile README substancial** (>200 bytes). Baixei e analisei **34** (todas as referências obrigatórias + toda a prioridade Alta + Média e Exploratória alinhadas a backend/arquitetura/cloud/IA/criativo).

---

## 2. READMEs validados (34 analisados)

Legenda: **Q** = qualidade de referência (A alta / B média / C baixa); **Disp** = disponibilidade (200/404).

### Prioridade Alta
| # | Dev | URL | Q | Primeira impressão | Hero/Banner | Seções | Badges/Cards | SVG/GIF | Diferencial | Genérico/Excessivo | Envelhece/Quebra |
|---|---|---|---|---|---|---|---|---|---|---|---|
| 8 | **Guillaume Falourd** | github.com/guillaumefalourd | A | Banner + cumprimento, denso em badges | Gif emoji `blob-sunglasses` (slackmojis) | Languages&Tools / Analytics / Connect / Customize | shields (≈40), metrics, streak, summary-cards, komarev, snake | snake SVG, metrics SVG | Separa "Analytics" e ainda ensina a montar o README | **Excesso**: ~40 badges em 6 linhas + snake + metrics + cards | snake via Action, streak em `herokuapp` (frágil), komarev |
| 13 | **Motirck (Ricardo)** | github.com/Motirck | A | centered, typing SVG, muito organizado | typing-svg (Fira Code) | TechStack por domínio / Architecture / Featured Project / Stats / Certifications / Connect | skillicons + devicon + shields, gh-card, stats, streak | typing SVG | Stack por domínio + metodologias + projeto com features | **Excesso**: 6 tabelas de logos, cards de stats, badges de certificação | typing/stats em `herokuapp`; tabela de logos muito longa no mobile |
| 1 | André Bianchi (nikumu) | github.com/nikumu | A | capsula + typing, limpo | capsule-render + typing | About / What I do / Tech Stack / Current focus | skillicons, shields | capsule | **Barras de %** em `txt` — anti-padrão | barras de % (rejeitado) | capsule-render (render on-the-fly) |
| 3 | Danilo Pantani | github.com/pantani | **A+** | `/whoami` em Go, tom de engenheiro | capsule-render + typing | /whoami /selected_work /stack /stats | shields, follower badge | capsule | **Bloco de código Go** + **seleção de trabalho com PRs reais** (ignite/cli, blockatlas) | quase nada excessivo | mínima (shields + capsule) |
| 4 | Davi Fernandes (davimgfx) | github.com/davimgfx | B | trecho de código JS | — | one-liner + badges | shields | — | abertura em código | boa densidade, pouca estrutura | baixa |
| 5 | Erwin (goerwin) | github.com/goerwin | C | texto puro | — | nenhuma | — | — | denso e direto (4 bullets) | **seco demais** | n/a |
| 6 | Felipe Tuyama (ftuyama) | github.com/ftuyama | B | nome + cargo + badges | — | contínuo | shields, stats | — | conciso | stats | — |
| 7 | Felipe N. Moura (felipenmoura) | github.com/felipenmoura | A | foto falando, tom pessoal | imagem header própria | Who am I / Find me / Communities / Entrepreneurship / Contributions / Motto | — | — | **narrativa pessoal + comunidade**, motto | — | sem deps externas (ótimo) |
| 9 | Hermanyo H. | github.com/hermanyo | C | bullets | — | bullets | shields, stats, snake | snake | — | **quase só stats** | snake/blob output |
| 10 | Luiz Bartolomeu (bartollo) | github.com/bartollo | B+ | texto curto e sênior | — | bio + Find me | — | — | **bio enxuta de sênior** bem escrita | — | nenhuma |
| 11 | Marcelo Adamatti | github.com/adamatti | C | lista de links | — | links | simple-icons SVG | — | links externos como âncora | **só links** | simple-icons v3 (versão antiga) |

### Prioridade Média / Exploratória (relevantes)
| Dev | URL | Q | Destaque | Lição |
|---|---|---|---|---|
| Thiago Marinho (tgmarinho) | github.com/tgmarinho | **A+** | Tabela **Projeto/What I did/Proof** com métricas; métricas via `lowlighter/metrics` **estáticas (sem 3rd-party)**; "How I work"; "AI focus" | **Padrão-ouro de evidência + stats sem dependência frágil** |
| Diogo Cezar (diogocezar) | github.com/diogocezar | A | PT-BR, conquistas com números, stack, experiência por cargo, soft skills, hobbies | Riqueza PT-BR, mas **métricas de negócio não verificáveis** aqui |
| Gleuton Dutra (gleuton) | github.com/gleuton | A | Sênior PT-BR: Especialidades (DDD/Clean/Hexagonal) + tecnologias por camada + interesses + motto | **Closest match ao Sergio** (backend sênior/arquitetura) |
| Alexandre Sanlim | github.com/alexandresanlim | A | `<details>` para Resume/Packages/MCP/Mobile; seção "workspace" | **`<details>` para profundidade sem poluir** |
| Nick-Gabe | github.com/Nick-Gabe | A | Banner próprio + "Skills wall" + "Follower of the day" automático | Criatividade + automação leve |
| Leonardo Cavalcante (leocavalcante) | github.com/leocavalcante | B+ | "Currently / Background / AI Focus" enxuto | Estrutura enxuta e sênior |
| Carlos Becker (caarlos0) | github.com/caarlos0 | A | "Repos I created recently", "What I've been working on", "Books I'm reading", latest posts | **Feed vivo de atividade real** (sem badges) |
| aripiprazole | github.com/aripiprazole | A | Tom hacker (`# hey adventurer`), public stuff / writings | **Identidade textual forte** sem SVG |
| Jonas Galvez (galvez) | github.com/galvez | B+ | "Principal Engineer", livro, manutenção de `@fastify/vite` | Autoridade via trabalho real |
| santanaraphael | github.com/santanaraphael | B+ | "Senior backend engineer… automate what shouldn't be manual" | **Bio de posicionamento** exemplar (1 parágrafo) |
| Alison Pezzott | github.com/alisonpezzott | B | Misão + badges MVP/MCT locais | Credenciais com assets **próprios** |
| Jakeliny Gracielly | github.com/jakeliny | B | banner + skillicons de backend/fintech | skillicons enxuto |
| Vitor Hugo Negrisoli | github.com/vhnegrisoli | ❌ 404 | — | **Sem Profile README** (só site) |

**Total validado com qualidade A/A+/B+:** 16. **Com alguma limitação (C/404):** registradas acima e descartadas como referência principal.
**Limitação declarada:** não há 20 READMEs "excelentes" na planilha; enviesada para *sites*. Usei os 16 validados + os 2 obrigatórios como base.

---

## 3. Análise aprofundada das referências obrigatórias

### 3.1 Guillaume Falourd — `github.com/guillaumefalourd`

- **Primeira impressão / identidade:** cumprimento amigável `<h1><img blob-sunglasses/> Hello World !</h1>`; linha "🇫🇷 Software Developer living in 🇧🇷 working at Zup". Identidade = simpático, internacional, produtivo.
- **Banner:** não há banner próprio; usa um **GIF de emoji** (slackmojis) + `komarev` (contador de views) no topo.
- **Organização visual:** muito **densa em badges**. 6 linhas de badges `style=flat` agrupadas por tema (Linguages& Tools, Clouds, CI, Editor, Segurança, IA). Depois **Analytics** e **Connect**.
- **Cards/estatísticas:** `lowlighter/metrics` (SVG), `github-readme-streak-stats`, `github-profile-summary-cards`, StackOverflow reputation, GitHub stars.
- **Contribuições/atividade:** **snake animation** (contribution grid) gerada por GitHub Action no próprio repo.
- **Links:** badges shields em linha (`<p align=left>`), tudo por `bit.ly` + `mailto`.
- **Profissional × personalidade:** 95% profissional (stack/analytics/contato); personalidade só no tom do cumprimento.
- **Automações GitHub Actions:** snake (repo `output` branch) + Metrics + summary-cards — **o autor explica no fim** e ensina a replicar.
- **Claro/escuro:** badges usam fundo escuro fixo (`05122A`) → no tema claro ficam "flutuando"; **não é theme-agnostic**.
- **Dependências/custo de manutenção:** ALTO — 4+ serviços externos (`herokuapp`, `komarev`, `metrics`, `shields`, slackmojis). `herokuapp` de streak **já migrou de domínio** (quebradiço).
- **Ideia reutilizável (sem copiar):** *seção que explica a própria automação* + agrupar stack por tema em vez de listar tudo junto.

### 3.2 Motirck (Ricardo Alves Paula) — `github.com/Motirck`

- **Primeira impressão / identidade:** centralizado, `typing-svg` "Hi there, I'm Ricardo 👋 / Senior Software Engineer", tagline "Always Learning & Building". Identidade = organizado, sênior, corporativo.
- **Banner:** sem banner gráfico; **typing SVG** + linha de bio centrada + followers/views badges.
- **Organização visual:** núcleo em **6 tabelas de logos** (Backend, Frontend, Databases, Cloud&DevOps, Tools&IDE, PM&Collaboration), cada célula = ícone 48px + nome. Depois Architecture & Methodologies (lista), Featured Project, Stats, Certifications, Connect.
- **Cards/estatísticas:** `github-readme-stats`, `streak-stats`, `gh-card` (Featured Project), `komarev`.
- **Certificações:** tabela de 5 badges de imagem (Docker, Scrum, LGPD, Remote Work, Lifelong Learner) — **assets hospedados no próprio repo**.
- **Links:** badges shields `for-the-badge` centralizados (LinkedIn, GitHub, Instagram).
- **Equilíbrio pessoal × técnico:** majoritariamente técnico; pessoal reduzido a "passionate Full Stack Developer from Timóteo".
- **Excessos:** 6 tabelas de logos ≈ **45 ícones** — muito longo, **ruim no mobile** e envelhece rápido; cards de stats padronizados.
- **Dependências:** `skillicons.dev`, `devicon` (jsDelivr), `herokuapp` (streak), `gh-card`. Maioria estável, mas há hotspots frágeis.
- **Ideia reutilizável:** *stack separada por domínio* + *seção de arquitetura/metodologias* + *projeto principal com bullets de features técnicas* + certificações com **assets próprios**.

### 3.3 Comparação com os 3 melhores da planilha
| Critério | Guillaume | Motirck | **Pantani** | **tgmarinho** | **gleuton** |
|---|---|---|---|---|---|
| Evidência real de trabalho | Baixa (stats) | Média (1 projeto) | **Altíssima (PRs reais)** | **Altíssima (métricas + proof)** | Média (relato) |
| Densidade visual | Muito alta | Alta | Média | Baixa/média | Baixa |
| Dep. externas frágeis | **Muitas** | Muitas | Poucas | **Nenhuma p/ stats (SVG estático)** | 1 (streak) |
| Theme cl/escuro | Não robusto | Parcial | Robusto | Robusto | Parcial |
| Mobile | Ruim (6 linhas badges) | Ruim (6 tabelas) | Bom | Bom | Bom |
| Adequação sênior→arquiteto | Média | Boa | **Alta** | **Alta** | **Alta** |
| Personalidade | Baixa | Baixa | Média (Go/bloco código) | Média | Média |

**Veredito:** as referências favoritas brilham em *organização e amplitude*, mas falham em **evidência, dependências frágeis e leitura no tema claro/mobile**. Os melhores da planilha (Pantani, tgmarinho, gleuton) mostram o caminho para um README sênior **com provas e leve**.
# Fase 1 — Matriz de padrões (REFERENCE / PATTERN / WHY / ADAPTATION / RISK / DECISION)

Agrupada nas categorias pedidas. **DECISION**: ✅ adotar · 🔶 adaptar · ⚪ opcional · ❌ rejeitar.

## A. Credibilidade
| REFERENCE | PATTERN | WHY IT WORKS | ADAPTATION (Sergio) | RISK | DECISION |
|---|---|---|---|---|---|
| Pantani, tgmarinho | Trabalho selecionado com **PRs/links verificáveis** | Prova > afirmação; mostra impacto | `/selected_work` ligando a PRs/issues/docs reais | Nenhum (é o diferencial) | ✅ |
| tgmarinho | Tabela **Projeto / What I did / Proof** | Escaneável e honesto | Mesma tabela, 3–6 projetos, incl. `teishoku` | Métricas inventadas → usar só o verificável | 🔶 |
| gleuton, santanaraphael, bartollo | Bio sênior em **1 parágrafo** de posicionamento | Comunica nível em 5s | 2–3 linhas: sênior TS/Node → arquitetura | frases genéricas | ✅ |
| Motirck, gleuton | **Stack por domínio** | Organiza em vez de enumerar | Toolbox por capacidade (Languages/Backend/…) | virar "lista de logos" | 🔶 |
| Pantani, galvez | Autoridade por **manutenção real** (Fastify, ignite) | Credibilidade concreta | Citar contribuições de forks (kimi-cli, agentmemory) | inventar contribuição | 🔶 |
| Alison, Motirck | Certificações/credenciais em destaque | Prova de formação | Incluir **Microsoft Certs** (voucher via ESI/Avanade) só se aprovado | expor info corporativa | ⚪ |

## B. Personalidade
| REFERENCE | PATTERN | WHY | ADAPTATION | RISK | DECISION |
|---|---|---|---|---|---|
| aripiprazole | **Voz textual forte** (`# hey adventurer`) sem SVG | Cria identidade sem asset | Voz de "engineering command center", sem clichês | exagero no tom | 🔶 |
| felipenmoura | Narrativa pessoal + comunidade + **motto** | Humaniza | "Beyond Code" curto (games/anime/carros/homelab) + motto próprio | seção longa demais | 🔶 |
| caarlos0 | **Hobbies + leituras** ("Books I'm reading") | Mostra pessoa, não só stack | Beyond Code discreto | envelhece (livros) | ⚪ |
| diogocezar | "Fun facts" | Proximidade | 1–2 fun facts verificáveis | inventar | ⚪ |
| Nick-Gabe | "Follower of the day" automatic | Engajamento | **Rejeitado** (automation fútil, 0 followers) | — | ❌ |

## C. Escaneabilidade
| REFERENCE | PATTERN | WHY | ADAPTATION | RISK | DECISION |
|---|---|---|---|---|---|
| tgmarinho, Pantani | Hierarquia clara + sumário implícito | Navegação rápida | Seções numeradas/curtas | — | ✅ |
| alexandresanlim | `<details>` para conteúdo longo (Resume/Packages) | Profundidade sem poluir | `<details>` para Toolbox completa/Contributions | quebra acessibilidade em alguns clientes | 🔶 |
| gleuton, bartollo | Bullets curtos, zero enfeite | Escaneável | Bullets em Current Quest/Engineering Profile | fica seco demais | ✅ |
| Motirck, diogocezar | Emojis como âncora de seção | Escaneável | Emojis discretos consistentes | excesso | 🔶 |
| santanaraphael | README **curto** de 1 parágrafo | Respeita o tempo | Manter topo curto; profundidade em `<details>` | — | ✅ |

## D. Impacto visual
| REFERENCE | PATTERN | WHY | ADAPTATION | RISK | DECISION |
|---|---|---|---|---|---|
| Pantani, nikumu | **capsule-render** (header/footer wave) | Moldura leve | Banner próprio em pixel art (**<picture>**) — evitar serviço externo | dep. de terceiros/`herokuapp` | ✅ (local) / ❌ (service) |
| Motirck, nikumu | `readme-typing-svg` | Movimento/charme | ⚪ opcional; prefira **texto alternativo** | recurso externo, quebra em alguns clients | ⚪ |
| Guillaume, Hermanyo | **Snake animation** via GitHub Action | Destaque | ❌ rejeitado (mais uma automação + ruído) | — | ❌ |
| Nick-Gabe, jakeliny, ftuyama | **skillicons.dev** | Stack visual compacta | ⚪ opcional, 1 linha só p/ capacidades | envelhece quando faltar ícone | ⚪ |
| davimgfx, adamatti | Abertura/instrumentos em **código** | Charme técnico | Bloco `ts` curto no banner/perfil | — | 🔶 |

## E. Compatibilidade com pixel art e menu de jogo
| REFERENCE | PATTERN | WHY | ADAPTATION | RISK | DECISION |
|---|---|---|---|---|---|
| nikumu, Pantani | Banner + divisores | Estrutura visual | **Pixel art própria** (banner + divisores) em `assets/` | fontes, claro/escuro | ✅ |
| Pantani | `/whoami`, `/selected_work` (estética de CLI/menu) | Dá "query" ao perfil | Menu de jogo: `[ INÍCIO ■] [ PERFIL ] [ PROJETOS ]…` como **índice textual** | ícone sem label = inacessível | ✅ |
| Nik-Gabe | RGB/hex da marca em badges | Consistência | Paleta **própria** de pixel art | copiar paleta alheia → proibido | ✅ (própria) |

## F. Adequação a sênior evoluindo para arquiteto
| REFERENCE | PATTERN | WHY | ADAPTATION | RISK | DECISION |
|---|---|---|---|---|---|
| gleuton | Seção **Especialidades** com DDD/Clean/Hexagonal | Sinaliza arquitetura | Engineering Profile (Arquitetura/Backend/Cloud/IA/IAM/Tooling) | — | ✅ |
| tgmarinho | "How I work" | Mostra método | Bloco curto de princípios (spec-driven, secure by design) | virar autoajuda | 🔶 |
| Pantani | "Currently/Experiments" | Está construindo | **Current Quest** (arquitetura, secure dev, agentes IA, CLIs, homelab) | — | ✅ |
| Motirck | Projeto principal destacado | Profundidade | `teishoku` como projeto principal | só 1 projeto original público | ✅ |
| galvez, leocavalcante | Transição de carreira explícita | Contexto | "evoluindo para arquitetura de software" | — | ✅ |

## G. Padrões que devem ser evitados ❌
| Padrão | Onde aparece | Por que evitar |
|---|---|---|
| Barras de % de habilidade | nikumu | Subjetivo, não verificável, clichê |
| Lista gigante de logos (6 tabelas) | Motirck | Ruim no mobile, envelhece, poluição |
| Excesso de badges (~40) | Guillaume | Ruído visual, quebra tema claro |
| Stats/cards sem contexto (+ `herokuapp`) | Guillaume, Motirck, Hermanyo | Serviços frágeis, números não explicam senioridade |
| Snake animation | Guillaume, Hermanyo, HakaCode | Automação sem valor, ruído |
| Clichês ("apaixonado por tecnologia", "café em código") | diogocezar/vários | Genérico |
| Botão "Nominate me to GitHub Stars"/pedido de sponsor | alexandresanlim | Soa promocional |
| README puramente template/gerado | hermanno, heynemann (`<!-- -->` default) | Zero valor de referência |
| Contador de views (`komarev`) no topo | Guillaume, Motirck, maykbrito | Métrica de vaidade, dep. externa |
