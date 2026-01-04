# 🚀 Como fazer Deploy na Vercel

## Método 1: Via Interface Web (Mais Fácil)

### Passo 1: Preparar o Repositório
1. Crie um repositório no GitHub/GitLab/Bitbucket
2. Faça commit e push do projeto:
```bash
git init
git add .
git commit -m "Initial commit - Simulador Prospere"
git branch -M main
git remote add origin [URL_DO_SEU_REPOSITORIO]
git push -u origin main
```

### Passo 2: Deploy na Vercel
1. Acesse: https://vercel.com
2. Faça login (pode usar GitHub)
3. Clique em **"Add New Project"** ou **"Import Project"**
4. Importe o repositório que você criou
5. Configure:
   - **Framework Preset:** Vite
   - **Root Directory:** `./`
   - **Build Command:** `npm run build`
   - **Output Directory:** `dist`
6. Clique em **"Deploy"**

### Passo 3: Aguardar
- A Vercel vai instalar dependências e fazer build automaticamente
- Em 2-3 minutos seu site estará no ar!

---

## Método 2: Via CLI (Terminal)

### Passo 1: Instalar Vercel CLI
```bash
npm install -g vercel
```

### Passo 2: Login
```bash
vercel login
```

### Passo 3: Deploy
```bash
cd /Users/prospere/Desktop/teste-simulador
vercel
```

Siga as instruções:
- **Set up and deploy?** → `Y`
- **Which scope?** → Escolha sua conta
- **Link to existing project?** → `N` (primeira vez)
- **Project name?** → `simulador-prospere` (ou o nome que preferir)
- **Directory?** → `./`
- **Override settings?** → `N`

### Passo 4: Deploy de Produção
```bash
vercel --prod
```

---

## ⚙️ Configurações Importantes

O arquivo `vercel.json` já está configurado para:
- ✅ Build automático com Vite
- ✅ Output correto (`dist`)
- ✅ SPA routing (redirecionamento para index.html)

---

## 🔗 Após o Deploy

Você receberá uma URL tipo:
- `https://simulador-prospere.vercel.app`
- Ou URL customizada se configurar domínio

---

## 📝 Comandos Úteis

```bash
# Ver status do deploy
vercel ls

# Ver logs
vercel logs

# Ambiente de desenvolvimento
vercel dev
```

---

## ✨ Dicas

1. **Variáveis de Ambiente**: Se precisar, configure em Settings → Environment Variables
2. **Domínio Customizado**: Em Settings → Domains
3. **Deploy Automático**: Cada push no GitHub faz novo deploy automaticamente
4. **Preview Deploys**: Cada PR cria um preview URL para testar

---

**Pronto! Seu simulador estará no ar em minutos! 🎉**