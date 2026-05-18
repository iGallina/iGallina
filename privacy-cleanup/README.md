# Remoção de Presença Digital — Ian Gallina

Plano operacional completo para mapear, remover e prevenir exposição de dados
pessoais. Baseado no fluxo de 7 passos do thread, adaptado ao seu caso real
(Brasil / LGPD + GDPR + CCPA) com os resultados da auditoria já feita.

> **Importante — o que eu fiz e o que você precisa fazer**
>
> - ✅ **Feito por mim:** busca pública (OSINT) nos seus identificadores,
>   categorização e priorização da exposição, e todos os templates legais
>   prontos para enviar.
> - ⚠️ **Só você pode fazer:** rodar o Have I Been Pwned (exige confirmação
>   por e-mail), enviar os formulários/e-mails de opt-out (exigem CAPTCHA e
>   confirmação na sua caixa), e preencher seus dados pessoais nos templates
>   (`templates/_SEUS-DADOS.md`). Eu **não** envio requisições no seu nome.

---

## Resumo da auditoria (detalhes em `01-exposure-audit.md`)

| Prioridade | Item | Tipo | Ação |
|---|---|---|---|
| 🔴 P1 | Perfil **ZoomInfo** (`zoominfo.com/p/Ian-Gallina/6216554018`) | Data broker B2B | `templates/EN-zoominfo-optout.md` |
| 🔴 P1 | Vazamentos de e-mail (Passo 6 — HIBP) | Data breach | `04-breach-remediation.md` |
| 🟠 P2 | CSV em domínio `.gov` (`main.govpilot.com/uuploads/...`) | Registro público / possível vazamento | Verificar + `templates/EN-data-broker-generic.md` |
| 🟠 P2 | Outros data brokers (Spokeo, RocketReach, Apollo, Lusha…) | Data broker | `02-data-broker-optout-list.md` |
| 🟡 P3 | Contas antigas / fóruns (incl. `redspell84@hotmail.com`) | Old accounts | `03-account-deletion-guide.md` |
| 🟢 P4 | LinkedIn `/in/ian-gallina`, GitHub `iGallina` | Perfil próprio | Endurecer privacidade, **não** apagar |

---

## Os 7 passos

1. **Saber o que está visível** → `01-exposure-audit.md` (já feito; revise e complete)
2. **Data brokers (ganho fácil)** → `02-data-broker-optout-list.md` + `templates/`
3. **Matar contas mortas** → `03-account-deletion-guide.md`
4. **Requisições legais (LGPD/GDPR/CCPA)** → `templates/`
5. **Se não dá pra apagar, soterre** → `05-future-proofing.md` (seção "Reputação")
6. **Limpar vazamentos de dados** → `04-breach-remediation.md`
7. **Prevenir vazamentos futuros** → `05-future-proofing.md`

## Ordem de execução recomendada

1. Preencha `templates/_SEUS-DADOS.md` (5 min — destrava todo o resto).
2. Rode o **Have I Been Pwned** nos dois e-mails (`04-breach-remediation.md`)
   e me cole a lista de volta: eu priorizo troca de senha / 2FA / exclusão.
3. Envie o opt-out do **ZoomInfo** (P1, exposição confirmada).
4. Trabalhe a lista de brokers de cima pra baixo (`02-...`).
5. Verifique o CSV `.gov` e dispare o template genérico se seu dado estiver lá.
6. Limpe contas antigas (`03-...`).
7. Configure a prevenção contínua (`05-...`) e agende re-checagem em 90 dias —
   brokers te re-listam; isto é manutenção, não uma tarefa única.

## Aviso legal

Estes templates são modelos práticos, não aconselhamento jurídico. LGPD
(Lei 13.709/2018), GDPR (Reg. UE 2016/679) e CCPA/CPRA dão a você o direito
de pedir acesso e eliminação dos seus dados — exercer esse direito é legítimo.
Use os dados **apenas dos seus próprios identificadores**.
