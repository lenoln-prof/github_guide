# 📊 Diagramas Visuais - Conceitos Git/GitHub

## 1️⃣ O Fluxo Básico do Git

```
┌─────────────────────────────────────────────────────────────┐
│                                                             │
│              SEU COMPUTADOR          │      GITHUB          │
│              ─────────────────────────────────────────      │
│                                      │                      │
│   ┌──────────────────────┐           │   ┌───────────────┐  │
│   │  Seus Arquivos       │           │   │  Repositório  │  │
│   │  (Área de Trabalho)  │           │   │  (Online)     │  │
│   └──────────┬───────────┘           │   └───────────────┘  │
│              │                       │          ▲           │
│              │ git add               │          │           │
│              ▼                       │          │ git pull  │
│   ┌──────────────────────┐           │          │           │
│   │   Index (Staging)    │           │          │           │
│   │  (Preparação)        │           │   git push           │
│   └──────────┬───────────┘           │          │           │
│              │                       │          ▼           │
│              │ git commit            │   ┌───────────────┐  │
│              ▼                       │   │  Servidor     │  │
│   ┌──────────────────────┐           │   │  GitHub       │  │
│   │   Local Repository   │─────────► │   └───────────────┘  │
│   │  (.git folder)       │           │                      │
│   └──────────────────────┘           │                      │
│                                      │                      │
│      git push origin main ──────────►                       │
│                                      │                      │
└─────────────────────────────────────────────────────────────┘
```

---

## 2️⃣ Ciclo de Vida do Arquivo no Git

```
┌─────────────┐
│ Arquivo     │
│ Novo/       │
│ Modificado  │
└──────┬──────┘
       │
       │ git add
       ▼
┌─────────────────┐
│  STAGED         │
│  (Preparado)    │
│  Pronto para    │
│  commit         │
└──────┬──────────┘
       │
       │ git commit
       ▼
┌─────────────────┐
│  COMMITTED      │
│  (Confirmado)   │
│  No repositório │
│  local          │
└──────┬──────────┘
       │
       │ git push
       ▼
┌─────────────────┐
│  PUSHED         │
│  (Enviado)      │
│  No GitHub      │
└─────────────────┘
```

---

## 3️⃣ Primeira Vez: Setup Completo

```
┌──────────────────────────────────────────────────────────┐
│  1. Criar Conta                                          │
│     ├─ Ir para github.com                                │
│     ├─ Clicar "Sign up"                                  │
│     ├─ Preencher formulário                              │
│     └─ Verificar email                                   │
└────────────────┬─────────────────────────────────────────┘
                 │
┌────────────────▼─────────────────────────────────────────┐
│  2. Criar Repositório                                    │
│     ├─ Clicar "New repository"                           │
│     ├─ Escolher nome                                     │
│     ├─ Selecionar Público/Privado                        │
│     └─ Criar repositório                                 │
└────────────────┬─────────────────────────────────────────┘
                 │
┌────────────────▼─────────────────────────────────────────┐
│  3. Instalar Git                                         │
│     ├─ Baixar de git-scm.com                             │
│     ├─ Executar instalador                               │
│     └─ Verificar: git --version                          │
└────────────────┬─────────────────────────────────────────┘
                 │
┌────────────────▼─────────────────────────────────────────┐
│  4. Configurar Git                                       │
│     ├─ git config --global user.name                     │
│     └─ git config --global user.email                    │
└────────────────┬─────────────────────────────────────────┘
                 │
┌────────────────▼─────────────────────────────────────────┐
│  5. Criar Personal Access Token                          │
│     ├─ GitHub > Settings > Developer settings            │
│     ├─ Personal access tokens (classic)                  │
│     ├─ Generate new token                                │
│     └─ COPIAR E GUARDAR                                  │
└────────────────┬─────────────────────────────────────────┘
                 │
┌────────────────▼─────────────────────────────────────────┐
│  6. Pronto para Usar!                                    │
│     ├─ Clonar repositório                                │
│     └─ Começar a trabalhar                               │
└──────────────────────────────────────────────────────────┘
```

---

## 4️⃣ Usando o Git - Ciclo Repetido

