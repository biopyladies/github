# **Aula 2 – Git na Prática: Repositórios Locais e Remotos**

*Esta aula prática faz parte do módulo de Git/GitHub do curso de Python Básico e Intermediário da comunidade **PyLadies Bioinfo**.*

## 🎯 **Objetivos**

- Criar e gerenciar repositórios locais com Git
- Conectar repositórios locais ao GitHub
- Usar os comandos básicos no terminal e no VSCode
- Entender o fluxo de versionamento local/remoto

---

## 🧰 **Pré-requisitos**

- Conta no [GitHub](https://github.com/)
- Git instalado ([site oficial](https://git-scm.com))
- Git configurado:
    ```bash
    git config --global user.name "Seu Nome"
    git config --global user.email "seuemail@exemplo.com"
    ```

* Chave SSH cadastrada ([tutorial aqui](https://docs.github.com/pt/authentication/connecting-to-github-with-ssh))

---

## 🛠️ **Passo a passo prático**

### **1. Criar um diretório do projeto**

```bash
mkdir meu-projeto-git
cd meu-projeto-git
```

### 2. Inicializar o repositório local

```bash
git init
```

> Um diretório oculto `.git/` será criado – ele armazena o histórico do seu repositório.

---

### 3. Criar e adicionar arquivos

```bash
echo "# Meu Projeto com Git" > README.md
git add README.md
git commit -m "feat: add initial README"
```

---

### 4. Criar o repositório no GitHub

1. Vá para [github.com](https://github.com)
2. Clique em **"New Repository"**
3. Dê o mesmo nome do diretório local (`meu-projeto-git`)
4. Não marque para criar README (já temos um)

---

### 5. Conectar repositório local ao remoto

#### Usando SSH:

```bash
git remote add origin git@github.com:seu-usuario/meu-projeto-git.git
```

#### Usando HTTPS (menos recomendado):

```bash
git remote add origin https://github.com/seu-usuario/meu-projeto-git.git
```

---

### 6. Enviar as alterações

```bash
git push -u origin main
```

> A opção `-u` salva essa conexão entre seu repositório local e o `main` remoto, para que você possa usar `git push` nas próximas vezes.

---

### 7. Clonar um repositório já existente

```bash
git clone git@github.com:outro-usuario/algum-projeto.git
cd algum-projeto
```

---

## 🧪 Comandos úteis

| Comando                       | Descrição                          |
| ----------------------------- | ---------------------------------- |
| `git status`                  | Verifica o que mudou               |
| `git log`                     | Mostra o histórico de commits      |
| `git diff`                    | Mostra diferenças entre versões    |
| `git branch`                  | Lista branches                     |
| `git checkout -b nova-branch` | Cria e muda para nova branch       |
| `git pull`                    | Atualiza com as alterações remotas |
| `git push`                    | Envia as alterações para o GitHub  |

---

## 📝 Dica: Criar um .gitignore

Evite versionar arquivos temporários ou ambientes virtuais. Exemplo de conteúdo:

```
*.pyc
__pycache__/
.venv/
.env
.DS_Store
```

---

## 📚 Recursos extras

* [Guia oficial do Git](https://git-scm.com/book/pt-br/v2)
* [Git cheatsheet em português](https://training.github.com/downloads/pt_BR/github-git-cheat-sheet/)
* [Git Explorer (para montar comandos)](https://gitexplorer.com/)
* [Oh My Git! (jogo para aprender Git)](https://ohmygit.org/)

---

## ✅ Tarefa sugerida

1. Crie um repositório local com um script Python de teste.
2. Versione e envie para um repositório GitHub.
3. Compartilhe o link no grupo do curso!

---

> ✨ Este material é parte do esforço da PyLadies Bioinfo para promover autonomia técnica e colaboração entre mulheres na bioinformática.