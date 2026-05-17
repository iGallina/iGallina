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
- Expõe: nome, cargo ("AI & Automation Manager, Engineering"),
  empregador (Gran Cursos Online), padrão de e-mail corporativo
  (`****@grancursosonline.com.br`), telefone.
- Risco: alto. Alimenta ferramentas de prospecção/spam e outros brokers.
- Ação: `templates/EN-zoominfo-optout.md` (privacy.zoominfo.com).

### 2. Vazamentos de credenciais (a confirmar via HIBP — Passo 6)
- Não verificável por busca pública; exige Have I Been Pwned.
- `redspell84@hotmail.com` é um e-mail antigo (handle de fórum/jogo) —
  alta probabilidade de aparecer em breaches antigos.
- Ação: `04-breach-remediation.md`. **Me cole a lista de breaches** que
  o HIBP retornar e eu monto a ordem de prioridade.

## 🟠 Prioridade 2 — Verificar e remover

### 3. Arquivo `.csv` em domínio governamental
- URL detectada: `https://main.govpilot.com/uuploads/EmailAttachments/6897/55b4f12c-e2023112417_Results_GV_1.csv`
- Apareceu na busca por `ian.gallina@gmail.com`. Pode ser uma planilha de
  registro público (GovPilot é plataforma de governo municipal nos EUA).
- ⚠️ **Não abra e redistribua** — pode conter dados de terceiros. Apenas
  verifique se **o seu** e-mail está lá (Ctrl+F no seu próprio dado).
- Ação se confirmado: pedir takedown ao GovPilot e ao órgão que publicou,
  usando `templates/EN-data-broker-generic.md` (cite CCPA + remoção de
  documento mal-publicado).

### 4. Outros data brokers (não indexados, mas prováveis)
- Para um profissional, os relevantes são B2B: RocketReach, Apollo.io,
  Lusha, SignalHire, ContactOut, Lead411, Clearbit, Adapt.io.
- People-search (EUA, menor relevância p/ residente no Brasil mas checar):
  Spokeo, BeenVerified, Whitepages, MyLife, Radaris, Intelius.
- Ação: `02-data-broker-optout-list.md` (lista priorizada com URLs).

## 🟡 Prioridade 3 — Contas antigas

- `redspell84@hotmail.com` / handle `redspell84`: sem hits públicos no
  índice de busca, mas o handle sugere cadastros antigos em fóruns/jogos
  (2014+). O risco real está nas bases de vazamento desses sites.
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
