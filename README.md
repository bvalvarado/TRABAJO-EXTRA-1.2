## TUTORIAL PARA SIMULAR LA ESTRUCTURA ELECTRÓNICA DE UNA RASPBERRY PI 1 MODELO B  EN MULTISIM

<br>

**1. MARCO TEÓRICO**

<br>

**A. RASPBERRY PI 1 MODELO B**

Raspberry Pi es un miniordenador de placa reducida también que trabaja con un MICROPROCESADOR BCM 2835, aunque no se indica expresamente si es hardware libre o con derechos de marca, es compatible con varios Sistemas operativos de libre acceso, siendo su sistema operativo oficial una versión adaptada de Debian, denominada Raspbian, aunque permite lenguaje de programación Python – IDLE.
El Modelo B, trajo consigo diversas mejoras, la inclusión del doble de memoria RAM, pasando de 256MB a 512MB, puertos USB y por fin, un conector Ethernet. No hubo variaciones ni en el procesador ni en la parte gráfica.








B.	ESPECIFICACIONES TÉCNICAS y ELEMENTOS PRINCIPALES DE LA PLACA BASE
RASPBERRY PI 1 MODELO B
o	Microprocesador:	 	Broadcom BCM2835
o	CPU:				ARM 1176JZF-S a 700 MHz (familia ARM11)
o	Juego de instrucciones:	RISC de 32 bits
o	Memoria:			512 MB 
o	Puertos USB 2.0:		2 puertos
o	Entradas de vídeo:		Conector MIPI y CSI que permite instalar un módulo         de cámara 
o	Salidas de vídeo:		Conector RCA (PAL y NTSC), HDMI, Interfaz DSI para panel LCD
o	Salidas de audio:		Jack de 3.5 mm, HDMI
o	Almacenamiento:		Tarjeta de almacenamiento SD
o	Conectividad de red:	 	10/100 Mbps - Ethernet  vía hub USB, micro controlador LAN 9514
o	Consumo energético:	 		500 mA (2.5 W)	
o	Fuente de alimentación:			5V  vía Micro USB o puerto GPIO Dimensiones:					85mm x 53mm
o	Sistemas operativos soportados:		GNU/Linux: Raspbian
o	Interfaz de programación soportada:	Python IDLE
o	Reguladores de voltaje:


















C.	NI MULTISIM 14.0
Es un programa que ha sido diseñado específicamente para profesores, estudiantes y profesionales del diseño de circuitos, hace que la creación de cualquier circuito eléctrico se convierta en un proceso sencillo, con la posibilidad de añadir cualquier elemento a los circuitos, teniendo una librería con más de 4000 objetos, y un sistema de pruebas que se activa y desactiva mediante un pequeño interruptor. 
Por tanto, si eres un estudiante de ingeniería eléctrica y quieres tener acceso a uno de los mejores programas del sector para la creación de circuitos eléctricos, descarga e instala NI Multisim Student Edition en tu ordenador.
 
¿Dónde puedo instalar NI MULTISIM 14.0? 
NI MULTISIM es compatible con las siguientes plataformas:
o	Sistema Operativo Windows® 10 Windows® 8 / 8.1 Windows® 7, XP
o	128 MB MEMORIA RAM
o	Tarjeta de Video Integral
o	Tarjeta de Sonido 5.1
o	2000 Megas Espacio Disco Duro
o	Procesador 2.3Ghz dual core
o	Monitor VGA
o	Conexión a Internet


2.	DIAGRAMA ELECTRÓNICO

3.	LISTA DE COMPONENTES 

3.1	COMPONENTES GENERALES 

•	Computador con  Sistema Operativo Windows 8 ó 10


•	
•	

•	
•	Software de simulación NI Multisim 14.0			







				   3.2. COMPONENTES EN MULTISIM
o	Microprocesador (Z08470 equivalente al BCM2835):

Controla todas las operaciones lógicas de la Raspberry es el cerebro del dispositivo






o	Controlador:
ETHERNET LAN

Gestiona y controla la conexión de red 






o	Puertos: 
Puertos de acceso y alimentación de las raspberry pi y lector de tarjetas SD

USB                                   MICRO USB                    ENTRADA TARJETA SD






