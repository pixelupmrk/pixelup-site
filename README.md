# PixelUp Site (estático)

Site estático pronto para deploy na **Vercel**.

## Estrutura
- `index.html` — página única com seções (Serviços, Cases, Depoimentos, Sobre, Contato) e WhatsApp flutuante.
- `vercel.json` — config simples para URLs limpas.

## Como publicar (GitHub + Vercel)

### 1) Criar repositório e enviar os arquivos
```bash
# 1. Baixe e descompacte o ZIP
# 2. Entre na pasta
cd pixelup-site

# 3. Inicie Git e faça o primeiro commit
git init
git add .
git commit -m "Inicial: site PixelUp"

# 4. Crie um repositório no GitHub (no site) chamado pixelup-site
# 5. Conecte e envie
git branch -M main
git remote add origin https://github.com/<seu-usuario>/pixelup-site.git
git push -u origin main
```

### 2) Conectar na Vercel
1. Acesse https://vercel.com/import/git e conecte sua conta GitHub.
2. Selecione o repositório **pixelup-site**.
3. **Framework Preset**: *Other* (ou *Static*).  
4. **Output Directory**: deixe em branco (raiz).  
5. Clique em **Deploy**.

Pronto! Quando fizer novo commit na branch `main`, a Vercel publica automaticamente.

## Dicas
- Personalize textos/links dentro do `index.html` (WhatsApp, e-mail, og:url).
- Para páginas extras, crie novos arquivos `.html` na raiz (ex.: `politica.html`) e linke no menu/rodapé.
