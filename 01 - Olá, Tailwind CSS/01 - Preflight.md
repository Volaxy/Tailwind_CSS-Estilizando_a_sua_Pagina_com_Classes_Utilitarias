# Preflight

Nesta aula, vimos a ação do Preflight no elemento `<h1>`, vamos entender mais a fundo sobre essa folha de estilos que o Tailwind oferece.

O Preflight foi construído com base no [modern-normalize](https://github.com/sindresorhus/modern-normalize), é um conjunto de estilos básicos que atuam com o intuito de reduzir as inconsistências entre navegadores, visto que cada um define seu próprio conjunto padrão de propriedades CSS que são aplicadas aos elementos HTML.

## Quai estilos são redefinidos:

* Remove os estilos dos cabeçalhos (h1 até h6), como a margem, peso e tamanho de fonte, o tornando idêntico ao texto base.
* Remove o estilo das listas ul e ol, resultando em nenhum número ou marcador por padrão. Caso queira estilizar uma lista, pode fazê-lo usando os utilitários [list-style-type](https://tailwindcss.com/docs/list-style-type) e [list-style-position](https://tailwindcss.com/docs/list-style-position).
* Define todas as margens como zero para elementos que normalmente teriam margens por padrão.
* Todas as tags referentes a imagem se tornam elementos em nível de bloco ao invés de linha, assumindo o display: block por padrão.
* Define todas as bordas para uma largura de 0 pixel, sólida e a cor da borda definida por padrão.

## Código do Preflight:

```css
h1,
h2,
h3,
h4,
h5,
h6 {
  font-size: inherit;
  font-weight: inherit;
}

ol,
ul {
  list-style: none;
  margin: 0;
  padding: 0;
}

blockquote,
dl,
dd,
h1,
h2,
h3,
h4,
h5,
h6,
hr,
figure,
p,
pre {
  margin: 0;
}

img,
svg,
video,
canvas,
audio,
iframe,
embed,
object {
  display: block;
  vertical-align: middle;
}

*,
::before,
::after {
  border-width: 0;
  border-style: solid;
  border-color: theme('borderColor.DEFAULT', currentColor);
}
```