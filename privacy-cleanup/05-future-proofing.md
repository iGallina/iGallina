# Passos 5 e 7 — Soterrar o que não some + prevenir vazamentos futuros

## Passo 5 — Se não dá pra apagar, soterre (reputação)

Quando um resultado não pode ser removido (artigo legítimo de terceiro,
registro que a empresa se recusa a apagar dentro da lei), a estratégia é
**empurrá-lo para baixo** publicando conteúdo legítimo e verdadeiro que você
controla e que rankeia melhor.

> Abordagem ética: isto é **criar conteúdo real e preciso sobre você**, não
> spam de SEO, cloaking ou fazenda de links. Conteúdo enganoso é
> contraproducente e pode violar termos de plataformas.

Ativos que você controla e que o Google prioriza para buscas pelo seu nome:

- Site/portfólio pessoal (domínio próprio com seu nome) — maior peso
- LinkedIn `/in/ian-gallina` (já existe — mantenha ativo e completo)
- GitHub `iGallina`, perfil de empresa, About.me
- Artigos técnicos no seu nome (dev.to, Medium, LinkedIn Articles) sobre
  Product Management / IA — alinhados ao seu posicionamento profissional

Prompt reutilizável (me peça quando quiser):

> "Com meu nome e profissão (Technical Product Manager / Senior PO, IA e
> automação), gere 5 ângulos de conteúdo legítimo e verdadeiro. Para cada
> um: título, palavras-chave do meu nome a reforçar, e onde publicar para
> rankear bem em buscas pelo meu nome."

Recursos legais de remoção (use antes de só soterrar):

- **Google — remover conteúdo desatualizado:** `templates/PT-google-conteudo-desatualizado.md`
- **Google — informações pessoais/doxxing:** `https://support.google.com/websearch/answer/9673730`
- **Direito ao esquecimento (LGPD/GDPR):** requisição ao site de origem
  (`templates/`), não só ao buscador.

Realista: soterramento leva ~2–3 meses para o Google reordenar. Comece já.

## Passo 7 — Prevenir vazamentos futuros

### E-mail por alias (pare de espalhar o e-mail real)

Em **todo cadastro novo**, use um alias descartável. Se vazar, você deleta o
alias e o e-mail real (`ian.gallina@gmail.com`) fica intocado — e você ainda
descobre **quem** vazou (cada serviço recebe um alias diferente).

- SimpleLogin, addy.io (anonaddy), Firefox Relay, ou **Apple Hide My Email**
  (se usa Apple) / **Gmail + DuckDuckGo Email Protection**.
- Truque grátis e imediato no Gmail: `ian.gallina+nomedosite@gmail.com` —
  ajuda a rastrear origem de spam (não esconde o e-mail base, mas já filtra).
- Aposente `redspell84@hotmail.com` para cadastros novos — só recuperação de
  contas antigas (Passo 3), depois desative.

### Navegador e rastreadores

- Use **Brave** ou **Firefox** (bloqueiam rastreadores por padrão; Chrome
  não). No Firefox: proteção "Rígida". Adicione uBlock Origin.
- Desligue ad personalization: `myadcenter.google.com`,
  `https://optout.aboutads.info`, `https://www.youronlinechoices.com`.

### Telefone e dados sensíveis

- Número secundário (eSIM/VoIP) para cadastros; o pessoal só para contatos
  reais e 2FA (preferindo app/passkey a SMS).
- Nunca preencha campos opcionais (endereço, data de nascimento, CPF) em
  cadastros que não exigem legalmente.

### Monitoramento contínuo (não é tarefa única)

- HIBP **Notify me** ativo nos dois e-mails.
- Google: "Resultados sobre você" + alerta de dark web (`myactivity.google.com`).
- Crie um **Google Alerts** para `"Ian Gallina"`.
- **A cada 90 dias:** repita as buscas de `01-exposure-audit.md` e revisite
  `02-data-broker-optout-list.md` — brokers re-coletam e te re-listam.
- Mantenha a planilha de controle (broker | data do pedido | status | re-checar).

### Higiene recorrente

- [ ] Aliases ativados; e-mail real fora de cadastros novos
- [ ] Navegador com bloqueio de rastreador + uBlock Origin
- [ ] Ad personalization desligada (Google + AdChoices)
- [ ] Google Alerts + HIBP Notify configurados
- [ ] Lembrete recorrente de re-auditoria a cada 90 dias
