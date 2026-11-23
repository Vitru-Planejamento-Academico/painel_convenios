# Painel de Convênios

Página estática (um único `index.html`, sem dependências externas) publicada via GitHub Pages.

## Publicar

```sh
git init -b main
git add .
git commit -m "Publica painel de convênios"
git remote add origin https://github.com/<usuario>/<repo>.git
git push -u origin main
```

No GitHub: **Settings → Pages → Build and deployment → Deploy from a branch → `main` / `/ (root)`**.
O site fica em `https://<usuario>.github.io/<repo>/`.

## Observações

- `index.html` tem ~53 MB. O GitHub avisa acima de 50 MB e bloqueia acima de 100 MB por arquivo.
- `.nojekyll` desativa o processamento Jekyll (o arquivo é servido como está).
- Os dados vêm criptografados dentro da página; a Web Crypto API exige HTTPS, que o GitHub Pages fornece.
