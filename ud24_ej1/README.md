

#Elección entre display: inline-block y display: flex

He optado por display: flex aplicado al contenedor contenido

 Con display: inline-block, los espacios en blanco y los saltos de línea en el archivo HTML entre los elementos <div> se interpretan como espacio visible en el navegador. Esto añade unos píxeles extra a cada tarjeta, obligando a ajustar manualmente márgenes o anchos para evitar que la última tarjeta salte de línea. Por otro lado display: flex organiza las cajas hijas automáticamente en fila sin verse afectado por los espacios del código HTML.

---


 1.¿Qué diferencia hay entre margin y padding?
padding: Es el espacio que hay desde el contenido del elemento hasta su propio borde (por dentro de la caja).
margin: Es la distancia o espacio de separación que hay desde el borde de la caja hacia los demás elementos de alrededor (por fuera de la caja).

2.¿Por qué saltaba la tercera tarjeta de línea al usar inline-block?
Porque el ancho total ocupado por cada caja no es solo su width (220px)


3.¿Qué propiedades ignoraba el <span> y por qué?
Por defecto, la etiqueta <span> es un elemento de tipo display-inline. Los elementos en línea ignoran las propiedades width y height (su tamaño depende únicamente del texto que contienen) y tampoco aplican correctamente los márgenes verticales (margin-top y margin-bottom). Al cambiar a display: inline-block, pasa a comportarse como una caja a la que sí se le pueden definir dimensiones físicas e interlineado.

4.¿Qué hace display: none con el espacio que ocupaba la caja?
Cuando se aplica display-none, la caja desaparece por completo del flujo del documento y las demás cajas ocupan inmediatamente su lugar como si nunca hubiera existido. A diferencia de visibility-hidden (que oculta el elemento pero reserva el hueco), display-none no deja ningún espacio en blanco.
