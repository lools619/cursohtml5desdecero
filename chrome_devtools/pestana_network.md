# Pestaña network

Como decíamos, esta pestaña nos permite ver los recursos recuperados a través de las peticiones HTTP y los detalles de las mismas: tipo del mensaje (GET/POST), código de respuesta (200, 404, ...), etc.

Si abres las DevTools después de haber cargado la página la pestaña "Network" te saldrá vacía, si es así, refresca la página y verás como te aparece algo parecido<sup>1</sup> a esto:

![](../images/pestana_network.png)

Cada fila representa una petición HTTP, y si te fijas, dejando el cursor encima de una petición te mostrará la URL completa del recurso.

Si haces clic en cualquiera de las peticiones podrás ver los contenidos del recurso y algunos detalles que no nos preocuparán en este curso.

![](../images/cerrar_respuesta_red.png)

Para cerrar el detalle de la petición puedes pulsar en el aspa.

Veamos ahora **algunos** de las cosas que podemos hacer en esta pestaña. Si te dijas, las opciones en esta imagen no coinciden exactamente con las de la imagen anterior (y posiblemente tampoco con las tuyas), no importa que de momento no veremos ninguna de las nuevas, veamos que significan estas:

![](../images/network-panel.png)

* **[Preserve records on navigation](https://developer.chrome.com/devtools/docs/network#preserving-the-network-log-upon-navigation)**: por defecto aparece el bóton en rojo, esto significa que cada vez que cambiemos de página se eliminarán las peticiones y se añadirán las nuevas. Si lo desactivamos, se mantendrán las peticiones antiguas.
* **Preserve log**: si marcas esta opción, el efecto será justo lo contrario, nunca se borrarán las peticiones HTTP, ni siquiera aunque cambies de dominio.
* **Clear records**: este botón nos permite vaciar la información de las peticiones.
* **Hide/show filter buttons**: para ocultar/mostrar los botones para filtar.
* **Filter buttons**: estos botones nos permite ver sólo las peticiones HTTP que ha recuperado un tipo de recurso. *De momento* no lo usaremos mucho.
* **Summary view**: podemos ver cuántas peticiones HTTP se han necesitado para cargar la página (requests), cuando ocupa la suma de todos los recursos recuperados (XXX transferred), el tiempo que ha tardado en cargar, etc.
* **No throttling** (se ve en la imagen anterior): esto permite simular que tu conexión a Intenet es más lenta. Lo usaremos más adelante cuando queramos ver si nuestra página carga la suficientemente rápido usando un dispositivo conectado por 3G.

*Si es tu primera vez con DevTools **no te lo recomiendo***, pero si quieres, puedes encontrar más información (en inglés) sobre esta pestaña en:
* [Los recursos para desarrolladores de Chrome](https://developer.chrome.com/devtools/docs/network#preserving-the-network-log-upon-navigation)
* [Lección 5 del curso: Discover DevTools](https://www.codeschool.com/courses/discover-devtools)

Por último, simplemente quería animarte a que dediques un par de minutos a jugar con esta pestaña antes de pasar a la siguiente. Si tienes cualquier duda no olvides preguntarla en los [issues de Github](https://github.com/hhkaos/cursohtml5desdecero/issues).

<small>Aclaraciones:</small><br>
<small>1. Las peticiones serán distintas en cada página, por lo tanto con casi total seguridad tus peticiones serán distintas a las de la imagen.</small><br>