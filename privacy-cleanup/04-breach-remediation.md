# Passo 6 — Limpar vazamentos de dados

Seu e-mail provavelmente vazou em lugares que você nem lembra. 20 minutos de
trabalho, 10 anos de proteção.

## 1. Verificar (só você consegue fazer)

Não consigo rodar isto por você — o HIBP exige confirmação no seu e-mail.

1. Acesse `https://haveibeenpwned.com` e teste os **dois** e-mails:
   - `ian.gallina@gmail.com`
   - `redspell84@hotmail.com`
2. Em `https://haveibeenpwned.com/Passwords` teste padrões de senha que você
   reutilizou (a checagem é por hash k-anonimato — seguro).
3. Ative o **Notify me** (`haveibeenpwned.com/NotifyMe`) nos dois e-mails
   para ser avisado de vazamentos futuros.
4. Cheque também: `https://monitor.mozilla.org` e, no Google,
   `myactivity.google.com` → "Resultados sobre você" / Dark Web report.

## 2. Me mande a lista — eu priorizo

Cole aqui a lista de breaches que o HIBP retornar (nome do site + ano + o que
vazou). Eu devolvo a ordem de ação por risco atual, classificando cada um em:

- **Trocar senha** (só credencial vazou, conta ainda útil)
- **Trocar senha + ativar 2FA** (conta sensível: e-mail, banco, financeiro)
- **Excluir a conta** (serviço morto/inútil — vai pro Passo 3)

Prompt que vou aplicar:

> "Olhe esta lista de breaches [colada]. Ordem de prioridade: troca de
> senha, configuração de 2FA, ou exclusão de conta? Classifique pelo risco
> atual, considerando dado vazado, sensibilidade da conta e reuso de senha."

## 3. Regras de remediação (faça em paralelo)

- **Senha única por site.** Use gerenciador (Bitwarden, 1Password, ou o do
  navegador). Nunca reutilize — vazamento de um vira invasão de vários.
- **Prioridade máxima:** os e-mails em si. Se `ian.gallina@gmail.com` ou
  `redspell84@hotmail.com` cair, tudo ligado a eles cai. Senha forte e
  única + 2FA já.
- **2FA em tudo que importa**, preferindo app autenticador (TOTP) ou
  **passkey/chave física** em vez de SMS (SMS é vulnerável a SIM-swap).
- **Senhas comprometidas primeiro:** troque todas as que o HIBP/gerenciador
  marcar como vazadas ou reutilizadas.
- **E-mail antigo:** se `redspell84@hotmail.com` não é mais usado, não
  abandone — ele ainda é chave de recuperação de contas antigas. Recupere o
  acesso, faça o inventário (Passo 3) e só então decida desativar.
- **Alertas:** ative aviso de novo login/dispositivo em e-mail e banco.

## 4. Verificação final

- [ ] HIBP rodado nos 2 e-mails + Notify me ativo
- [ ] Lista de breaches enviada para priorização
- [ ] Senhas vazadas/reutilizadas trocadas (únicas, no gerenciador)
- [ ] 2FA (app/passkey) nas contas-chave: e-mails, banco, financeiro, GitHub
- [ ] Contas inúteis de sites vazados → enfileiradas no Passo 3
