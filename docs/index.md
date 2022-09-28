# <FONT COLOR=#8B008B>1. Mis notas sobre programación de la placa Easy Plug con ArduinoBlocks</font>
Estas notas se dedican a la programación de la placa de control Ks0240 keyestudio EASY plug V2.0 con ArduinoBlocks a partir de diferentes actividades y/o retos incluyendo información básica de los componentes y de programación de manera progresiva.

## <FONT COLOR=#007575>**1.1. Elementos y componentes Easy Plug**</font>
Easy Plug es una placa donde podemos conectar diferentes sensores y actuadores de forma muy sencilla. Además, se pueden crear diferentes programas, proyectos y experimentos muy interesantes para niñas y niños de los últimos cursos de Educación Primaria así como, durante la etapa de educación secundaria.

Sus características técnicas principales son:

* Es compatible con Arduino Uno
* Cinco puertos digitales (de entrada y salida)
* Cuatro puertos de entrada analógica
* Un puerto SPI
* Un puerto I2C.
* Sus conectores son pines RJ-11 de cuatro hilos, lo que les hace mucho más fáciles para conectarlos y evitar malas conexiones.

En la Figura 1.1 vemos una imagen de la placa con rótulos descriptivos de la misma.

<center>

![Descripción de la placa Easy Plug](./img/index/F1.1.png)

*Figura 1.1. Descripción de la placa Easy Plug*

</center>

## <FONT COLOR=#007575>**ArduinoBlocks: programa, acceso e interfaz**</font>
Arduino es una plataforma de prototipos de código abierto, basada en hardware y software flexibles y fáciles de utilizar. Su finalidad es que todo el mundo pueda generar proyectos y entornos interactivos mediante placas y sensores compatibles con Arduino.

