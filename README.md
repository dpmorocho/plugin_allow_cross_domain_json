## Plugin Allow Cross Domain (SPANISH)

Este es el plugin que permite realizar consultas JSON en otros dominios, es simple:

  - Se crea una variable que contenga la URL del JSON que queremos.
    ```var request = 'https://raw.github.com/devsar/d3talk/master/flare.json';```
  - Se crea la consulta mediante jQuery, como prefijo se hace el llamado al archivo proxy.php el cual realiza la consulta de datos antes de que se envie la informacion al navegador.
  - Se limpia la URL mediante la funcion SCAPE.
  - Se obtiene la funcion de retorno (data).
    ```$.getJSON('proxy.php?request=' + escape(request) , function(data) { console.log(data); }```
  - Para comprobar si el objeto ha sido obtenido correctamente, en Chrome dar clic derecho - inspeccionar elemento - Consola y ver el objeto.

- Basado en [Obtener un JSON Cross-Domain con jQuery (rápido Proxy con PHP)](http://jafrancov.com/2010/08/quick-proxy-php/).

## Plugin Allow Cross Domain (ENGLISH)

This is the plugin that allows query of JSON from other domains, it's very simple:

  - We create a variable that contain the URL to json we want.
  ```var request = 'https://raw.github.com/devsar/d3talk/master/flare.json';```
  - We build the query, the prefix contain the call to proxy.php file, this file is a filter and it get the data before send the information to browser.
  - Clean the URL with SCAPE function.
  - We get the function (data).
     ```$.getJSON('proxy.php?request=' + escape(request) , function(data) {  console.log(data);  }```
  - To test it, load the page and then do right clic - inspect element - console and see the object.

- Basado en [Obtener un JSON Cross-Domain con jQuery (rápido Proxy con PHP)](http://jafrancov.com/2010/08/quick-proxy-php/).
