# Seus dados — NÃO preencha dados reais aqui

> 🛑 **Este arquivo é versionado e vai para um PR público. NÃO coloque
> CPF, endereço, telefone ou nome completo real aqui.** Esta é a versão
> de modelo, intencionalmente só com placeholders.

## Como usar (fluxo seguro)

1. Copie este arquivo para `_SEUS-DADOS.local.md` (mesma pasta).
2. O `.gitignore` já bloqueia `_SEUS-DADOS.local.md` e `*.local.md` — esse
   arquivo **nunca** é versionado nem enviado.
3. Preencha seus dados reais **apenas** no `.local.md`.
4. Ao montar um template, copie os valores do `.local.md` na hora de
   enviar. Não cole dado real em nenhum arquivo rastreado.

```sh
cp privacy-cleanup/templates/_SEUS-DADOS.md \
   privacy-cleanup/templates/_SEUS-DADOS.local.md
git check-ignore privacy-cleanup/templates/_SEUS-DADOS.local.md  # deve listar o caminho
```

## Estrutura (só placeholders — preencha no `.local.md`)

| Campo | Valor | Status |
|---|---|---|
| Nome completo legal | `[NOME COMPLETO]` | preencher no .local |
| E-mail principal | `ian.gallina@gmail.com` | público (ok) |
| E-mail secundário/antigo | `redspell84@hotmail.com` | público (ok) |
| Cidade/UF/País | `Brasília, DF, Brasil` | público (ok) |
| Endereço postal completo | `[NÃO AQUI — só no .local]` | sensível |
| Telefone | `[NÃO AQUI — só no .local]` | sensível |
| CPF | `[NÃO AQUI — só no .local]` | **sensível** |
| LinkedIn | `https://www.linkedin.com/in/ian-gallina` | público (ok) |
| Identificador do broker | (ex.: URL do perfil ZoomInfo) | por caso |

## Princípio da minimização

Na maioria dos pedidos LGPD/GDPR/CCPA, **e-mail + nome bastam** para
identificação. Só inclua CPF/endereço se a empresa exigir explicitamente
para verificação, e por canal seguro. Nunca anexe documento a e-mail aberto
sem necessidade.
