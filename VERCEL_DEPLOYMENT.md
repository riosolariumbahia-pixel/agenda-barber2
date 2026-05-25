# Barberflow Pro - SaaS de Agendamento para Barbearias

Sistema completo de agendamento para barbearias com suporte a múltiplos usuários.

## 🚀 Deploy no Vercel

Este projeto foi configurado para fazer deploy no Vercel com sucesso.

### ✅ Alterações Realizadas

#### 1. Dependências Atualizadas
- **Removido**: Vite, TanStack Start, Cloudflare Vite Plugin
- **Adicionado**: Next.js 15.1.3 (framework Vercel-ready)
- **Mantidas**: Todas as libs de UI (Radix UI, React Query, Tailwind, etc.)

#### 2. Configurações Criadas
- ✅ `next.config.mjs` - Configuração Next.js otimizada
- ✅ `tsconfig.json` - TypeScript para Next.js
- ✅ `tailwind.config.ts` - Tailwind CSS
- ✅ `postcss.config.ts` - PostCSS
- ✅ `eslint.config.js` - ESLint
- ✅ `.prettierrc.json` - Code formatting
- ✅ `vercel.json` - Build Vercel
- ✅ `.vercelignore` - Arquivos ignorados

#### 3. Requisitos
- Node.js >= 18.17.0
- npm ou yarn

---

## 📋 Como Fazer Deploy

### 1️⃣ Local - Testar Antes
```bash
# Clone a branch
git checkout vercel-deploy

# Instale as dependências
npm install

# Teste o desenvolvimento
npm run dev

# Teste o build
npm run build
npm start
```

### 2️⃣ Deploy no Vercel
```bash
# Opção 1: CLI Vercel
npm i -g vercel
vercel login
vercel

# Opção 2: Dashboard Vercel
# 1. Acesse https://vercel.com
# 2. Clique "Add New" → "Project"
# 3. Selecione riosolariumbahia-pixel/agenda-barber2
# 4. Selecione branch: vercel-deploy
# 5. Configure variáveis de ambiente (se necessário)
# 6. Clique "Deploy"
```

---

## 🔧 Variáveis de Ambiente

Se seu SaaS usa Supabase, crie arquivo `.env.local`:

```env
NEXT_PUBLIC_SUPABASE_URL=your_url_here
NEXT_PUBLIC_SUPABASE_ANON_KEY=your_key_here
```

No Vercel Dashboard → Settings → Environment Variables, adicione as mesmas variáveis.

---

## 📁 Estrutura do Projeto

```
agenda-barber2/
├── src/
│   ├── pages/          # Páginas Next.js (Rotas)
│   ├── components/     # Componentes React
│   ├── utils/          # Funções utilitárias
│   └── types/          # Tipos TypeScript
├── public/             # Assets estáticos
├── package.json
├── next.config.mjs
├── tsconfig.json
├── tailwind.config.ts
└── vercel.json
```

---

## 🎯 Comandos Disponíveis

```bash
npm run dev        # Desenvolvimento local
npm run build      # Build para produção
npm start          # Inicia servidor produção
npm run lint       # Valida código
npm run format     # Formata código
```

---

## ✨ Benefícios do Vercel

- ⚡ Deploy automático (push → live)
- 🌍 Edge Functions + CDN global
- 🔄 Preview URLs para PRs
- 📊 Analytics automático
- 🔐 HTTPS gratuito
- 💬 Suporte integrado

---

## 🎉 Pronto para Deploy!

Sua aplicação está pronta para ser publicada no Vercel. Siga os passos acima e seu SaaS estará online em minutos!
