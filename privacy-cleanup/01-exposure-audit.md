# Passo 1 — Auditoria de Exposição

Resultado da busca pública (OSINT) feita em 2026-05-17 sobre:

- Nome: **Ian Gallina** — Brasília/DF, Brasil
- E-mails: `ian.gallina@gmail.com`, `redspell84@hotmail.com`
- Usuário/handle: `redspell84`, `iGallina`
- Perfis próprios: LinkedIn `/in/ian-gallina`, GitHub `iGallina`

> Nota de método: busca em índice público de buscadores. Data brokers e
> bases de vazamento **não** aparecem bem em buscadores — por isso os
> Passos 2 e 6 (opt-out direto e HIBP) são essenciais e complementam isto.

## 🔴 Prioridade 1 — Remover já

### 1. ZoomInfo (data broker B2B) — EXPOSIÇÃO CONFIRMADA
- URL: `https://www.zoominfo.com/p/Ian-Gallina/6216554018`
- Expõe um **dossiê profissional completo**, não só contato:
  - Nome, cargo atual ("AI & Automation Manager, Engineering")
  - Empregador atual (Gran Cursos Online) + padrão de e-mail corporativo
    (`****@grancursosonline.com.br`) + telefone
  - **Histórico de carreira:** Act (Product Manager), OutSystems, CNI,
    DevSquad, AIS DIGITAL, Ministério das Comunicações
  - **Formação:** Bacharelado pela UniCEUB (Centro Universitário de Brasília)
- Risco: alto. É a fonte mais rica indexada; alimenta ferramentas de
  prospecção/spam e re-popula outros brokers.
- Ação: `templates/EN-zoominfo-optout.md` (privacy.zoominfo.com).

### 2. Vazamentos de credenciais (a confirmar via HIBP — Passo 6)
- Não verificável por busca pública; exige Have I Been Pwned.
- `redspell84@hotmail.com` é um e-mail antigo (handle de fórum/jogo) —
  alta probabilidade de aparecer em breaches antigos.
- Ação: `04-breach-remediation.md`. **Me cole a lista de breaches** que
  o HIBP retornar e eu monto a ordem de prioridade.

## 🟠 Prioridade 2 — Verificar e remover

### 3. Arquivo `.csv` em domínio governamental (GovPilot / OPRA)
- URL detectada: `https://main.govpilot.com/uuploads/EmailAttachments/6897/55b4f12c-e2023112417_Results_GV_1.csv`
  (a mesma pasta `6897/` tem arquivos irmãos: `..._Results_RM_2.csv`)
- Contexto identificado: GovPilot é software de governo municipal/condado
  nos EUA. Esse caminho `EmailAttachments/.../Results_*.csv` são **exports
  de pedidos OPRA** (Open Public Records Act, lei de transparência de
  Nova Jersey/EUA). Seu Gmail apareceu indexado dentro de um desses CSVs.
- Hipótese: seu e-mail entrou numa lista/anexo de um pedido de registro
  público (ou foi raspado para dentro dele), e o município publicou o
  resultado sem redação.
- ⚠️ **Não abra e redistribua** — contém dados de terceiros. Apenas
  verifique se **o seu** e-mail está lá (Ctrl+F no seu próprio dado).
- Ação se confirmado: pedir redação/takedown a **dois** alvos —
  (a) o **Custodian of Records** do município (canal OPRA) e
  (b) **GovPilot** (abuse/privacy, por hospedar o arquivo) — usando
  `templates/EN-data-broker-generic.md` (cite CCPA + documento publicado
  sem base legal + pedido de de-indexação no Google em paralelo,
  `templates/PT-google-conteudo-desatualizado.md`).

### 4. Outros data brokers (não indexados, mas prováveis)
- Para um profissional, os relevantes são B2B: RocketReach, Apollo.io,
  Lusha, SignalHire, ContactOut, Lead411, Clearbit, Adapt.io.
- People-search (EUA, menor relevância p/ residente no Brasil mas checar):
  Spokeo, BeenVerified, Whitepages, MyLife, Radaris, Intelius.
- Ação: `02-data-broker-optout-list.md` (lista priorizada com URLs).

## 🟡 Prioridade 3 — Contas antigas

- `redspell84@hotmail.com` / handle `redspell84`: verificado também em
  Reddit, Steam, Twitch, GitHub e fóruns — **zero footprint público**.
  Bom sinal: o único vetor de risco real é base de vazamento (Passo 6).
- Detalhe de privacidade: o sufixo "84" pode permitir inferência de ano de
  nascimento — evite reusar esse handle em cadastros novos.
- Ação: `03-account-deletion-guide.md` + cruzar com resultado do HIBP.

## 🟢 Prioridade 4 — Perfis próprios (NÃO apagar)

| Perfil | Recomendação |
|---|---|
| LinkedIn `/in/ian-gallina` | Manter (ativo para vagas). Revisar visibilidade pública, ocultar telefone/e-mail, desligar indexação fora do LinkedIn se não quiser. |
| GitHub `iGallina` | Manter. Confirme que o e-mail de commits está privado (`github.com/settings/emails` → "Keep my email address private"). |

Estes são ativos profissionais sob seu controle — a estratégia aqui é
**endurecer privacidade**, não remover.

## O que NÃO foi encontrado (bom sinal)

- Sem perfis públicos indexados em Spokeo/BeenVerified/Whitepages/MyLife
  para o nome (eles não indexam bem — confirmar direto no Passo 2).
- Sem artigos/notícias negativas associados ao nome.
- Sem exposição pública direta de `redspell84@hotmail.com` no índice.

## Próximo passo

Revise esta lista, complete com o que você encontrar manualmente
(Google: `"Ian Gallina"`, seus e-mails entre aspas, `site:` nos brokers)
e siga para o Passo 2.
