Dicas Desenvolvimento
===========================

### A meta tag X-UA-Compatible

- meta charset deve estar sempre antes dos 512b do documento;
- X-UA-Compatible sempre no início do <head>.
```
<!DOCTYPE html>
  <html>
    <head>
      <meta http-equiv="X-UA-Compatible" content="IE=Edge" />
      <meta charset="utf-8">
    ...
```


### Organização dos arquivos CSS

```
less/
├── _core/ (Configurações básicas do projeto)
│   ├── mixins/
│   |── colors
│   ├── fonts
│   ├── grid
│   ├── margins
│   ├── media-queries
│   ├── mixins
│   ├── normalize
│   ├── type
|
├── atoms/ (Classes individuais e elementos pequenos e reutilizáveis)
│   ├── global/
│   |   ├── scaffolding (html, body)
│   |   ├── utilies (.hidden, .show, .sr-only)
|   |
│   ├── buttons/
│   |   ├── btn
│   |   ├── btn-link
|   |
│   ├── text/
│   |   ├── headings (h1, h1, h3, h4, h5, h6)
│   |   ├── paragraph (p)
│   |   ├── blockquote
│   |   ├── code
│   |   ├── link (a)
│   |   ├── hr
│   |   ├── date (.date)
│   |   ├── inline (b, i, strong, em, u, stroke, cite ...)
|   |
│   ├── list/
│   |   ├── unordered
│   |   ├── ordered
│   |   ├── definition
|   |
│   ├── images/
│   |   ├── icons
│   |   ├── img
│   |   ├── logo
|   |
│   ├── forms/
│   |   ├── label
│   |   ├── input
│   |   ├── input-file
│   |   ├── select
│   |   ├── radio
│   |   ├── checkbox
|   |
│   ├── tables/
│       ├── tables
|
├── molecules/ (Cria um elemento 'pai' para modificar os atomos)
│   ├── blocks/
│   |   ├── toolbar
│   |   ├── filterbar
|   |
│   ├── media/
│   |   ├── banner
│   |   ├── media
|   |
│   ├── forms/
│   |   ├── search
│   |   ├── form-group
|   |
│   ├── navigation/
│   |   ├── navbar
│   |   ├── breadcrumbs
│   |   ├── pagination
│   |   ├── tabs
|   |
│   ├── text/
│   |   ├── address
│   |   ├── page-header
│   |   ├── author
│   |   ├── article-text
│   |   ├── captions
|   |
│   ├── components/ (Componentes que usam JavaScript)
│       ├── carousel
│       ├── collapse
│       ├── tooltip
│       ├── popover
│       ├── modal
|
├── organisms/ (Estruturas maiores do projeto, que podem modificar átomos e móleculas)
│   ├── header
│   ├── footer
│   ├── main
│   ├── wrap
│   ├── content
│   ├── comments
|
├── templates/ (Sistemas de grids e alinhamentos de templates)
│   ├── grids
│   ├── container
│   ├── thumbnails
|
├── pages/ (Estiliza páginas individualmente)
│   ├── home
|
├── vendor/ (Estiliza dependencias externas)

```
