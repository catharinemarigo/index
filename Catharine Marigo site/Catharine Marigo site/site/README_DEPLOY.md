# Catharine Marigo — Site estático para Vercel

## O que trocar antes de publicar

1. Abra `index.html`.
2. Procure por `WHATSAPP_NUMBER`.
3. Troque `5500000000000` pelo WhatsApp real no formato país + DDD + número, sem espaços.
4. No rodapé, troque `CRM/UF: inserir`, endereço e telefone.
5. Se o domínio final não for `catharinemarigo.com.br`, troque o domínio em:
   - `<link rel="canonical">`
   - meta `og:url`
   - JSON-LD
   - `robots.txt`
   - `sitemap.xml`

## Deploy pelo GitHub + Vercel

1. Crie um repositório no GitHub, por exemplo: `catharine-marigo-site`.
2. Abra o GitHub Desktop.
3. Use `File > Add local repository` e selecione esta pasta.
4. Faça `Commit to main`.
5. Clique em `Publish repository`.
6. Entre em https://vercel.com.
7. Clique em `Add New > Project`.
8. Importe o repositório do GitHub.
9. Framework Preset: `Other`.
10. Build Command: deixe vazio.
11. Output Directory: deixe vazio ou use `.`.
12. Clique em `Deploy`.

## Deploy direto pela Vercel CLI

```bash
npm i -g vercel
cd catharine_marigo_site
vercel
vercel --prod
```

## Estrutura

- `index.html`: página completa.
- `assets/`: fotos, logomarca e favicon.
- `vercel.json`: headers e cache.
- `robots.txt` e `sitemap.xml`: SEO básico.
- `manifest.webmanifest`: instalação como atalho/PWA simples.
