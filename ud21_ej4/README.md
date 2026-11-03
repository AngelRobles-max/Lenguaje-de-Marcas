
En `index_con_error.html` puse a propósito `id="corp"` en un `<h1>` y en un `<h2>`.
Al pasar la página por el validador de W3C (validator.w3.org) aparece un mensaje como este:

```
Error: Duplicate ID corp.

From line 10, column 5; to line 10, column 18

</h1>↩    <h2 id="corp">Un sub
```

¿Cómo lo he corregido?

He dejado el `id="corp"` solo en el `<h1>` y en el `<h2>` he usado `class="corp"`.
En el CSS hay una regla `#corp` para el id y otra `.corp` para la clase.
Esa es la versión final, que está en `index.html`, y ya no da el error.

¿Por qué se desaconseja usar id para dar estilo?

- Un `id` tiene que ser único en la página, así que no se puede reutilizar para otros
  elementos. Una clase sí se puede repetir todas las veces que haga falta.
- El selector de id es muy específico y gana a casi todo (clases, etiquetas...). Eso hace
  difícil después cambiar o sobrescribir el estilo.
- Los id se reservan para otras cosas, como los enlaces internos (`href="#seccion"`).

Parte B: selectores de atributo

- `a[target]` da color rojo solo a los enlaces que tienen el atributo `target`
  (los dos que abren en pestaña nueva).
- `p[class]` da fondo amarillo claro solo a los párrafos que tienen el atributo `class`.
