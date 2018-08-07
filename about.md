---
layout: page
title: Sobre
---

<!-- Mantenha esta página sincronizada com o conteúdo do README.md :) -->

[Odin Expo](http://expo.wpod.in/) é um _showcase_ de sites desenvolvidos com [Odin](https://github.com/wpbrasil/odin), criado pela comunidade [WordPress Brasil](https://github.com/wpbrasil).

Inspirado em [Bootstrap Expo](http://expo.getbootstrap.com/), [Built With Ember](http://builtwithember.io/) e [Beautiful Open](http://beautifulopen.com/).
Este site é feito como [Jekyll](http://jekyllrb.com), desenvolvido no [GitHub](https://github.com/wpbrasil/odin-expo), e é hospedado no [GitHub Pages](https://pages.github.com).

## Como enviar um site

Para enviar uma sugestão de site, [abra uma issue](https://github.com/wpbrasil/odin-expo//issues/new) ou [crie um pull request](https://github.com/wpbrasil/odin-expo//pulls/new). Será dada prioridade para as sugestões que seguirem as regras.

Verifique se já não existe um **Issue** ou **Pull Request** com o mesmo site. Apenas um site por **Issue** ou **Pull Request**.

### 1) Execute o site localmente (Opcional)

Esta é uma etapa opcional caso queira pré-visualizar o resultado da sua publicação ou fazer outras alterações mais profundas.

#### Opção 1 - Jekyll com Docker

Instale o [Docker](https://www.docker.com/).

```sh
docker-compose up
```

#### Opção 2 - Jekyll com Ruby / Bundler

Instale [Ruby](https://www.ruby-lang.org/en/documentation/installation/), [Bundler](https://bundler.io/) com `gem install bundler`, e execute `run bundle install`. Isso irá instalar as dependências Ruby, como o Jekyll e seus plugins. **Usuários Windows:** Leia [este guia](https://jekyllrb.com/docs/windows/) para rodar Jekyll no Windows sem problemas.

```sh
bundle exec jekyll serve
```

### 2) Crie uma nova publicação

Dentro do diretório `_site`, crie um novo arquivo no formato `.md` seguindo o formato:

```md
---
layout: post
title: "Título do site"
slug: slug-do-site
source: http://url-do-site.com.br
screenshot: image-do-site.png
---
```

### 3) Capturar screenshot

A imagem deverá ser salva otimizada em `screenshots/` com dimensões corretas, **1000x800px**.

Antes de enviar, é uma boa pratica otimizar a imagem através de um otimizador como o [TinyPNG](https://tinypng.com/) ou [ImageOptim](https://imageoptim.com/). Isso ajudará a manter o site rápido e o repositório mais leve possível.

**Dica:** Use os pacotes Node, [pageres-cli](https://www.npmjs.com/package/pageres-cli) e [imagemin-cli](https://www.npmjs.com/package/imagemin-cli), para gerar e otimizar o screenshot no formato `.png` do site através do url, siga o exemplo a abaixo. Lembre-se de substituir `wordpress.org` pelo url do seu site.
