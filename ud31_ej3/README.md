

Parte A - Etiqueta sobre la tarjeta

La tarjeta tiene position: relative para que la etiqueta con position: absolute se coloque tomando la tarjeta como referencia. La etiqueta sobresale con top: -10px y right: -10px.

Como la tarjeta tiene overflow: hidden, se recorta la parte de la etiqueta que sobresale. Para verla entera, podemos quitar esa propiedad o cambiarla por overflow: visible.

Parte B - Caja de comentarios

- visible: el contenido que no cabe se ve fuera de la caja.
- hidden: el contenido que no cabe queda cortado.
- scroll: aparecen barras para poder desplazarse por todo el contenido.
- auto: aparecen barras cuando hacen falta. Es el valor que dejamos en el CSS.

visibility: hidden y display: none

- visibility: hidden:el elemento no se ve, pero mantiene reservado su espacio.
- display: none: el elemento desaparece y no reserva espacio; los elementos siguientes ocupan su lugar.

En el CSS se pueden ver las dos propiedades aplicadas a las tarjetas de prueba.