o	Salidas:

Salidas o terminales en las cuales se pueden conectar: internet por medio de cable DNS, un periférico con entrada HDMI al igual que salidas de audio y video.

ETHERNET                              HDMI                               AUDIO Y VIDEO






o	Reguladores de Voltaje:
Regulan la entrada de voltaje a los puertos o pines para evitar una sobrecarga, la regulación se realiza en dos valores 1,8V y 3V.

Regulador 1.8V                                                 Regulador 3V









o	Conectores:
Entradas para la transmisión de información mediante la conexión de cables macho -hembra o buses de datos. 



DSI                                                                   CSI






GPIO o PINES                                                                        Clavijas JTAG


o	LEDs

Son 4 focos que según se enciendan tienen diferentes propósitos entre los principales indican cuando existe paso de corriente o cuando algún periférico o cable sea de audio, HDMI o de Internet se encuentra conectado







4.	EJECUCIÓN DEL PROYECTO

1.	Primero abrimos el software de simulación NI Multisim 14.0, de la siguiente manera, damos clic derecho sobre el icono del programa y elegimos la opción:

Propiedades/compatibilidad/Nivel de privilegio/ejecutar como administrador/aplicar y aceptar


2.	Una vez ingresamos a nuestro espacio de trabajo podemos utilizar el scroll del mouse para desplazarnos con mayor facilidad y regular el zoom de la pantalla.



3.	Para empezar a agregar los diferentes componentes de nuestra placa base presionamos la combinación de teclas:	

Ctrl + W

Nos enviará a una ventana donde observamos todos los componentes eléctricos y electrónicos que dispone Multisim.

 

4.	Una vez en la ventana de componentes nos desplazamos hacia la parte izquierda, seleccionamos el elemento y su modelo, siguiendo el diseño del diagrama electrónico citado en la parte 2 del presente tutorial y le damos clic en aceptar.
  
5.	Colocamos  un microprocesador que vendría a ser el corazón de la placa. En vista que Multisim no cuenta con el elemento BCM 2835 se va a colocar un componente con características y funciones similares en este caso un microprocesador Z08470, le damos clic en aceptar.

 

6.	Si le damos clic derecho sobre el elemento nos aparece un menú de edición donde se puede cambiar el color del trazo, el tipo y tamaño de letra o rotar la posición del elemento.

 
  

7.	Al dar doble clic sobre el elemento podemos cambiar el nombre del componente y el valor nominal del dispositivo.

 

8.	Para agregar un elemento de manera más rápida abrimos la ventana de componentes (Ctrl+W) en la parte derecha oprimimos el botón buscar.

 

9.	Una vez en esta ventana ingresamos directamente el código del elemento en el apartado  Componente:________  y le damos clic en búsqueda.

(Podemos revisar los códigos de los elementos en la parte 3.2 de este documento).
 

10.	Aparece una nueva ventana con el elemento que se buscaba,  simplemente le damos  clic en aceptar, regresamos a la ventana inicial nuevamente clic en aceptar y después clic en la pantalla.










11.	Repetimos este proceso con los elementos restantes.

 

 

12.	Una vez que ya se tienen todos los elementos que conforman la Raspberry Pi, nos dirigimos a:
                                  Barra de Menús/Colocar/Gráficos/Rectángulo













13.	Trazamos un rectángulo que delimite a todos los componentes 
 
14.	Finalmente tenemos la simulación de la ESTRUCTURA ELECTRÓNICA DE UNA RASPBERRY PI 1 MODELO B  EN MULTISIM.










5.	BIBLIOGRAFÍA

•	Xataka Basics. (2017). RASPBERRI PI, qué es y cómo funciona. Blog de Tecnologías de la Información. Recuperado el 11 de junio del 2019 de: https://www.xataka.com/basics/raspberri pi-que-es-y-como-funciona
•	http://www.xumarhu.net/raspberrypi_arquitectura.pdf
•	http://blogmultisim.blogspot.com/2011/04/utilizando-buses-de-datos-en-multisim.html
•	https://www.raspberrypi.org/documentation/hardware/computemodule/datasheets/rpi_DATA_CM_1p0.pdf




