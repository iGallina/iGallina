# Passo 2 — Data Brokers (lista priorizada de opt-out)

Eles são legalmente obrigados a remover seus dados quando você pede. Trabalhe
de cima para baixo. Para cada um: ou use o formulário de opt-out direto, ou
envie o template (`templates/`) ao e-mail de privacidade.

> Dica: opt-out exige confirmação por e-mail/CAPTCHA — só você consegue
> concluir. Faça pelo navegador endurecido (Brave/Firefox) e registre datas
> numa planilha (coluna: broker | data do pedido | status | re-checar em).

## 🔴 P1 — Confirmado na sua auditoria

| Broker | Opt-out | Observação |
|---|---|---|
| **ZoomInfo** | `https://privacy.zoominfo.com/` (formulário) | Exposição confirmada. Use também `templates/EN-zoominfo-optout.md`. Peça remoção **e** "do not sell/share". |

## 🟠 P2 — B2B (mais relevantes para um profissional)

| Broker | Opt-out |
|---|---|
| RocketReach | `https://rocketreach.co/optout` |
| Apollo.io | `https://apolloio.zendesk.com/` → solicitar exclusão (privacy@apollo.io) |
| Lusha | `https://www.lusha.com/opt-out/` |
| SignalHire | `https://www.signalhire.com/optout` |
| ContactOut | privacy@contactout.com (pedido de exclusão) |
| Lead411 | `https://www.lead411.com/data-removal-request/` |
| Clearbit (HubSpot) | `https://claim.clearbit.com/claim` → depois "delete" |
| Adapt.io | privacy@adapt.io |
| Hunter.io | `https://hunter.io/claim` → remover |

## 🟠 P2 — People-search (EUA; checar mesmo morando no Brasil)

| Broker | Opt-out |
|---|---|
| Spokeo | `https://www.spokeo.com/optout` |
| BeenVerified | `https://www.beenverified.com/app/optout/search` |
| Whitepages | `https://www.whitepages.com/suppression-requests` |
| MyLife | `https://www.mylife.com/ccpa/index.pubview` |
| Radaris | `https://radaris.com/control/privacy` |
| Intelius / PeopleConnect | `https://www.intelius.com/opt-out/` |
| PeopleFinders | `https://www.peoplefinders.com/opt-out` |
| TruePeopleSearch | `https://www.truepeoplesearch.com/removal` |
| FastPeopleSearch | `https://www.fastpeoplesearch.com/removal` |
| Acxiom | `https://isapps.acxiom.com/optout/optout.aspx` |
| LexisNexis | `https://optout.lexisnexis.com/` |

## 🇧🇷 Brasil — dados que circulam localmente

Não há "opt-out form" padronizado; o caminho é a **requisição LGPD**
(`templates/PT-LGPD-eliminacao-art18.md`) enviada ao DPO/canal de privacidade
da empresa. Aplicável a: bureaus de crédito (Serasa, Boa Vista/SCPC), sites
de "consulta CPF/CNPJ", agregadores de currículo, e qualquer empresa que você
identificar tratando seus dados sem base legal vigente.

- Serasa: `https://www.serasa.com.br/` → canal do titular / privacidade
- Para qualquer empresa BR: e-mail do **Encarregado (DPO)** no rodapé/política
  de privacidade do site → enviar template LGPD.

## Atalho opcional (pago)

Serviços como Optery, DeleteMe, Incogni e Kanary automatizam opt-out em
100+ brokers recorrentemente. Útil porque brokers **te re-adicionam** a cada
poucos meses. Não é necessário — o método manual acima é gratuito — mas
considere para manutenção de longo prazo.

## Como usar os templates

1. Tente primeiro o **formulário de opt-out direto** (mais rápido).
2. Sem formulário, ou ignorado em 30–45 dias → envie o template legal:
   - Broker dos EUA → `templates/EN-CCPA-opt-out.md`
   - Empresa da UE/global → `templates/EN-GDPR-erasure-art17.md`
   - Empresa brasileira → `templates/PT-LGPD-eliminacao-art18.md`
   - Genérico (sem saber jurisdição) → `templates/EN-data-broker-generic.md`
