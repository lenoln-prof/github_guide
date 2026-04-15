# Guia Completo: GitHub para Iniciantes

## 📚 Sumário

1. [O que é GitHub?](#o-que-é-github)
2. [Criando uma Conta no GitHub](#criando-uma-conta-no-github)
3. [Criando seu Primeiro Repositório](#criando-seu-primeiro-repositório)
4. [Instalando o Git no Windows](#instalando-o-git-no-windows)
5. [Configurando o Git](#configurando-o-git)
6. [Criando um Personal Access Token](#criando-um-personal-access-token)
7. [Enviando Arquivos para o GitHub](#enviando-arquivos-para-o-github)
8. [Boas Práticas](#boas-práticas)
9. [Erros Comuns e Soluções](#erros-comuns-e-soluções)

---

## 🤔 O que é GitHub?

GitHub é uma plataforma online que permite que você armazene, gerencie e compartilhe seus projetos de código. É como um "Google Drive" para programadores, mas muito mais poderoso!

### Por que usar GitHub?

- **Controle de Versão**: Rastreie todas as alterações no seu código
- **Backup na Nuvem**: Seus projetos ficam seguros online
- **Colaboração**: Trabalhe em equipe de forma organizada
- **Portfólio Profissional**: Mostre seus projetos para empregadores
- **Código Aberto**: Compartilhe seu conhecimento com a comunidade

### Conceitos Importantes

| Conceito | Explicação |
|----------|-----------|
| **Repositório** | Pasta do projeto que armazena todos os arquivos e histórico de mudanças |
| **Commit** | Uma "foto" do seu código em um momento específico |
| **Push** | Enviar suas alterações do computador para o GitHub |
| **Pull** | Baixar as alterações do GitHub para seu computador |
| **Branch** | Uma versão paralela do seu código para trabalhar sem afetar o principal |

---

## ✍️ Criando uma Conta no GitHub

### Passo 1: Acessar o Site oficial

1. Abra seu navegador (Chrome, Firefox, Edge, etc.)
2. Acesse **www.github.com**
3. Você verá a página inicial do GitHub com o lema "The future of building happens together"

### Passo 2: Iniciar o Cadastro

1. Clique no botão verde **"Sign up for GitHub"** no centro da página
2. Você será redirecionado para o formulário de cadastro

### Passo 3: Preenchendo o Formulário

Na página de cadastro, você precisa preencher os seguintes campos:

#### Email
- Digite seu **email válido** que você usa regularmente
- Exemplos: `seu.nome@gmail.com`, `seu.nome@outlook.com`
- ⚠️ **Importante**: Este email será usado para recuperar sua conta, então use um que você tenha acesso

#### Senha
- Crie uma **senha forte** (mínimo 15 caracteres OU 8 caracteres com letras, números e símbolos)
- Exemplos de senhas fortes:
  - `MeuProjeto2024#GitHub`
  - `Senha@Segura123Forte`
- ⚠️ **Aviso**: Nunca use datas de nascimento ou nomes pessoais como senha

#### Nome de Usuário
- Escolha um **nome único** para sua conta
- Pode conter letras, números e hífens
- Exemplos: `joao-silva`, `dev-maria-2024`, `tech-developer`
- Este nome será parte da sua URL: `github.com/seu-usuario`
- 💡 Dica: Escolha um nome profissional que você gostaria que empregadores vissem

#### País/Região
- Selecione **Brasil** no dropdown se for brasileiro
- Esta informação é importante para conformidade legal

### Passo 4: Verificando o Email

1. Após clicar em "Create account", o GitHub enviará um **email de confirmação**
2. Abra seu email e procure pela mensagem do GitHub
3. Clique no link de verificação dentro do email
4. Sua conta estará ativa e pronta para uso!

### 🎉 Parabéns!

Você agora tem uma conta GitHub! Na próxima etapa, você criará seu primeiro repositório.

---

## 🏗️ Criando seu Primeiro Repositório

Um repositório é onde todos os arquivos do seu projeto ficarão armazenados.

### Passo 1: Acessar a Página de Novo Repositório

1. Faça login na sua conta GitHub
2. Clique no ícone **"+"** no canto superior direito
3. Selecione **"New repository"**
4. Ou acesse diretamente: `github.com/new`

### Passo 2: Configurando o Repositório

#### Nome do Repositório
- Digite um nome **descritivo** para seu projeto
- Exemplos: `meu-primeiro-projeto`, `calculadora-python`, `site-pessoal`
- O nome pode conter letras, números, hífens e underscores
- Dica: Use um nome que descreva o que o projeto faz

#### Descrição (Opcional)
- Adicione uma breve descrição do seu projeto
- Exemplo: "Um projeto para aprender Git e GitHub"
- Máximo de 100 caracteres

#### Visibilidade

Escolha entre **Público** ou **Privado**:

| Opção | Descrição | Ideal para |
|-------|-----------|-----------|
| **Público** | Qualquer um na internet pode ver | Portfólio, projetos open source |
| **Privado** | Apenas você e pessoas convidadas podem ver | Projetos pessoais, trabalho confidencial |

💡 **Para iniciantes**: Comece com um repositório **Público** para praticar

#### Inicializar com README

- ✅ **Marque**: "Add a README file"
- O README é um arquivo que descreve seu projeto
- Facilitará entender o que seu projeto faz quando alguém visitá-lo

#### Adicionar .gitignore (Opcional)

- .gitignore especifica quais arquivos não devem ser enviados ao GitHub
- Para iniciantes, deixe em branco por enquanto
- Aprenderá sobre isso mais adiante

### Passo 3: Criar o Repositório

1. Clique no botão verde **"Create repository"**
2. Seu repositório foi criado com sucesso!
3. Você verá a página do repositório com o arquivo README.md

### ✨ Resultado

Você agora tem um repositório online! A URL será: `github.com/seu-usuario/nome-do-repositorio`

---

## 💻 Instalando o Git no Windows

Git é o software que você usa no computador para enviar arquivos para o GitHub.

### Passo 1: Baixar o Git

1. Acesse **https://git-scm.com**
2. Clique em **"Download for Windows"**
3. O arquivo será baixado automaticamente (cerca de 50-100 MB)
4. Procure o arquivo na pasta Downloads

### Passo 2: Instalar o Git

1. **Clique duas vezes** no arquivo baixado (`Git-2.x.x-64-bit.exe`)
2. A janela do instalador abrirá
3. Clique em **"Next >"** várias vezes para aceitar as configurações padrão
4. ⚠️ **Importante**: Na tela "Choose the default editor used by Git", selecione uma opção:
   - **Visual Studio Code** (recomendado para iniciantes)
   - **Notepad** (simples)
   - Qualquer outra que você preferir

5. Continue clicando **"Next >"** até chegar em **"Install"**
6. Clique em **"Install"** e aguarde a instalação completar
7. Clique em **"Finish"** para encerrar

### Passo 3: Verificar a Instalação

Vamos confirmar que o Git foi instalado corretamente:

1. Abra o **Command Prompt** (ou PowerShell):
   - Pressione `Windows + R`
   - Digite: `cmd`
   - Pressione Enter

2. Digite o comando:
   ```
   git --version
   ```

3. Pressione Enter

4. Você deverá ver algo como:
   ```
   git version 2.43.0.windows.1
   ```

✅ Se viu a versão, o Git foi instalado com sucesso!

---

## ⚙️ Configurando o Git

Após instalar o Git, você precisa configurar seu nome de usuário e email. Estes dados aparecerão em todos os seus commits.

### Passo 1: Abrir o Command Prompt

1. Pressione `Windows + R`
2. Digite: `cmd`
3. Pressione Enter

### Passo 2: Configurar Nome de Usuário

Digite o comando abaixo (substitua pelos seus dados reais):

```bash
git config --global user.name "Seu Nome Completo"
```

Exemplo:
```bash
git config --global user.name "João Silva"
```

Pressione Enter.

### Passo 3: Configurar Email

Digite o comando abaixo (use o mesmo email que usou no GitHub):

```bash
git config --global user.email "seu.email@exemplo.com"
```

Exemplo:
```bash
git config --global user.email "joao.silva@gmail.com"
```

Pressione Enter.

### Passo 4: Verificar as Configurações

Para confirmar que tudo foi configurado corretamente, digite:

```bash
git config --global --list
```

Você verá algo como:
```
user.name=João Silva
user.email=joao.silva@gmail.com
```

✅ **Pronto!** Sua configuração do Git está completa.

---

## 🔐 Criando um Personal Access Token

⚠️ **Importante**: O GitHub não aceita mais sua senha comum para fazer push via linha de comando. Você precisa de um **Personal Access Token** (PAT).

Um Personal Access Token é como uma "senha especial" para autenticação segura.

### Passo 1: Acessar as Configurações

1. Faça login no GitHub
2. Clique na sua **foto de perfil** no canto superior direito
3. Clique em **"Settings"** (Configurações)

### Passo 2: Navegar para Tokens

1. No menu à esquerda, clique em **"Developer settings"**
2. Clique em **"Personal access tokens"**
3. Clique em **"Tokens (classic)"**
4. Clique no botão verde **"Generate new token (classic)"**

### Passo 3: Configurar o Token

#### Nota (Note)
- Digite um nome descritivo: `windows-git-token` ou `meu-token-git`
- Assim você saberá de onde vem este token

#### Expiração (Expiration)
- Selecione **"30 days"** (30 dias) para começar
- Tokens com data de expiração são mais seguros
- 💡 Você pode criar novos tokens quando este expirar

#### Escopo (Select scopes)
- ✅ Marque **"repo"** (acesso total a repositórios públicos e privados)
- Esta é a permissão essencial para fazer push/pull

### Passo 4: Gerar e Copiar

1. Clique no botão verde **"Generate token"** no final da página
2. **COPIE O TOKEN IMEDIATAMENTE** (ele só aparecerá uma vez!)
3. Salve em um local seguro (bloco de notas, por exemplo)
4. ⚠️ **Nunca compartilhe** este token com ninguém!

### ✅ Token Criado

Você agora tem seu Personal Access Token. Usaremos isto no próximo passo!

---

## 📤 Enviando Arquivos para o GitHub

Agora vem a parte emocionante! Você enviará seus primeiros arquivos para o GitHub.

### Cenário: Você tem uma pasta com arquivos locais

Suponha que você tem uma pasta chamada `meu-projeto` na sua área de trabalho com alguns arquivos.

### Passo 1: Clonar o Repositório

**Clonagem** é baixar seu repositório do GitHub para o computador.

1. Abra o **Command Prompt** (Windows + R, digitar `cmd`)
2. Navegue até onde você quer clonar:
   ```bash
   cd Desktop
   ```
3. Copie a URL do seu repositório:
   - Vá para `github.com/seu-usuario/nome-do-repositorio`
   - Clique em **"<> Code"** (botão verde)
   - Clique em **"HTTPS"**
   - Copie a URL (Ctrl + C)

4. No Command Prompt, digite:
   ```bash
   git clone https://github.com/seu-usuario/nome-do-repositorio.git
   ```
   
   Exemplo:
   ```bash
   git clone https://github.com/joao-silva/meu-primeiro-projeto.git
   ```

5. Pressione Enter e aguarde. Será criada uma pasta com o nome do repositório.

### Passo 2: Entrar na Pasta do Repositório

```bash
cd meu-primeiro-projeto
```

(Substitua pelo nome do seu repositório)

### Passo 3: Adicionar seus Arquivos

1. Copie os arquivos do seu projeto para esta pasta
2. Você pode usar o Explorador de Arquivos do Windows para isto
3. Exemplos de arquivos:
   - `main.py`
   - `index.html`
   - `dados.txt`
   - Qualquer arquivo do seu projeto

### Passo 4: Ver o Status

Para ver quais arquivos mudaram, digite:

```bash
git status
```

Você verá uma lista em **vermelho** dos arquivos novos/modificados.

### Passo 5: Adicionar Arquivos ao Índice

Use `git add` para "preparar" os arquivos para envio:

#### Adicionar um arquivo específico:
```bash
git add nome-do-arquivo.txt
```

#### Adicionar todos os arquivos:
```bash
git add .
```

(O ponto significa "todos os arquivos")

Exemplo:
```bash
git add .
```

### Passo 6: Confirmar as Mudanças (Commit)

Um **commit** é como fazer um "checkpoint" no seu projeto. Você descreve o que mudou:

```bash
git commit -m "Sua mensagem de commit"
```

**Dicas para boas mensagens de commit:**
- Seja **descritivo e conciso**
- Use **presente do indicativo**
- Comece com **letra maiúscula**

**Exemplos de boas mensagens:**
```bash
git commit -m "Adiciona calculadora básica"
git commit -m "Corrige bug na multiplicação"
git commit -m "Atualiza documentação README"
```

**❌ Evite:**
```bash
git commit -m "alterações"
git commit -m "teste"
git commit -m "mudanças várias"
```

### Passo 7: Enviar para o GitHub (Push)

Agora vem a parte final! Use `git push` para enviar seus commits para o GitHub:

```bash
git push origin main
```

Quando pedir autenticação:

#### Primeira vez:
- **Username**: Digite seu **nome de usuário do GitHub**
- **Password**: Cole o **Personal Access Token** que você criou (não é sua senha!)

#### Próximas vezes:
- O Git pode memorizar suas credenciais (marque "Save credentials" se aparecer)

### ✅ Enviado!

Se viu uma mensagem de sucesso, seus arquivos já estão no GitHub!

Verifique visitando: `github.com/seu-usuario/nome-do-repositorio`

---

## 🔄 Workflow Simplificado (Para Próximas Vezes)

Depois que clonar o repositório uma vez, seu fluxo de trabalho fica assim:

```bash
# 1. Abra Command Prompt e entre na pasta
cd caminho/do/seu/repositorio

# 2. Faça suas alterações nos arquivos
# (use Notepad, VS Code, ou qualquer editor)

# 3. Veja o que mudou
git status

# 4. Adicione os arquivos alterados
git add .

# 5. Faça um commit descrevendo as mudanças
git commit -m "Descrição do que mudou"

# 6. Envie para o GitHub
git push origin main
```

---

## 🌟 Boas Práticas

### 1. Mensagens de Commit Claras

**✅ BOM:**
```
git commit -m "Adiciona função de busca ao formulário"
git commit -m "Corrige problema de login no mobile"
git commit -m "Atualiza dependências do projeto"
```

**❌ RUIM:**
```
git commit -m "ajustes"
git commit -m "alterações"
git commit -m "teste"
```

### 2. Commits Frequentes

- Faça commits **pequenos e frequentes**
- Não acumule muitas mudanças em um único commit
- Facilita entender o histórico e reverter mudanças se necessário

### 3. Organize seus Arquivos

Estrutura de pastas recomendada:
```
meu-projeto/
├── README.md              # Descrição do projeto
├── src/                   # Código-fonte
│   ├── main.py
│   └── utils.py
├── dados/                 # Dados do projeto
│   └── dados.csv
├── docs/                  # Documentação
│   └── guia.md
└── .gitignore            # Arquivos a ignorar
```

### 4. Arquivo README.md

O README é a "capa" do seu projeto. Inclua:

```markdown
# Nome do Projeto

Uma breve descrição do que seu projeto faz.

## Como Instalar

Passo a passo para alguém usar seu projeto.

## Como Usar

Exemplos de uso.

## Requisitos

Quais programas/bibliotecas são necessários.

## Autor

Seu nome
```

### 5. .gitignore - Arquivos a Não Enviar

Crie um arquivo `.gitignore` na raiz do projeto para especificar quais arquivos NÃO enviar:

**Exemplo para Python:**
```
__pycache__/
*.pyc
.env
venv/
```

**Exemplo para JavaScript:**
```
node_modules/
.env
dist/
```

### 6. Revise Antes de Fazer Push

```bash
# Ver o diff (diferenças) do seu código
git diff

# Ver o que vai ser enviado
git status
```

---

## ❌ Erros Comuns e Soluções

### Erro 1: "Permission denied (publickey)"

**Problema**: Pode aparecer quando tenta fazer push.

**Solução**:
1. Verifique se criou o Personal Access Token
2. Certifique-se de ter digitado corretamente ao autenticar
3. Se salvou credenciais erradas, remova-as:
   - **Windows**: Painel de Controle > Credenciais > Gerenciar credenciais
   - Delete as entradas do GitHub

### Erro 2: "fatal: not a git repository"

**Problema**: Você não está dentro de um repositório Git.

**Solução**:
```bash
# Confirme que está na pasta correta
cd caminho/do/seu/repositorio

# Verifique se existe a pasta .git
dir /A | find ".git"

# Se não existir, clone novamente
git clone https://github.com/seu-usuario/seu-repositorio.git
```

### Erro 3: Esqueci minha Senha/Token

**Problema**: Não consegue autenticar no GitHub.

**Solução**:
1. **Para a senha**: Use "Forgot password?" no GitHub.com
2. **Para o Token**: Crie um novo Token (o antigo não será restaurado)
   - Acesse: github.com/settings/tokens
   - Gere um novo token e copie

### Erro 4: "Your branch is ahead of 'origin/main'"

**Problema**: Você tem commits locais não enviados.

**Solução**:
```bash
git push origin main
```

### Erro 5: Enviou Arquivo Confidencial por Acidente

**Problema**: Colocou senha, chave API ou arquivo sensível no repositório.

**Solução Imediata**:
1. Delete o arquivo do repositório local
2. Faça commit: `git commit -m "Remove arquivo sensível"`
3. Faça push: `git push origin main`
4. ⚠️ **Importante**: Uma vez público, pode ter sido visto. Mude senhas/chaves!

---

## 🎓 Próximos Passos

Após dominar o básico, explore:

1. **Branches**: Trabalhe em diferentes versões do código
2. **Pull Requests**: Contribua com projetos de outras pessoas
3. **Colaboração**: Trabalhe em equipe com seus amigos
4. **GitHub Pages**: Crie um site gratuito com GitHub
5. **GitHub Actions**: Automatize tarefas (testes, deploy, etc.)

---

## 📞 Recursos Adicionais

- **Documentação Oficial**: https://docs.github.com/pt
- **Pro Git Book**: https://git-scm.com/book/pt-br/v2
- **GitHub Learning Lab**: https://lab.github.com

---

## ✅ Checklist de Aprendizado

- [ ] Criei uma conta no GitHub
- [ ] Criei meu primeiro repositório
- [ ] Instalei o Git no Windows
- [ ] Configurei nome de usuário e email no Git
- [ ] Criei um Personal Access Token
- [ ] Clonei um repositório para meu computador
- [ ] Adicionei arquivos locais ao repositório
- [ ] Fiz meu primeiro commit
- [ ] Enviei (push) arquivos para o GitHub
- [ ] Verifiquei os arquivos online no GitHub

🎉 **Parabéns!** Você agora é capaz de usar Git e GitHub como um verdadeiro desenvolvedor!

---

## 📝 Notas Finais

- **Sempre verifique** antes de fazer push
- **Mensagens claras** facilitam a vida de todos
- **Pratique regularmente** para ficar confortável
- **Não tenha medo de erros** - é assim que aprendemos!
- **Pergunte em comunidades** se tiver dúvidas

---

*Guia criado para iniciantes em Git e GitHub - v1.0*
*Última atualização: 2025*