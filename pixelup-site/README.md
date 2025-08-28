# PixelUp Site (moderno, com fallback de logo)

- `assets/pixelup-logo.webp` e `assets/pixelup-logo.png` (fallback).
- `index.html` usa `<picture>` para exibir a logo em **webp** com fallback **png**.
- `og:image` aponta para PNG (melhor compatibilidade).

## Publicação
1) Suba os arquivos **na raiz do repositório** (ver `index.html` + pasta `assets/`).
2) Na Vercel: *Other/Static*, Output Directory vazio, **Deploy**.
