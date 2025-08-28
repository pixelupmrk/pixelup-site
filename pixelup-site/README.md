# PixelUp Site (estático)

Site estático pronto para deploy na **Vercel**.

## Estrutura
- `index.html` — página única com seções (Serviços, Cases, Depoimentos, Sobre, Contato) e WhatsApp flutuante.
- `assets/pixelup-logo.webp` — sua logo usada no topo e para Open Graph.
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
git commit -m "Inicial: site PixelUp com logo"

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
