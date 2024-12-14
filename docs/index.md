# WLED Shield V2

Placa controladora para LEDs direccionables de 5V, características avanzadas con conectividad wi-fi. 

## La placa
 

-	Conectividad directa de 2 tiras led con patrones de iluminación independientes, programables y configurables.

-	Software WLED traducido por nosotros al español y pre-configurado para la placa.

-	Alimentación de 5V DC via USB tipo C con un cargador de teléfono o mediante cable SATA de 15 pines (opcional para colocar en una PC gaming).

-	2 salidas o segmentos independientes para tiras de 5 V para controlar LEDs NeoPixel (WS2812B, WS2811, SK6812). Fan coolers RGB direccionales. Etc.

-	2 botones configurables desde la interfaz: 
    *	1 botón sobre la placa: SW1 (GPIO9)
    *	1 botón opcional externo mediante el conector J5 (GPIO9).  

-	El software incluido incluye 3 mods instalados y preconfigurados para la placa:

    *	Autosave que guarda el último estado de la configuración.
    *	Display de 4 líneas para conectar opcionalmente un display en el conector J4.
    *	Encoder opcional para conectar en J3.  

## Pines
## WLED  

<p><img src="https://kno.wled.ge/assets/images/ui/headers/macbook-pro-space-gray-on-the-wooden-table.jpg" width="50%"><img src="https://kno.wled.ge/assets/images/ui/headers/walking-with-iphone-x.jpg" width="50%"></p>

WLED es el software que utiliza la placa, la página oficial y la que ofrece la mayor documentación es la siguiente: [https://kno.wled.ge](https://kno.wled.ge).

![Texto alternativo](https://kno.wled.ge/assets/images/ui/headers/wled_logo_akemi.png)


### Características
 
*	Biblioteca WS2812FX integrada con más de 100 efectos especiales.
*	Efectos FastLED y 50 paletas de colores.
*	Interfaz web moderna con controles de color, efectos y segmentos.
*	Segmentos: permite configurar diferentes efectos y colores en distintas partes de los LEDs.
*	Página de configuración: ajustes accesibles a través de la red.
*	Modo punto de acceso (AP) y estación: incluye AP de respaldo automático.
*	Hasta 3 salidas LED por instancia de ESP8266 y 10 salidas LED por instancia de ESP32. (nuestra placa al ser reducida tiene 2 salidas físicas, sin embargo se pueden obtener más ya que presenta accesibilidad a todos los pines).
*	Soporte para tiras LED RGBW.
*	Hasta 250 presets de usuario para guardar y cargar colores/efectos fácilmente, con soporte para ciclos automáticos.
*	Los presets pueden ejecutar llamadas API automáticamente.
*	Función de luz nocturna (se atenúa gradualmente).
*	Actualización completa de software por OTA (HTTP + ArduinoOTA), con opción de protección por contraseña.
*	Límite de brillo automático configurable para un funcionamiento más seguro.
*	Configuración basada en sistema de archivos para facilitar el respaldo de presets y configuraciones.
*	Integración nativa con Home Assistant: inicia la configuración de integración nativa.

### Comunicación
-	Aplicaciones móviles desarrolladas por la comunidad:
-	Aplicación nativa de WLED creada por Moustachauve:
-	Para Android [Fuente]
-	Para iOS [Fuente]
-	APIs de solicitudes JSON y HTTP.
-	MQTT.
-	Blynk IoT.
-	E1.31, Art-Net, DDP y TPM2.net.
-	Hyperion.
-	Realtime UDP.
-	Control por voz con Alexa (incluye ajuste de brillo y color).
-	Sincronización con luces Philips Hue.
-	Adalight (Ambilight para PC vía serial) y TPM2.
-	Sincronización del color entre múltiples dispositivos WLED (notificador UDP).
-	Mandos infrarrojos (requiere receptor y mando RGB de 24 teclas).
-	Temporizadores simples/programación (hora desde NTP, soporta zonas horarias/DST).

## Commands

* `mkdocs new [dir-name]` - Create a new project.
* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs build` - Build the documentation site.
* `mkdocs -h` - Print help message and exit.

## Project layout

    mkdocs.yml    # The configuration file.
    docs/
        index.md  # The documentation homepage.
        ...       # Other markdown pages, images and other files.
