# 🚀 Guia de Deployment Remoto - EvoluaMD

## Opções Disponíveis

### 1. **GitHub Pages** (RECOMENDADO - Gratuito & Fácil)
- ✅ Gratuito
- ✅ URL automática
- ✅ HTTPS incluído
- ✅ Sincroniza automaticamente com GitHub

**URL Final:** `https://brinersf.github.io/EvoluaMD`

---

### 2. **Vercel** (Alternativa - Mais Rápida)
- ✅ Gratuito
- ✅ Deploy automático do Git
- ✅ Domínio customizável
- ✅ Performance excelente

**URL Final:** `https://evoluamd.vercel.app` (ou customizada)

---

### 3. **Netlify** (Alternativa - Fácil)
- ✅ Gratuito
- ✅ Interface visual
- ✅ Deploy automático
- ✅ CMS integrado

**URL Final:** `https://evoluamd.netlify.app` (ou customizada)

---

## 📝 Configuração Passo a Passo

### **Opção 1: GitHub Pages (MAIS SIMPLES)**

#### Passo 1: Preparar o Repositório
```bash
cd /workspaces/EvoluaMD
git add .
git commit -m "Deploy EvoluaMD v1.0"
git push origin main
```

#### Passo 2: Ativar GitHub Pages
1. Vá para: **GitHub.com → seu repositório → Settings**
2. Na esquerda, clique em **"Pages"**
3. Em "Source", selecione:
   - Branch: `main`
   - Pasta: `/root`
4. Clique em **Save**

#### Passo 3: Aguarde (1-2 minutos)
GitHub construirá e publicará automaticamente.

**Seu site estará em:** `https://brinersf.github.io/EvoluaMD`

---

### **Opção 2: Vercel (MAIS RÁPIDO)**

#### Passo 1: Instale Vercel CLI
```bash
npm install -g vercel
```

#### Passo 2: Deploy
```bash
cd /workspaces/EvoluaMD
vercel
```

#### Passo 3: Siga as Instruções
- Selecione sua conta GitHub
- Autorize a integração
- Aguarde o deploy

**Seu site estará em:** `https://evoluamd.vercel.app`

---

### **Opção 3: Netlify (MAIS VISUAL)**

#### Passo 1: Conecte no Netlify
1. Vá para: **https://app.netlify.com**
2. Clique em **"Add new site"**
3. Selecione **"Connect to Git"**
4. Escolha GitHub
5. Selecione o repositório `EvoluaMD`

#### Passo 2: Configurações
- **Build command:** (deixe em branco - não precisa)
- **Publish directory:** `public`

#### Passo 3: Deploy
Clique em **"Deploy site"** e aguarde!

**Seu site estará em:** `https://evoluamd.netlify.app`

---

## 🔗 Links Rápidos

| Plataforma | Comando | URL Esperada |
|---|---|---|
| **GitHub Pages** | `git push` | `https://brinersf.github.io/EvoluaMD` |
| **Vercel** | `vercel` | `https://evoluamd.vercel.app` |
| **Netlify** | Web | `https://evoluamd.netlify.app` |

---

## ✅ Checklist Final

- [ ] Código commitado no GitHub
- [ ] Repository é público
- [ ] Escolheu uma plataforma
- [ ] URL gerada
- [ ] Teste no navegador
- [ ] Compartilhe com sua equipe!

---

## 🎯 Próximos Passos

Após o deploy, você pode:

1. **Personalizar o Domínio** (opcional)
   - Conectar domínio customizado
   - Ex: `evoluamd.com.br`

2. **Adicionar SSL/HTTPS** (automático em todas)

3. **Monitorar Analytics** (Vercel e Netlify)

4. **Criar Versões** (use Git Tags)
   ```bash
   git tag -a v1.0.0 -m "Release v1.0.0"
   git push origin v1.0.0
   ```

---

## 🆘 Troubleshooting

**"Página não funciona após deploy?"**
- Verifique se `index.html` está em `/public`
- Confirme que não há `build` necessário (é apenas HTML)
- Limpe cache do navegador (Ctrl+Shift+Del)

**"GitHub Pages diz repositório privado?"**
- Vá em Settings → Make public
- Se usar plano gratuito, precisa ser público

**"Vercel pergunta sobre build?"**
- Deixe "Build Command" em branco
- "Output Directory" pode ser `public`

---

## 📞 Compartilhando com sua Equipe

Após publicar, compartilhe o link:

```
🏥 EvoluaMD - Sistema de Evolução Clínica

Acesse: https://brinersf.github.io/EvoluaMD

Funcionalidades:
✅ Registro de evolução do paciente
✅ Exame físico com sistemas
✅ Medicações e exames lab
✅ Reconhecimento de voz (ditação)
✅ Exportar para texto

Precisa de algo? Abra uma issue no GitHub!
```

---

**Dúvidas? Veja os READMEs específicos:**
- [GitHub Pages Docs](https://docs.github.com/pt/pages)
- [Vercel Docs](https://vercel.com/docs)
- [Netlify Docs](https://docs.netlify.com/)
