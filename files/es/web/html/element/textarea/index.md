---
title: <textarea>
slug: Web/HTML/Element/textarea
tags:
  - Elemento
  - Formularios(2)
  - HTML
  - Referencia
  - Web
translation_of: Web/HTML/Element/textarea
original_slug: Web/HTML/Elemento/textarea
---
## Resumen

El **elemento** **HTML `<textarea>`** representa un control para la edición mutilínea de texto sin formato.

## Contenido de Uso

| [Content categories](/es/docs/HTML/Content_categories "HTML/Content_categories") | [Flow content](/es/docs/HTML/Content_categories#Flow_content "HTML/Content categories#Flow content"), [phrasing content](/es/docs/HTML/Content_categories#Phrasing_content "HTML/Content categories#Phrasing content"), [Interactive content](/es/docs/HTML/Content_categories#Interactive_content "HTML/Content categories#Interactive content"), [listed](/es/docs/HTML/Content_categories#Form_listed "HTML/Content categories#Form listed"), [labelable](/es/docs/HTML/Content_categories#Form_labelable "HTML/Content categories#Form labelable"), [resettable](/en/HTML/Content_categories#form_resettable "en/HTML/Content categories#form resettable"), y [submittable](/es/docs/HTML/Content_categories#Form_submittable "HTML/Content categories#Form submittable") [form-associated](/es/docs/HTML/Content_categories#Form-associated_ "HTML/Content categories#Form-associated ") elemento |
| -------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Contenido Permitido                                                              | Datos carácter                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| Omisión de etiquetas                                                             | {{no_tag_omission}}                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| Elementos padre permitidos                                                       | Cualquier elemento que soporta [phrasing content](/es/docs/HTML/Content_categories#Phrasing_content "HTML/Content_categories#Phrasing_content").                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| Interfaz Dom                                                                     | {{domxref("HTMLTextAreaElement")}}                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |

## Atributos

Este elemento contiene [global attributes](/es/docs/HTML/Global_attributes "HTML/Global attributes").

- {{htmlattrdef("autocapitalize")}} {{non-standard_inline}}
  - : Este es un atributo no estándar utilizado por iOS Safari Mobile (y, por lo tanto, también por casi todos los navegadores de iOS, incluyendo Safari, Firefox y Chrome). Controla cuándo y cómo el texto debe ponerse automáticamente en mayúsculas mientras es ingresado/editado por el usuario. Los valores no obsoletos están disponible en iOs 5 y en versiones posteriores. Sus valores posibles son:
    - `none`: Deshabilita la capitalización automática
    - `sentences`: Escribe automáticamente con mayúscula la primera letra de cada frase.
    - `words`: Automáticamente escribe con mayúsculas la primera letra de las palabras.
    - `characters`: Automáticamente escribe con mayúscula todos los caracteres.
    - `on`: {{deprecated_inline()}} En desuso desde la versión 5 de iOS.
    - `off`: {{deprecated_inline()}} En desuso desde la versión 5 de iOS.
- {{htmlattrdef("autocomplete")}} {{HTMLVersionInline("5")}}
  - : Este atributo indica si el valor del control puede ser completado automáticamente por el navegador. Los posibles valores son:
    - `off`: El usuario debe explícitamente introducir el valor del campo para cada uso, o el documento proporciona su propio método de auto-completado; el navegador no completa automáticamente.
    - `on`: El navegador puede completar automáticamente el valor basándose en valores que el usuario haya insertado durante usos previos.
    
    Si el atributo **autocomplete** no está definidio en el elemento textarea, entonces el navegador usa el valor del atributo **autocomplete** del propietario del elemento `<textarea>` . El propietario del formulario es o bien el elemento form del cual el \<textarea> es descendiente o el elemento form cuyo id está especificado en el atributo form del elemento. Para más información, ver el atributo {{htmlattrxref("autocomplete", "form")}} en {{HTMLElement("form")}}.
- {{ htmlattrdef("autofocus") }} {{ HTMLVersionInline("5") }}
  - : Este atributo booleano te permite especificar que un control de un formulario adquiera el foco cuando se carga la página, salvo que el usuario anule esto , por ejemplo tecleando en un control diferente. Sólo se puede especificar este atributo en los elementos asociados a formularios.
- {{ htmlattrdef("cols") }}
  - : La anchura visible del control de texto, en caracteres de anchura media. Si está definido debe ser positivo. Si no, por defecto, el valor es 20 (HTML 5).
- {{ htmlattrdef("disabled") }}
  - : Este atributo booleano indica que el usuario no puede interactuar con el control. Si el atributo no está definido se hereda su valor del elemento en el que está contenido, por ejemplo {{ HTMLElement("fieldset") }}; Si no está dentro de un elemento contenedor con el atributo disable establecido, entonces el control estará habilitado.
- {{ htmlattrdef("form") }} {{ HTMLVersionInline("5") }}
  - : El formulario al cual el elemento textarea está asociado (el propietario del formulario). El valor del atributo debe ser un ID de un elemento formulario del mismo documento. Si no se especifica este atributo, el textarea debe ser un descendiente de un elemento formulario. Permite colocar elementos textarea en cualquier lugar dentro de un documento, no sólo como descendientes de formularios.
- {{ htmlattrdef("maxlength") }} {{ HTMLVersionInline("5") }}
  - : Indica el número máximo de caracteres (Unicode code points) que el usuario puede insertar. Si no está especificado entonces el usuario puede insertar un número ilimitado de caracteres.
- {{ htmlattrdef("minlength") }} {{ HTMLVersionInline("5") }}
  - : El mínimo número de caracteres (Unicode code points) que el usuaurio debe insertar.
- {{ htmlattrdef("name") }}
  - : El nombre del control
- {{ htmlattrdef("placeholder") }} {{ HTMLVersionInline("5") }}
  - : Se puede añadir un indicación para el usuario que defina que se debe insertar en el control. Los retornos de carro y las nuevas líneas dentro lso marcadores de posición deben ser tratado como nuevas líneas al representar dicha indicación.
- {{ htmlattrdef("readonly") }}
  - : Este atributo booleano indica que el usuario no puede modificar el valor del control. Al contrario que el atributo` disable`, el atributo `readonly `no evita que el usuario haga click o seleccione el control. El valor del control read-only si que se envía con el formulario.
- {{ htmlattrdef("required") }} {{ HTMLVersionInline("5") }}
  - : Este atributo indica que el usuario debe rellenar el contro con un valor antes de poder enviar el formulario.
- {{ htmlattrdef("rows") }}
  - : El número de líneas visibles en el control
- {{ htmlattrdef("selectionDirection") }} {{ HTMLVersionInline("5") }}
  - : La dirección en la que la selección ocurre dentro del control. Es "forward" si la selección ocurre de izquierda a derecha en una localización LTR, o "backward" si la selección fue hecha en sentido contrario. Puede ser "none" si se desconoce la dirección.
- {{ htmlattrdef("selectionEnd") }}
  - : El índice del último caracter de la selección actual.
- {{ htmlattrdef("selectionStart") }}
  - : El índice del primer caracter de la selección actual.
- {{ htmlattrdef("spellcheck") }} {{ HTMLVersionInline(5) }}
  - : Un valor `true` en este atributo indica que el elemento necesita tener `checked` el corrector ortográfico y gramatical. El caloor `default` indica que el elemento va a comportarse de acuerdo al comportamiento por defecto, basado en el `spellcheck` del padre. El valor `false` indica que no se deben hacer esas comprobaciones.
- {{ htmlattrdef("wrap") }} {{ HTMLVersionInline("5") }}
  - : Indica como el control envuelve al texto. Los posibles valores son:
    - `hard`: El navegador insertar automáticamente caracteres de nueva línea (CR+LF) para que ninguna línea tenga más anchura que la del control; el atributo `cols` debe estar espeficicado.
    - `soft`: El navegador asegura que todas las nuevas líneas constan de la pareja de caracteres CR+LF , pero no insertar nuevas líneas adicionales.Soft es el valor por defecto si no se especifica nada.

## Interfaz DOM

Este elemento implementa el interfaz [`HTMLTextAreaElement`](/en/DOM/HTMLTextAreaElement "en/DOM/textarea") .

{{ gecko("2.0") }} introduce el soporte para textareas redimensionable. Esto se controla con la propiedad CSS {{ cssxref("resize") }} . Por defecto la posibilidad de redimiensionar el control está habilitada, pero puede ser explícitamente deshabilitada mediante el uso del siguiente CSS:

    textarea {
      resize: none;
    }

## Interacción con CSS

En relación a CSS, un `<textarea>` es un [replaced element](/es/docs/CSS/Replaced_element "/en-US/docs/CSS/Replaced_element"). La especificación HTML no define dónde está el punto de referencia de un `<textarea>`. Así que los diferentes navegadores lo sitúan en diferentes posiciones. En los navegadores basados en Gecko, ese punto de referencia del `<textarea>` se sitúa en el punto de referencia de la primera línea del `<textarea>`, en otro navegadores puede estár situado al final de la caja del `<textarea>` . Se recomienda no usar {{cssxref("vertical-align")}}`: baseline` , ya que obtendríamos un comportamiento no impredecible.

Un _textarea_ tiene dimensiones intrínsecas, como una imagen agrandada.

## Ejemplo

### Contenido HTML

```html
<textarea name="textarea" rows="10" cols="50">Write something here</textarea>
```

{{ EmbedLiveSample('Example','600','200') }}

## Especificaciones

| Especificación                                                                                                                   | Estado                           | Comentarios |
| -------------------------------------------------------------------------------------------------------------------------------- | -------------------------------- | ----------- |
| {{SpecName('HTML WHATWG', 'the-button-element.html#the-textarea-element', '&lt;textarea&gt;')}} | {{Spec2('HTML WHATWG')}} |             |
| {{SpecName('HTML5 W3C', 'forms.html#the-textarea-element', '&lt;textarea&gt;')}}                     | {{Spec2('HTML5 W3C')}}     |             |
| {{SpecName('HTML4.01', 'interact/forms.html#h-17.7', '&lt;textarea&gt;')}}                             | {{Spec2('HTML4.01')}}     |             |

## Compatibilidad en Navegadores

{{Compat("html.elements.textarea")}}

## Ver además

Otros elementos relacionados con formularios: {{ HTMLElement("form") }}, {{ HTMLElement("button") }}, {{ HTMLElement("datalist") }}, {{ HTMLElement("legend") }}, {{ HTMLElement("label") }}, {{ HTMLElement("select") }}, {{ HTMLElement("optgroup") }}, {{ HTMLElement("option") }}, {{ HTMLElement("input") }}, {{ HTMLElement("keygen") }}, {{ HTMLElement("fieldset") }}, {{ HTMLElement("output") }}, {{ HTMLElement("progress") }} and {{ HTMLElement("meter") }}.

{{HTMLRef}}
