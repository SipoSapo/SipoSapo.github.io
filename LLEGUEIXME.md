# Survival Anarko · blog fanzín (HTML + CSS purs)

Sense JavaScript ni frameworks. Obre `index.html` al navegador i ja està.

## Estructura
- `index.html`, `manifest.html`, `sobre-mi.html`, `contacte.html`: pàgines principals.
- `articles/`: una pàgina per entrada.
- `css/base.css`: reset, variables `:root` i tipografia.
- `css/layout.css`: estructura (header, nav, main, aside, footer).
- `css/components.css`: botons, targetes, badges, widgets, efectes.
- `css/pagines/`: un CSS per pàgina (`inici`, `article`, `contacte`). `manifest` i `sobre-mi` reutilitzen `article.css`.
- `assets/icones/`: cursor i icones pixelades (SVG). `assets/imatges/`: les teves fotos i collages.

Ordre de càrrega a cada HTML: base → layout → components → pàgina.

## Afegir un article
1. Copia un fitxer de `articles/` amb un nom nou (p. ex. `el-meu-article.html`).
2. Canvia `<title>`, el títol `<h2>`, la data (`<time>`), el badge i el text.
3. A `index.html`, copia un bloc `<article class="targeta">` i enllaça'l a `articles/el-meu-article.html`.

## Canviar la paleta
Edita les variables del bloc `:root` a `css/base.css` (`--negre`, `--blanc`, `--vermell`, `--groc`, `--verd-mc`). Cap altre fitxer té colors fixos, tret dels tons del bloc de terra (`--terra-1/2/3`).

## Header i footer
Estan repetits a cada HTML entre `<!-- COMPONENT: header -->` i `<!-- /COMPONENT: header -->` (igual pel footer). Per canviar-los a tot el web, fes un find & replace global d'aquest bloc. Atenció: a `articles/` els enllaços porten el prefix `../`.