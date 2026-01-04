# 🚀 GUIA SIMPLES - Deploy na Vercel

## ⚡ Método MAIS FÁCIL (Sem Terminal)

### Passo 1: Criar conta no GitHub (se não tiver)
1. Acesse: https://github.com
2. Crie uma conta ou faça login

### Passo 2: Criar repositório no GitHub
1. Clique no botão **"+"** no canto superior direito
2. Escolha **"New repository"**
3. Nome: `simulador-prospere`
4. Deixe **público** ou privado (não importa)
5. **NÃO** marque "Add README" ou outros
6. Clique em **"Create repository"**

### Passo 3: Fazer upload dos arquivos
**Opção A - Via GitHub Web:**
1. Na página do repositório, clique em **"uploading an existing file"**
2. Arraste TODA a pasta `teste-simulador` (exceto `node_modules`)
3. Clique em **"Commit changes"**

**Opção B - Via Terminal (se preferir):**
```bash
cd /Users/prospere/Desktop/teste-simulador
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/SEU_USUARIO/simulador-prospere.git
git push -u origin main
```

### Passo 4: Deploy na Vercel
1. Acesse: **https://vercel.com**
2. Clique em **"Sign Up"** ou **"Log In"**
3. Escolha **"Continue with GitHub"**
4. Autorize a Vercel a acessar seus repositórios
5. Clique em **"Add New Project"**
6. Selecione o repositório `simulador-prospere`
7. Clique em **"Import"**
8. **NÃO PRECISA MUDAR NADA** - a Vercel detecta Vite automaticamente
9. Clique em **"Deploy"**
10. Aguarde 2-3 minutos

### Passo 5: Pronto! 🎉
Você receberá uma URL tipo: `https://simulador-prospere.vercel.app`

---

## 🔧 Se der erro no build

### Erro comum: "Build failed"

**Solução:**
1. Na Vercel, vá em **Settings** → **General**
2. Em **Build & Development Settings**, verifique:
   - **Framework Preset:** Vite
   - **Build Command:** `npm run build`
   - **Output Directory:** `dist`
   - **Install Command:** `npm install`

---

## 📱 Método Alternativo: Vercel CLI

Se preferir usar terminal:

```bash
# 1. Instalar Vercel CLI
npm install -g vercel

# 2. Ir para a pasta do projeto
cd /Users/prospere/Desktop/teste-simulador

# 3. Fazer login
vercel login

# 4. Deploy
vercel

# Responda:
# - Set up and deploy? → Y
# - Which scope? → Sua conta
# - Link to existing? → N
# - Project name? → simulador-prospere
# - Directory? → ./
# - Override settings? → N

# 5. Deploy produção
vercel --prod
```

---

## ❓ Problemas Comuns

### "Cannot find module"
**Solução:** Certifique-se que `package.json` está correto

### "Build command failed"
**Solução:** Verifique se todas as dependências estão no `package.json`

### "404 Not Found" após deploy
**Solução:** O arquivo `vercel.json` já está configurado para SPA routing

---

## 🆘 Precisa de ajuda?

Me diga qual erro apareceu ou em qual passo travou que eu ajudo!
