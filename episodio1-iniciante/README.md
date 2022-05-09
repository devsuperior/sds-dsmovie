# ![DevSuperior logo](https://raw.githubusercontent.com/devsuperior/bds-assets/main/ds/devsuperior-logo-small.png) Semana Spring React - Episódio 1
>  *Crie um app completo para seu portfólio com as tecnologias mais demandadas do mercado*

## TRILHA PARA INICIANTES

## Realização
[DevSuperior - Escola de programação](https://devsuperior.com.br)

[![DevSuperior no Instagram](https://raw.githubusercontent.com/devsuperior/bds-assets/main/ds/ig-icon.png)](https://instagram.com/devsuperior.ig)
[![DevSuperior no Youtube](https://raw.githubusercontent.com/devsuperior/bds-assets/main/ds/yt-icon.png)](https://youtube.com/devsuperior)

## Objetivos do projeto para esta aula
- Criar o projeto e salvar no Github
- Criar o layout da barra superior
- Criar o layout da listagem de filmes

## AVISO: as aulas ficarão disponíveis somente até domingo às 23h59

## AVISO: Instruções sobre certificado no Github do [aqui](https://github.com/devsuperior/sds-dsmovie/tree/main/_certificado)

## Checklist

### Passo: preparação

#### Dica: extensões do VS Code

- Color Highlight
- Live Server

#### Design Figma

https://www.figma.com/file/hpQuzpGHq2MmrI87xnfMoT/DSMovie1

https://www.figma.com/file/svCMhNqgpAZuN86w9IHJ4v/DSMovie2

https://www.figma.com/file/gEZYKqJJs2gEhIB6k9ksGB/DSMovie3

https://www.figma.com/file/hyovBMIxwrn2Bb5MZLrxHL/DSMovie4


### Passo: criar projeto HTML

HTML é uma **linguagem de marcação** que define a **estrutura do conteúdo** de uma página web. 

O código HTML segue uma estrutura **hierárquica** de *elementos*. Cada elemento corresponde a uma **tag** que deve abrir e fechar, respeitando a hierarquia.

Um site web pode conter vários arquivo HTML. Geralmente o arquivo HTML que será aberto por padrão se chama `index.html`.

### Passo: salvar primeira versão no Github

Caso não tenha configurado ainda seu Github:

[![Image](https://img.youtube.com/vi/_hZf1teRFNg/mqdefault.jpg "Vídeo no Youtube")](https://youtu.be/_hZf1teRFNg)

```bash
git init

git add .

git commit -m "Projeto criado"

git branch -M main

git remote add origin git@github.com:seuusuario/seurepositorio.git

git push -u origin main
```

### Passo: adicionar Bootstrap ao projeto

Bootstrap é um framework CSS. Ele fornece recursos que facilitam algumas tarefas na estilização das nossas páginas web.

Site oficial do Bootstrap:

https://getbootstrap.com

- **COMMIT: Bootstrap**

### Passo: fonte do Google Fonts

```css
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:wght@400;700&display=swap');
```

- **COMMIT: Google Fonts**

### Passo: Barra superior PARTE 1

Referências sobre HTML e CSS:

https://developer.mozilla.org/pt-BR/docs/Web/HTML

https://developer.mozilla.org/pt-BR/docs/Web/CSS

https://www.w3schools.com/html/

https://www.w3schools.com/css/

https://css-tricks.com/snippets/css/a-guide-to-flexbox/

```css
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:wght@400;700&display=swap');

:root {
  --color-primary: #4d41c0;
  --bg-gray: #e8e8e8;
}

* {
    box-sizing: border-box;
    font-family: 'Open Sans', sans-serif;
}

html, body {
    background-color: var(--bg-gray);
}

a, a:hover {
  text-decoration: none;
  color: unset;
}
```

- **COMMIT: Barra superior PARTE 1**

### Passo: Barra superior PARTE 2

- **COMMIT: Barra superior PARTE 2**

### Passo: Card de filme

Vamos usar imagens o The Movie Database:

https://www.themoviedb.org

- **COMMIT: Card de filme**

### Passo: Listagem de cards

Grid System do Bootstrap:

https://getbootstrap.com/docs/5.1/layout/grid/

Breakpoints do Bootstrap:

https://getbootstrap.com/docs/5.0/layout/breakpoints/

- **COMMIT: Listagem de cards**



## PARABÉNS!

![Parabéns!](https://raw.githubusercontent.com/devsuperior/bds-assets/main/img/trophy.png)

- Quero muito saber seu feedback
  - O que você está achando da nossa abordagem?
  - Você está conseguindo acompanhar?
  - O que você está achando do evento?
- Participe
  - Comente no Instagram e marque a gente @devsuperior.ig
  - Divulgue seu projeto no Linkedin e marque a DevSuperior
