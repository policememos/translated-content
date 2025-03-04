---
title: '::-webkit-progress-inner-element'
slug: Web/CSS/::-webkit-progress-inner-element
tags:
  - CSS
  - No estándar(2)
  - Pseudo-elemento
  - Referencia
translation_of: Web/CSS/::-webkit-progress-inner-element
---
{{CSSRef}}{{Non-standard_header}}

## Resumen

El [pseudo-elemento](/es/docs/Web/CSS/Pseudo-elements) [CSS ](/es/docs/Web/CSS)**`::-webkit-progress-inner-element`** representa la parte más exterior de un elemento {{HTMLElement("progress")}}. Es el padre del pseudo-elemento {{cssxref("::-webkit-progress-bar")}}.

> **Nota:** para que `::-webkit-progress-inner-element` tenga efecto , hay que darle valor none a {{cssxref("-webkit-appearance")}} en el elemento `<progress>`.

## Ejemplo

### Contenido CSS

```css
progress {
  -webkit-appearance: none;
}

::-webkit-progress-inner-element {
  border: 2px solid black;
}
```

### Contenido HTML

```html
<progress value="10" max="50">
```

### Salida

{{EmbedLiveSample("Ejemplo", 200, 50)}}

Una barra de progreso que use el estilo especificado anteriormente tendrá una apariencia similar a la siguiente::

![](https://mdn.mozillademos.org/files/13492/-webkit-progress-inner-element%20example.png)

## Especificaciones

No es parte de ninguna especificación. Es un pseudo-elemento propitario y específico de WebKit/Blink.

## Compatibilidad con los distintos navegadores

{{Compat("css.selectors.-webkit-progress-inner-element")}}

## Ver además

- Los pseudo-elementos usados por WebKit/Blink para dar estilos a otras partes de un elemento {{HTMLElement("progress")}} :

  - {{cssxref("::-webkit-progress-bar")}}
  - {{cssxref("::-webkit-progress-value")}}

- {{cssxref("::-moz-progress-bar")}}
- {{cssxref("::-ms-fill")}}
