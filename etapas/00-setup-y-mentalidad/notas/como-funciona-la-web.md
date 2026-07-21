# Que pasa cuando escribes "google.com" y presionas enter

Lo primero es que el navegador investiga mediante DNS, donde se encuentra el sitio. 
Una vez obtenido el resultado, envia una peticion HTTP de tipo GET, para obtener los datos del sitio principal.

<!-- MENTOR (punto 1 y 2): antes de la petición HTTP faltan dos pasos, y el orden importa.
     El flujo real es: DNS -> conexión TCP (3-way handshake) -> handshake TLS (porque google.com es HTTPS)
     -> recién ahí la petición HTTP GET. HTTP viaja ARRIBA de TCP; no es un extra.
     Integrá el TCP/TLS ACÁ, en orden, no al final. -->

Luego de obtener la response, que debe ser un 2xx o un OK, el navegador renderiza la respuesta en la pantalla.

<!-- MENTOR (punto 3): "renderizar" es más que pintar, y acá vive el DOM (clave para React después).
     El navegador: parsea el HTML y construye el DOM -> pide recursos extra (CSS, JS, imágenes = más peticiones)
     -> arma CSSOM y render tree -> calcula layout -> pinta. Ampliá esta línea con esos pasos. -->

Teniendo en cuenta también la conexión a internet y el protocolo TCP/IP de comunicación, sobre como se mueve la información en el internet.

<!-- MENTOR: esta línea final sobra si movés el TCP/IP a su lugar correcto (arriba, antes del HTTP GET).
     Menor: revisá acentos (envia -> envía, peticion -> petición). -->