```
     ╔═════════════════════════════════════════════════════╗
     ║           CICLO DE DESENVOLVIMENTO                  ║
     ╠═════════════════════════════════════════════════════╣
     ║                                                     ║
     ║  ┌────────────────────────────────────────────┐     ║
     ║  │  1. Editar Arquivos                        │     ║
     ║  │     (use seu editor favorito)              │     ║
     ║  └────────────────┬─────────────────────────┬─┘     ║
     ║                   │                         │       ║
     ║                   ▼                         │       ║
     ║  ┌────────────────────────────────────────┐ │       ║
     ║  │  2. git add .                          │ │       ║
     ║  │     (preparar mudanças)                │ │       ║
     ║  └────────────────┬──────────────────────┬┘ │       ║
     ║                   │                      │  │       ║
     ║                   ▼                      │  │       ║
     ║  ┌────────────────────────────────────┐  │  │       ║
     ║  │  3. git commit -m "mensagem"       │  │  │       ║
     ║  │     (confirmar mudanças)           │  │  │       ║
     ║  └────────────────┬──────────────────┬┘  │  │       ║
     ║                   │                  │   │  │       ║
     ║                   ▼                  │   │  │       ║
     ║  ┌────────────────────────────────┐  │   │  │       ║
     ║  │  4. git push origin main       │  │   │  │       ║
     ║  │                ▼               │  │   │  │       ║
     ║  │     (enviar para GitHub)       │  │   │  │       ║
     ║  └────────────────┬───────────────┘  │   │  │       ║
     ║                   │                  │   │  │       ║
     ║           ✅ Enviado!                │   │  │       ║
     ║                                      │   │  │       ║
     ║  Voltar ao passo 1?                  │   │  │       ║
     ║  ───────────────────────────────────►┴───┘──┘       ║
     ║                                                     ║
     ╚═════════════════════════════════════════════════════╝
```

---

## 5️⃣ Estrutura de Pastas Recomendada

```
meu-projeto/
│
├── README.md               ← Descrição do projeto
├── LICENSE                 ← Licença do projeto
├── .gitignore              ← Arquivos a ignorar
│
├── src/                    ← Código-fonte
│   ├── main.py
│   ├── utils.py
│   └── config.py
│
├── docs/                   ← Documentação
│   ├── guia.md
│   ├── tutorial.md
│   └── API.md
│
├── dados/                  ← Dados do projeto
│   ├── entrada.csv
│   └── saida.json
│
├── testes/                 ← Testes
│   ├── test_main.py
│   └── test_utils.py
│
└── .git/                   ← Pasta do Git (automática)
    └── (histórico interno)
```

---

## 6️⃣ O que Enviar vs O que NÃO Enviar

```
┌─────────────────────────────────────────────────────────┐
│  ✅ ENVIAR PARA GITHUB                                  │
├─────────────────────────────────────────────────────────┤
│  ✓ Código-fonte (.py, .js, .java, .cpp, etc)           │
│  ✓ README.md e documentação                             │
│  ✓ Dados públicos e não confidenciais                   │
│  ✓ Arquivos de configuração públicos                    │
│  ✓ Testes e scripts de build                            │
│  ✓ Arquivos de licença                                  │
└─────────────────────────────────────────────────────────┘

┌─────────────────────────────────────────────────────────┐
│  ❌ NÃO ENVIAR PARA GITHUB                              │
├─────────────────────────────────────────────────────────┤
│  ✗ Senhas e chaves de API                               │
│  ✗ Arquivo .env com dados sensíveis                     │
│  ✗ node_modules/, __pycache__, venv/                    │
│  ✗ Arquivos temporários e de cache                      │
│  ✗ Dados pessoais ou confidenciais                      │
│  ✗ Certificados SSL privados                            │
│  ✗ Tokens de autenticação                               │
│  ✗ Arquivos de sistema (.DS_Store, Thumbs.db)           │
│  ✗ Arquivos compilados grandes                          │
└─────────────────────────────────────────────────────────┘
```

---

## 7️⃣ Autenticação - Fluxo Seguro

```
┌──────────────────────────────────┐
│  Você vai fazer push             │
└────────────┬─────────────────────┘
             │
             ▼
┌──────────────────────────────────────┐
│  Git pede autenticação               │
│  Username: ?                         │
│  Password: ?                         │
└────────────┬─────────────────────────┘
             │
             ├─────────────────┬─────────────────┐
             │                 │                 │
             ▼                 ▼                 ▼
    ❌ Senha Normal   ✅ Token de Acesso  ✅ SSH Key
    (Não funciona)    (Recomendado)       (Avançado)
                           │
                           ▼
                  ┌─────────────────────┐
                  │ username: seu-user  │
                  │ password: ghp_xxxx  │
                  └─────────┬───────────┘
                            │
                            ▼
                       ✅ Acesso!
```

