# Passo 3 — Matar contas mortas

Todo fórum, app de teste e ferramenta antiga que você usou ainda guarda seus
dados. Foco especial: cadastros antigos sob `redspell84@hotmail.com` (handle
`redspell84`, era 2014±) e `ian.gallina@gmail.com`.

## Como achar todas as contas

1. **Have I Been Pwned** (Passo 6) — cada breach revela um site onde você
   tinha conta.
2. **Caixa de e-mail** — busque em ambos os e-mails por:
   `"welcome"`, `"confirm your account"`, `"verify your email"`,
   `"sua conta"`, `"redefinir senha"`, `"reset password"`.
3. **Gerenciador de senhas / "Senhas salvas"** do navegador e do Google
   (`passwords.google.com`) — lista direta de todo site com login salvo.
4. **"Login with Google/Facebook/Apple"** — revise apps de terceiros:
   - Google: `myaccount.google.com/connections`
   - Apple: `appleid.apple.com` → Sign in with Apple
5. **justdeleteme.xyz** — diretório com o nível de dificuldade de exclusão
   e link direto de cada serviço. Marque os piores.

## Exclusão de verdade ≠ desativar

Para cada conta, exija **exclusão permanente**, não desativação. Pergunte
sempre (prompt reutilizável — me mande por serviço):

> "Quero excluir minha conta no [SERVIÇO]. Qual é o processo de exclusão
> **permanente** (não apenas desativação)? O que acontece com backups e
> logs? Em quanto tempo os dados são apagados de fato? Há base legal para
> retenção parcial? Como confirmo por escrito que foi concluído?"

## Checklist por conta

- [ ] Localizar a opção de **exclusão definitiva** (não "desativar"/"pausar")
- [ ] Antes de apagar: baixar seus dados se quiser arquivo, e **trocar**
      e-mail/nome do perfil por valores neutros (alguns sistemas mantêm o
      último estado em backup por meses)
- [ ] Remover métodos de pagamento e dados de cobrança salvos
- [ ] Revogar acessos OAuth concedidos a/por esse serviço
- [ ] Solicitar exclusão; **guardar print + e-mail de confirmação**
- [ ] Se não houver opção de exclusão na interface → enviar requisição legal:
      - Site da UE/global → `templates/EN-GDPR-erasure-art17.md`
      - Empresa brasileira → `templates/PT-LGPD-eliminacao-art18.md`
      - Site dos EUA → `templates/EN-CCPA-opt-out.md`
- [ ] Re-checar em 30 dias se a conta realmente sumiu

## Prioridade de exclusão

1. Contas com **dados financeiros/documento** (pagamento, CPF, endereço).
2. Contas em sites com **histórico de vazamento** (cruzar com HIBP).
3. Contas com **dados pessoais públicos** (perfil, fotos, posts).
4. Cadastros triviais (newsletters, apps de teste) — em lote, por último.
