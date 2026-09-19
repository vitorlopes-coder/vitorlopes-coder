# Publicação do perfil

O GitHub mostra automaticamente o `README.md` no perfil quando existe um repositório **público** chamado exatamente `vitorlopes-coder` dentro da conta `vitorlopes-coder`.

Para publicar ou atualizar o seu perfil diretamente desta pasta:

```bash
cd /home/Vitor/Projetos/Eu
gh auth login -h github.com
git init
git add .
git commit -m "feat: adiciona perfil personalizado do GitHub"
gh repo create vitorlopes-coder --public --source=. --push
```

> **Dica após o push:**
> Abra a aba **Actions** no seu repositório no GitHub (`vitorlopes-coder/vitorlopes-coder`) e dispare manualmente uma vez a action **"Gerar animação de contribuições"**. Isso gerará a branch `output` com a cobrinha animada (`github-contribution-grid-snake.svg`), que a partir de então se atualizará automaticamente todo dia!
