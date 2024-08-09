## Guia Iniciante para Git e GitHub

Bem-vindo ao guia para iniciantes de Git e GitHub! Este tutorial irá guiá-lo através dos primeiros passos do uso de Git e GitHub, incluindo a configuração inicial e comandos básicos essenciais.

## Sumário

1. [Instalação do Git](#instalação-do-git)
2. [Configuração Inicial do Git](#configuração-inicial-do-git)
3. [Criando um Repositório Local](#criando-um-repositório-local)
4. [Conectando ao GitHub](#conectando-ao-github)
5. [Comandos Básicos do Git](#comandos-básicos-do-git)
6. [Fluxo de Trabalho com GitHub](#fluxo-de-trabalho-com-github)
7. [Recursos Adicionais](#recursos-adicionais)

## Instalação do Git

### Windows
1. Baixe o instalador do Git em: [Git para Windows](https://gitforwindows.org/)
2. Execute o instalador e siga as instruções na tela.

### macOS
1. Abra o Terminal.
2. Execute o comando: 
   ```bash
   brew install git
   ```

### Linux
1. Abra o Terminal.
2. Execute o comando correspondente à sua distribuição:
   ```bash
   sudo apt-get install git # Para distribuições baseadas em Debian/Ubuntu
   sudo yum install git      # Para distribuições baseadas em Red Hat/CentOS
   ```

## Configuração Inicial do Git

Após a instalação, configure seu nome de usuário e e-mail:

```bash
git config --global user.name "Seu Nome"
git config --global user.email "seuemail@example.com"
```

Verifique suas configurações:

```bash
git config --list
```

## Criando um Repositório Local

1. Crie um novo diretório para seu projeto:
   ```bash
   mkdir meu-projeto
   cd meu-projeto
   ```

2. Inicialize um repositório Git:
   ```bash
   git init
   ```

## Conectando ao GitHub

1. Crie uma conta no [GitHub](https://github.com/).
2. Crie um novo repositório no GitHub:
   - No canto superior direito, clique no sinal de "+" e selecione "New repository".
 <img width="200" src="https://github.com/user-attachments/assets/416fdf20-a078-46ec-b267-56aab2a0c10e">

   - Dê um nome ao seu repositório, escolha se ele será público ou privado e clique em "Create repository".

3. Conecte seu repositório local ao repositório remoto no GitHub:
   ```bash
   git remote add origin https://github.com/seu-usuario/nome-do-repositorio.git
   ```

## Comandos Básicos do Git

### Status do Repositório
```bash
git status
```

### Adicionar Arquivos ao Staging
```bash
git add nome-do-arquivo
# Ou para adicionar todos os arquivos:
git add .
```

### Comitar Alterações
```bash
git commit -m "Mensagem descritiva sobre a alteração"
```

### Ver Histórico de Commits
```bash
git log
```

### Enviar Alterações para o GitHub
```bash
git push origin master
```

### Atualizar Repositório Local com Mudanças do Repositório Remoto
```bash
git pull origin master
```

## Fluxo de Trabalho com GitHub

### Clonar um Repositório
```bash
git clone https://github.com/seu-usuario/nome-do-repositorio.git
```

### Criar uma Nova Branch
```bash
git checkout -b nome-da-branch
```

### Alternar entre Branches
```bash
git checkout nome-da-branch
```

### Mesclar Branches
```bash
git checkout master
git merge nome-da-branch
```

### Resolver Conflitos de Merge
1. Edite os arquivos conflitantes conforme necessário.
2. Adicione e comite as alterações:
   ```bash
   git add nome-do-arquivo-conflitante
   git commit
   ```

## Recursos Adicionais

- [Documentação Oficial do Git](https://git-scm.com/doc)
- [Guia de Git do GitHub](https://guides.github.com/introduction/git-handbook/)
- [Pro Git Book](https://git-scm.com/book/en/v2)

---

Este guia oferece uma introdução básica ao Git e GitHub. À medida que se sentir mais confortável, explore comandos e funcionalidades mais avançadas para aprimorar ainda mais seu fluxo de trabalho. Boas práticas de versionamento e colaboração são essenciais para projetos bem-sucedidos.
