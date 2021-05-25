
# LAB | Financial Data Graphing

## Introducción

![](http://i.giphy.com/l3Uct2K9N3CqxeCoU.gif)

[CoinDesk](http://www.coindesk.com/) es el líder mundial en noticias e información sobre monedas digitales como bitcoin y su tecnología subyacente: la blockchain.

Cubren noticias y análisis sobre las tendencias, movimientos de precios, tecnologías, empresas y personas en bitcoin, así como el mundo de la moneda digital.

En este ejercicio, utilizaremos uno de sus repositorios de datos: el [Índice de precios de Bitcoin](https://web.archive.org/web/20191106152143/https://www.coindesk.com/api). CoinDesk proporciona una API simple para generar sus datos de índice de precios de Bitcoin de forma programática, y la usaremos para representar los valores en un gráfico.

El índice de precios de Bitcoin es el valor que tiene bitcoin en diferentes monedas. Así que vamos a mostrar estas variaciones en un gráfico con [Chart.js](http://www.chartjs.org/).

:eyes: **[ChartJS](http://www.chartjs.org/) (también conocida como chart.js) es una biblioteca de código abierto que nos permite crear gráficos estáticos y animados increíbles a través de HTML5 lienzo y JavaScript.**

## Requerimientos

- Hacer fork a este repo
- Clonar este repo.

## Entrega

- Al finalizar, ejecute los siguientes comandos

```
$ git add .
$ git commit -m "done"
$ git push origin master
```

- Enviar la URL en la entrega del Canva

# Instrucciones

Ya hemos creado un archivo JavaScript para agregar todo el código AJAX: `public/javascripts/financialdata.js`

La aplicación será un ejercicio súper simple en el que representaremos algunos datos en un gráfico de líneas.

![](https://s3-eu-west-1.amazonaws.com/ih-materials/uploads/upload_b94d2137d3737b49ecf92ee8709f5a14.png)

Empecemos!

## Iteration #1: Obtener la data

Lo primero que debemos hacer es obtener los datos que vamos a representar en nuestro gráfico. Para hacer eso, usaremos la [Documentación de la API de CoinDesk](https://web.archive.org/web/20191106152143/https://www.coindesk.com/api).

Como queremos presentar datos históricos en el gráfico, como puede ver, debe realizar una solicitud `GET` a la URL`http://api.coindesk.com/v1/bpi/historical/close.json`. La respuesta será un JSON con los datos que queremos representar.

Como puede ver en la imagen de arriba, el eje Y representará el valor de bitcoin, mientras que el eje X representará la fecha de cada valor.

Vamos a utilizar Axios para realizar la solicitud AJAX, por lo que tenemos que importar Axios a través de su CDN.

**Tareas**

- Agrega la referencia de Axios en el HTML a través de CDN para poder usarlo.
- Debe crear una solicitud Axios para esta URL y obtener los datos. Use un `console.log()` para estar seguro de que estamos obteniendo los datos correctos.

## Iteration #2: Crear el gráfico

Una vez que tenemos los datos deseados, tenemos que mostrarlos como un gráfico. Vamos a utilizar [Chart.js](http://www.chartjs.org/) para hacer eso. Entonces tenemos que agregar la biblioteca a través de CDN.

Una vez que hemos agregado la referencia CDN en el archivo HTML, tenemos que representar los valores que obtuvimos en la Iteración 1 en un [Gráfico de líneas](http://www.chartjs.org/docs/#line-chart-introduction).

**Nota**: antes de pedir ayuda con la representación del gráfico, intente leer la documentación y averigüe cómo funciona. :)

**Tareas**

- Agregue la referencia Chart.js a través de CDN.
- Dar el formato correcto a los datos que obtenemos en la Iteración 1 para mostrarlo en un gráfico de líneas.
- Practique la lectura de documentación con la [documentación de la línea del gráfico](http://www.chartjs.org/docs/#line-chart-introduction).
- Crea un gráfico de líneas y muestra los datos.


¡Suerte! :heart:
