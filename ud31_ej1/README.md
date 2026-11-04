 Ejercicio 

- static: es la posición normal. Si ponemos left: 50px en el cuadro 1 sin cambiar position, no se mueve porque left no funciona con static.
- relative: el cuadro 2 se desplaza, pero conserva su espacio original. Por eso queda un hueco donde estaba antes.
- absolute: el cuadro 3 sale del espacio normal y se coloca arriba a la derecha del contenedor. El contenedor necesita position: relative para ser su referencia.
- Hueco del cuadro 3: los demás cuadros no ocupan su lugar porque el cuadro está fuera del espacio normal.
- z-index: el cuadro 1 tiene valor 2 y queda por encima del cuadro 2, que tiene valor 1. Funciona porque ambos están posicionados.

Para probar static, cambia temporalmente .c1 a position: static; left: 50px;. Después devuelve el CSS a su estado actual.