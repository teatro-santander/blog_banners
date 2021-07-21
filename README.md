Los banners son fragmentos HTML que deberán insertarse dentro del blog del teatro en cada uno de los artículos que lo requieran. Al hacerlo se aconseja editarlos en algún editor de texto plano y NO en Word u otro editor de texto. Podrán descargar visual studio Code para hacer.

# API
Los banners con formulario están conectados a la API de Sendy, si se requiere cambiar una lista de correos dentro del banner se deberá únicamente cambiar por el nuevo ID del formulario.

# Estructura
Los banner se encuentran dentro de un archivo HTML el cual no debe ser copiado en su totalidad. Dentro de cada uno de los archivos encontrarán las instrucciones y las lineas de código que se deben copiar dentro del artículo de Ghost

# Añadir banner en ghost
En la opción de (+) debe elegir la opción HTML y allí pegar el fragmento de código. Ten en cuenta que si quieres ver cómo se ve el fragmento deberás usar la opción de previsualizar el artículo.
![ghost-example](https://github.com/teatro-santander/blog_banners/blob/master/img-examples/ghost-ejemplo.gif)

# Sobre el Banner Event
![banner-1](https://github.com/teatro-santander/blog_banners/blob/master/img-examples/event_banner.png)

Usa este banner cuando la boletería para alguno de los eventos esté disponible y las personas puedan ir al sitio web del operador de boletería a realizar la compra

## Como cambiar los textos de los banners
Los textos que puedes cambiar siempre los encontrarás entre comillas, si usas un editor de texto plano los verás de un color diferente al resto del código. En el código solo se podrán cambiar:
* URL del botón de la compra de la boletería
* Textos del banner

# Sobre el Banner Wait List
![banner-2](https://github.com/teatro-santander/blog_banners/blob/master/img-examples/Screen%20Shot%202021-07-16%20at%2015.40.28.png)

Usa este banner cuando la boletería esté a la espera de una nueva apertura por aforo o cuando se este considerando hacer una segunda función del mismo evento. Los cambios que podrás hacer son: 
* Textos del banner
* Texto del botón del formulario
* Código de la API (id del formulario en Sendy)
* Campo del evento al cual se debe asociar el dato

## Cambiar el id de la API
El id de la API es el mismo ID del listado en Sendy, si se quiere que el formulario envíe datos a un nuevo listado deberá asegurarse de que el nuevo listado tenga los mismas propiedades de contacto (nombradas de la misma manera)

## Cambiar el nombre del evento
Cuando un usuario ingrese sus datos, de forma oculta se enviará el dato sobre el evento en el cual está interesado. Para que esto sucede deberán ingresar en el código el nombre o id del evento al cual esta asociado el formulario. Para hacerlo deberán ubicarse en la linea 125 del código y allí cambiar el texto que está entre comillas por el id o nombre del evento al cual se asociará ese registro del usuario.

## Cambiar texto del botón del formulario
Este cambio se podrá hacer en la linea 142 del código cambiando el texto que está entre comillas. 

# Banners en los mail enviados desde Ghost
Los clientes de correos no aceptan algunos estilos HTMLl por consiguiente los banner pueden variar su diseño al enviarse los artículos como correos. ==Se suigiere que estos banners se añadan despúes de enviar el newslatter desde ghost.== Si el banner es de formluario ten en cuenta que esta no podrá llenarse desde un correo electrónico y puede generar una mala experienica para el usuario.