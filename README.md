# SST Portugal — site estático

Site estático (HTML puro, sem build step) com a identidade "Dossier Técnico".

## Estrutura

```
index.html                          → homepage
formacao/construcao-civil.html      → artigo de formação, sector Construção Civil
vercel.json                         → URLs limpos (sem .html)
```

## Deploy no Vercel

**Opção A — arrastar a pasta (mais rápido, sem GitHub):**
1. Entra em vercel.com → New Project → "Deploy" → arrasta esta pasta inteira
2. Framework preset: escolher "Other" (não é Vite/Next, é HTML estático)
3. Build command: deixar vazio
4. Output directory: deixar vazio (raiz)
5. Deploy

**Opção B — via GitHub (recomendado para manter histórico, como o resto dos teus projectos):**
1. `git init && git add . && git commit -m "site inicial SST Portugal"`
2. Criar repo no GitHub (ex: `souzalrns/sst-portugal-site`) e fazer push
3. No Vercel: New Project → importar o repo → mesmas definições da Opção A
4. Auto-deploy fica activo a cada push, tal como o `viannalegal-site`

## Depois do primeiro deploy

- Ligar o domínio `sstportugal.pt` em Vercel → Settings → Domains
- Com `cleanUrls: true`, o link da homepage para o artigo (`/formacao/construcao-civil`) já funciona sem `.html`
- Novos artigos: criar `formacao/<sector>.html` e ligar o card correspondente na homepage da mesma forma que foi feito para Construção Civil

## Por fazer antes de publicar

- Substituir os `href="#"` do CTA/telefone por contactos reais
- Confirmar texto legal final com a Kathia
- Adicionar Google Analytics / Search Console quando o domínio estiver activo (mesmo processo já feito no ViannaLegal)
