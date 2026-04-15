# 🚀 Referência Rápida - Comandos Git Essenciais

## ⚡ Workflow Básico (Copie e Cole)

```bash
# 1. Entre na pasta do repositório
cd caminho/do/seu/repositorio

# 2. Veja o status
git status

# 3. Adicione todos os arquivos
git add .

# 4. Confirme as mudanças
git commit -m "Descrição do que mudou"

# 5. Envie para o GitHub
git push origin main
```

---

## 📋 Comandos Essenciais

### Configuração Inicial
```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu.email@exemplo.com"
git config --global --list          # Verificar configurações
```

### Clonar Repositório
```bash
git clone https://github.com/usuario/repositorio.git
```

### Ver Situação
```bash
git status                          # Ver arquivos modificados
git log                             # Ver histórico de commits
git diff                            # Ver mudanças detalhadas
```

### Adicionar e Confirmar
```bash
git add .                           # Adicionar todos os arquivos
git add nome-do-arquivo.txt         # Adicionar arquivo específico
git commit -m "Mensagem do commit"  # Confirmar mudanças
```

### Enviar e Receber
```bash
git push origin main                # Enviar para GitHub
git pull origin main                # Baixar do GitHub
```

### Verificar Conexão
```bash
git remote -v                       # Ver repositório remoto conectado
```

---

## 📝 Exemplos de Mensagens de Commit

### ✅ Boas Mensagens
```bash
git commit -m "Adiciona função de login"
git commit -m "Corrige bug na validação"
git commit -m "Atualiza documentação README"
git commit -m "Remove arquivo desnecessário"
git commit -m "Integra API de pagamento"
```

### ❌ Ruim - EVITE
```bash
git commit -m "alterações"
git commit -m "teste"
git commit -m "ajustes"
git commit -m "mudanças"
```

---

## 🔐 Autenticação

### Primeira Vez
Quando fazer `git push`, será pedido:
```
Username: seu-usuario-github
Password: colar o Personal Access Token (não a senha!)
```

### Salvar Credenciais (Opcional)
```bash
git config --global credential.helper store
```
Depois de autenticar uma vez, o Git lembrará nos próximos pushes.

---

## 🆘 Erros Comuns - Soluções Rápidas

### "fatal: not a git repository"
```bash
# Você não está na pasta certa
cd caminho/correto/da/pasta
```

### "Permission denied"
```bash
# Verifique seu Personal Access Token
# Vá para: https://github.com/settings/tokens
```

### "Your branch is ahead"
```bash
git push origin main
```

### "nothing to commit"
```bash
# Você não fez alterações ou já fez commit
git status  # Verifique o status
```

---

## 📂 Estrutura Recomendada

```
meu-projeto/
├── README.md          # Descrição do projeto
├── src/               # Código-fonte
│   ├── main.py
│   └── utils.py
├── dados/             # Dados
├── docs/              # Documentação
└── .gitignore         # Arquivos a não enviar
```

---

## 🎯 Checklist Antes de Fazer Push

- [ ] Testei meu código localmente?
- [ ] Verifiquei com `git status`?
- [ ] Adicionei os arquivos com `git add`?
- [ ] Fiz commit com mensagem clara?
- [ ] Não estou enviando arquivos confidenciais?
- [ ] Meu Personal Access Token está válido?

---

## 🔗 Links Úteis

- **GitHub**: https://github.com
- **Criar Token**: https://github.com/settings/tokens
- **Docs**: https://docs.github.com/pt
- **Git Book**: https://git-scm.com/book/pt-br/v2

---

## 💬 Dúvidas Comuns

**P: Qual a diferença entre add, commit e push?**
```
add    = Preparar arquivos
commit = Confirmar mudanças
push   = Enviar para GitHub
```

**P: Posso remover um commit?**
```
Sim, mas é avançado. Consulte docs para revert ou reset.
```

**P: Perdi meus arquivos locais!**
```bash
git clone https://github.com/usuario/repositorio.git
```

**P: Esqueci o que alterei?**
```bash
git diff
```

---

## 🎓 Próximos Passos para Aprender

1. **Branches**: Trabalhar em versões paralelas
2. **Merge**: Combinar branches
3. **Pull Requests**: Contribuir em projetos
4. **Stash**: Guardar mudanças temporariamente
5. **Rebase**: Reorganizar commits

---

*Imprima ou salve esta página nos favoritos para referência rápida!*