---

## 8️⃣ Anatomia de um Commit

```
┌─────────────────────────────────────────────────────────┐
│  git commit -m "Adiciona função de login"               │
│  ───┬──────────────┬─────────────────────────────────── │
│     │              │                                    │
│  Comando        Mensagem (imperativo, clara)            │
│                                                         │
│  O que é enviado:                                       │
│  ┌─────────────────────────────────────────────────┐    │
│  │ Commit: abc123def456                            │    │
│  │ Author: João Silva <joao@email.com>             │    │
│  │ Date:   Mon Apr 14 23:24:00 2024 +0000          │    │
│  │                                                 │    │
│  │ Adiciona função de login                        │    │
│  │                                                 │    │
│  │ Mudanças:                                       │    │
│  │  src/index.html      (modificado)               │    │
│  │  src/style.css     (novo)                       │    │
│  │  docs/API.md      (modificado)                  │    │
│  └─────────────────────────────────────────────────┘    │
│                                                         │
└─────────────────────────────────────────────────────────┘
```

---

## 9️⃣ Estados do Arquivo

```
                    NOVO ARQUIVO
                         │
                         ▼
    ┌────────────────────────────────────┐
    │  UNTRACKED                         │
    │  (Git não acompanha)               │
    └────────────────┬───────────────────┘
                     │ git add
                     ▼
    ┌────────────────────────────────────┐
    │  STAGED                            │
    │  (Pronto para commit)              │
    └────────────────┬───────────────────┘
                     │ git commit
                     ▼
    ┌────────────────────────────────────┐
    │  COMMITTED                         │
    │  (No repositório local)            │
    └────────────────┬───────────────────┘
                     │ git push
                     ▼
    ┌────────────────────────────────────┐
    │  PUSHED                            │
    │  (No GitHub)                       │
    └────────────────────────────────────┘

    ──────────────────────────────────────

                  ARQUIVO MODIFICADO
                         │
                         ▼
    ┌────────────────────────────────────┐
    │  MODIFIED                          │
    │  (Mudança não preparada)           │
    └────────────────┬───────────────────┘
                     │ git add
                     ▼
    ┌────────────────────────────────────┐
    │  STAGED                            │
    │  (Mudança preparada)               │
    └────────────────┬───────────────────┘
                     │ git commit
                     ▼
    ┌────────────────────────────────────┐
    │  COMMITTED                         │
    │  (Mudança confirmada)              │
    └────────────────────────────────────┘
```

---

## 🔟 Comparando: Git vs GitHub

```
┌─────────────────────────────────────────────────────────┐
│                     GIT                                 │
├─────────────────────────────────────────────────────────┤
│  • Software instalado no seu computador                 │
│  • Funciona offline                                     │
│  • Controla versões do código                           │
│  • Cria histórico de mudanças                           │
│  • Gerencia branches                                    │
│  • Usado via linha de comando                           │
│  • Gratuito e open source                               │
└─────────────────────────────────────────────────────────┘

┌─────────────────────────────────────────────────────────┐
│                   GITHUB                                │
├─────────────────────────────────────────────────────────┤
│  • Serviço online (na nuvem)                            │
│  • Requer internet para funcionar                       │
│  • Armazena repositórios remotamente                    │
│  • Interface web visual                                 │
│  • Facilita colaboração entre pessoas                   │
│  • Plano gratuito + planos pagos                        │
│  • Oferece CI/CD, issues, pull requests                 │
│  • GitHub Pages para sites                              │
└─────────────────────────────────────────────────────────┘

┌─────────────────────────────────────────────────────────┐
│          GIT + GITHUB JUNTOS = PERFEITO                 │
├─────────────────────────────────────────────────────────┤
│  ✓ Git faz a gestão local                               │
│  ✓ GitHub armazena na nuvem                             │
│  ✓ Push = Git → GitHub                                  │
│  ✓ Pull = GitHub → Git                                  │
│  ✓ Backup automático                                    │
│  ✓ Colaboração fácil                                    │
│  ✓ Histórico seguro                                     │
└─────────────────────────────────────────────────────────┘
```

---

## Conclusão

Estes diagramas cobrem os conceitos visuais principais. 
Para mais detalhes, consulte o **guia_github_iniciantes.md**!