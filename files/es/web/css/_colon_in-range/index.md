---
title: ':in-range'
slug: Web/CSS/:in-range
tags:
  - CSS
  - Pseudo-clase
  - Referencia
  - Web
translation_of: Web/CSS/:in-range
---
{{CSSRef}}

La [pseudo-clase](/es/docs/CSS/Pseudo-classes "Pseudo-classes") **`:in-range`** de [CSS](/es/docs/Web/CSS) representa un elemento {{htmlelement("input")}} cuyo valor actual se encuentra dentro de los límites de rango especificados por los atributos {{htmlattrxref("min", "input")}} y {{htmlattrxref("max","input")}}.

```css
/* Selecciona cualquier <input>, pero solo cuando tiene un rango
   especificado, y su valor está dentro de ese rango */
input:in-range {
  background-color: rgba(0, 255, 0, 0.25);
}
```

Esta pseudo-clase es útil para dar al usuario una indicación visual de que el valor actual de un campo está dentro de los límites permitidos.

> **Nota:** Esta pseudo-clase solo se aplica a los elementos que tienen (y pueden tomar) una limitación de rango. En ausencia de tal limitación, el elemento no puede estar "dentro del rango" ni "fuera de rango".

## Sintaxis

{{csssyntax}}

## Ejemplo

### HTML

```html
<form action="" id="form1">
  <ul>Los valores entre 1 y 10 son válidos.
    <li>
      <input id="value1" name="value1" type="number" placeholder="1 a 10" min="1" max="10" value="12">
      <label for="value1">Tu valor esta </label>
    </li>
  </ul>
</form>
```

### CSS

```css
li {
  list-style: none;
  margin-bottom: 1em;
}

input {
  border: 1px solid black;
}

input:in-range {
  background-color: rgba(0, 255, 0, 0.25);
}

input:out-of-range {
  background-color: rgba(255, 0, 0, 0.25);
  border: 2px solid red;
}

input:in-range + label::after {
  content: 'bien.';
}

input:out-of-range + label::after {
  content: 'fuera de rango!';
}
```

### Resultado

{{EmbedLiveSample('Ejemplo', 600, 140)}}

## Especificaciones

| Especificación                                                                                       | Estado                               | Comentarios                                               |
| ---------------------------------------------------------------------------------------------------- | ------------------------------------ | --------------------------------------------------------- |
| {{SpecName('HTML WHATWG', 'scripting.html#selector-in-range', ':in-range')}} | {{Spec2('HTML WHATWG')}}     | Define cuándo `:in-range` coincide con elementos en HTML. |
| {{SpecName('CSS4 Selectors', '#in-range-pseudo', ':in-range')}}                 | {{Spec2('CSS4 Selectors')}} | Definición Inicial.                                       |

## Compatibilidad con navegadores

{{Compat("css.selectors.in-range")}}

## Ver también

- {{cssxref(":out-of-range")}}
- [Validación de datos de formulario](/es/docs/Learn/HTML/Forms/Form_validation)