Arduino se programa con lenguaje C++ y se necesita el IDE (Integrated Development Environment), que permite escribir el código. Programar con C++ puede resultar complejo y no es accesible para todos, por eso, [Juanjo López](https://twitter.com/JuanjoLopezIbi) creó [ArduinoBlocks](http://www.arduinoblocks.com/web/), que es un lenguaje de programación por bloques que se ejecuta en la nube. Los diferentes bloques de programación sirven para leer y escribir las entradas y salidas de la placa.

Podemos registrarnos en la web, para guardar los proyectos, podemos añadir información a nuestros proyectos y ver proyectos de otros usuarios que hayan decidido compartirlos de forma pública. En la Figura 1.2 vemos la portada de la página web.

<center>

![Página principal web ArduinoBlocks](./img/index/F1.2.png)

*Figura 1.2. Página principal web ArduinoBlocks*

</center>

## <FONT COLOR=#007575>**¿Cómo se trabaja con ArduinoBlocks?**</font>
Para empezar a trabajar con ArduinoBlocks, es necesario registrarse utilizando un correo válido, pues habrá que validar la cuenta con ese correo, y crear un nuevo usuario. Debemos acceder al botón "Iniciar sesión" para después, seleccionar la opción de nuevo usuario, tal y como se indica en la Figura 1.3.

<center>

![Inicio de sesión en ArduinoBlocks](./img/index/F1.3.png)

*Figura 1.3. Inicio de sesión en ArduinoBlocks*

</center>

A continuación, se debe seleccionar "Empezar un proyecto nuevo" (Figura 1.4). 

<center>

![Iniciar un nuevo proyecto](./img/index/F1.4.png)

*Figura 1.4. Iniciar un nuevo proyecto*

</center>

Nos aparecen tres opciones: proyecto personal, profesor o alumno, tal y como vemos en la Figura 1.5.

<center>

![Opciones de proyecto](./img/index/F1.5.png)

*Figura 1.5. Opciones de proyecto*

</center>

Si escogemos el proyecto personal sólo podremos acceder nosotros, pero después lo podemos compartir si decidimos hacerlo público. En cambio, si seleccionamos el proyecto profesor, no se comienza un proyecto sino que se crea un código para que los alumnos puedan inscribirse en el proyecto. De esta forma, el profesor puede supervisar las programaciones de sus estudiantes. Por último, la opción de alumno es para unirnos al proyecto planteado por el profesor. Para aprender mas sobre [Usuarios Gestionados](https://drive.google.com/file/d/1uAhhYuQAzDbvmxJTRvDOK_rG4yPoQrxr/view?usp=drive_web) basta con acceder a la presentación del enlace anterior que se adjunta como anexo a este documento.

## <FONT COLOR=#007575>**Interfaz de programación de ArduinoBlocks**</font>
Una vez hemos escogido la opción de proyecto personal, nos pregunta qué placa estamos utilizando y qué nombre queremos dar a nuestro proyecto. A su vez, podemos añadir información, como: descripción del proyecto, componentes que necesitamos y otras especificaciones en el apartado de comentarios. En nuestro caso escogeremos: **Keyestudio EasyPlug**. Toda esta información es la que se ve en la Figura 1.6.

<center>

![Placa, nombre del proyecto,...](./img/index/F1.6.png)

*Figura 1.6. Placa, nombre del proyecto,...*

</center>

Una vez ponemos nombre, y aunque es opcional se recomienda cumplimentar los distintos apartados, y hacemos clic en el botón “Nuevo proyecto” entramos en el entorno de programación para el nuevo proyecto. Nos encontramos con la pantalla de la Figura 1.7 que está autodescrita.

<center>

![Entorno de programación](./img/index/F1.7.png)

*Figura 1.7. Entorno de programación*

</center>

Ya es posible guardar nuestros bloques favoritos de ArduinoBlocks en la mochila y llevarlos siempre con nosotros o usarla para compartir bloques entre nuestros proyectos. En este [enlace](https://twitter.com/ArduinoBlocks/status/1506352610059689988?s=20&t=GzAqgtY4gySw5FPZgOOzjA) tienes un video que lo explica de forma gráfica.


## <FONT COLOR=#007575>**ArduinoBlocks Connector**</font>
ArduinobBloks genera el código de Arduino a partir de los bloques. El programa copia y sube nuestra programación a la placa gracias a la aplicación ArduinoBlocks Connector. Si no ejecutamos ArduinoBlocks Connector, podremos programar y acceder a la plataforma ArduionBlocks, pero no podremos subir nuestro programa a la placa. Así pues, es necesario instalarlo en nuestro ordenador, y ejecutarlo cuando hagamos uso de la plataforma.

Actualmente, está disponible la versión 5 para estos sistemas operativos: Windows, Ubuntu, MacOS, Chromebook y Raspberry Pi, como vemos en la Figura 1.8.

<center>

![Disponibilidad de ArduinoBlocks Connector](./img/index/F1.8.png)

*Figura 1.8. Disponibilidad de ArduinoBlocks Connector*

</center>

## <FONT COLOR=#007575>**Sensores**</font>
Los sensores permiten recabar información para que sea procesada por la placa y se accionen ciertas programaciones según nuestra finalidad. Hay varios tipos de sensores. Por ejemplo, si vamos al apartado de "Sensores" del menú de herramientas de ArduinoBlocks, para la placa EasyPlug, existen varios. Algunos de ellos los vemos en la Figura 1.9.

<center>

![Algunos tipos de sensores](./img/index/F1.9.png)

*Figura 1.9. Algunos tipos de sensores*

</center>

En la Figura 1.10 vemos el aspecto real de algunos sensores que programaremos.

<center>

![Sensores](./img/index/F1.10.png)

*Figura 1.10. Sensores*

</center>

## <FONT COLOR=#007575>**Actuadores**</font>
Los actuadores se accionan cuando la placa procesa la programación, que puede estar influida por la recogida de datos de algún sensor.

Hay varios tipos de actuadores. Por ejemplo, si vamos al apartado de "actuadores" del menú de herramientas de ArduinoBlocks, para la placa EasyPlug, existen varios. Algunos de ellos los vemos en la Figura 1.11.

<center>

![Algunos tipos de actuadores](./img/index/F1.11.png)

*Figura 1.11. Algunos tipos de actuadores*

</center>

En la Figura 1.12 vemos el aspecto real de algunos actuadores que programaremos.

<center>

![Actuadores](./img/index/F1.12.png)

*Figura 1.12. Actuadores*

</center>
