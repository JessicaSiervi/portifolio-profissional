# Portfólio Profissional - Jessica Siervi

[![Esteira CI/CD](https://github.com/JessicaSiervi/portfolio-profissional/actions/workflows/ci-cd.yml/badge.svg)](https://github.com/JessicaSiervi/portfolio-profissional/actions/workflows/ci-cd.yml)

Site: https://jessicasiervi.github.io/portfolio-profissional/

## Sobre o projeto

Portfólio profissional desenvolvido com HTML5 e CSS3 para apresentar minhas habilidades, meus conhecimentos e meus projetos na área de Desenvolvimento de Sistemas.

## Tecnologias utilizadas

- HTML5
- CSS3
- Git e GitHub
- GitHub Actions
- GitHub Pages
- HTMLHint

## Automação CI/CD

A cada push ou pull request para a `main`, a esteira:

1. Executa a validação em Node.js 20 e 22.
2. Verifica a existência do `index.html`.
3. Executa o HTMLHint.
4. Verifica arquivos maiores que 500 KB.
5. Procura comentários proibidos (TODO, FIXME, senha, password).
6. Verifica links internos, âncoras e imagens.
7. Bloqueia a publicação se houver erros.
8. Publica automaticamente no GitHub Pages (somente em push na `main`).
9. Avisa falhas pelo Discord, se o secret `DISCORD_WEBHOOK` estiver configurado.

## Rodar localmente

```bash
npm install
npm run lint
npm run validate
```

## Estrutura do projeto

```text
portfolio-profissional/
├── .github/workflows/ci-cd.yml
├── assets/
│   ├── favicon.svg
│   └── foto-perfil.svg
├── scripts/validar.js
├── index.html
├── style.css
├── .htmlhintrc
├── package.json
├── package-lock.json
└── README.md
```

## Autora

Jessica Siervi

GitHub: https://github.com/JessicaSiervi

E-mail: jessicasiervi10@gmail.com
