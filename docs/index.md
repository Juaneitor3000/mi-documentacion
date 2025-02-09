# WLED Shield V2

Placa controladora para LEDs direccionables de 5V, características avanzadas con conectividad wi-fi. 

## La placa
 
 <div style="flex: 1; text-align: center; margin: 0 10px;">
    <a href="images/banner wled shield.png" target="_blank">
      <img src="images/banner wled shield.png" alt="Imagen 1" style="max-width: 100%; height: auto;width: auto;">
    </a>
</div>


<div style="display: flex; justify-content: space-between; align-items: center;width: auto;">

  <div style="flex: 1; text-align: center; margin: 0 10px;">
    <a href="images/Screenshot_7.png" target="_blank">
      <img src="images/Screenshot_7.png" alt="Imagen 2" style="max-width: 70%; height: auto;width: auto;">
      <p>Vista Trasera</p>
    </a>
  </div>
  <div style="flex: 1; text-align: center; margin: 0 10px;">
    <a href="images/Screenshot_3.jpg" target="_blank">
      <img src="images/Screenshot_3.jpg" alt="Imagen 3" style="max-width: 80%; height: auto;width: auto;">
      <p>Versión Full</p>
    </a>
  </div>
</div>

-	Conectividad directa de 2 tiras led con patrones de iluminación independientes, programables y configurables.

-	Software WLED traducido por nosotros al español y pre-configurado para la placa.

-	Alimentación de 5V DC via USB tipo C con un cargador de teléfono o mediante cable SATA de 15 pines (opcional para colocar en una PC gaming).

-	2 salidas o segmentos independientes para tiras de 5 V para controlar LEDs NeoPixel (WS2812B, WS2811, SK6812). Fan coolers RGB direccionales. Etc.

-	2 botones configurables desde la interfaz:<br/>
    *	1 botón sobre la placa: SW1 (GPIO 9)
    *	1 botón opcional externo mediante el conector J5 (GPIO 3).<br/><br/>
-	El software incluido incluye 3 mods instalados y preconfigurados para la placa:<br/><br/>
    *	Autosave que guarda el último estado de la configuración.
    *	Display de 4 líneas para conectar opcionalmente un display en el conector J4. El display debe contar con protocolo I2C.
    *	Encoder incremental opcional para conectar en J3 para manipular el menú del display.<br/><br/>
## WLED  
 <div style="flex: 1; text-align: center; margin: 0 10px;">
    <img src="images/wled_logo_akemi.png" alt="Imagen 1" style="max-width: none; height: 100px;width: auto;">
</div>
<p><img src="https://kno.wled.ge/assets/images/ui/headers/macbook-pro-space-gray-on-the-wooden-table.jpg" width="50%"><img src="https://kno.wled.ge/assets/images/ui/headers/walking-with-iphone-x.jpg" width="50%"></p>

WLED es el software que utiliza la placa, la página oficial de los desarrolladores y la que ofrece la mayor documentación es la siguiente: [https://kno.wled.ge](https://kno.wled.ge).

La aplicación para Android se puede descarcar en la play store:





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
- FXLed.
-	Realtime UDP.
-	Control por voz con Alexa (incluye ajuste de brillo y color).
-	Sincronización con luces Philips Hue.
-	Adalight (Ambilight para PC vía serial) y TPM2.
-	Sincronización del color entre múltiples dispositivos WLED (notificador UDP).
-	Mandos infrarrojos (requiere receptor y mando RGB de 24 teclas).
-	Temporizadores simples/programación (hora desde NTP, soporta zonas horarias/DST).

## Primera conexión

Alimentar la placa con un cable para teléfono USB tipo C y un cargador de teléfono. El led rojo se ha de iluminar.

Desde un teléfono celular conectarse a la red WIFI llamada WLED-AP. En caso de ser requerida colocar la clave del punto acceso: WLED1234. Desde allí debe aparecer la página de configuración, en caso de conectarse desde un PC, colocar en el navegador la IP del punto de acceso: 4.3.2.1

Es recomendable pero opcional configurar la red local wifi, añadiendo SSID y password de la red local. Luego de realizado el controlador se reinicia y se conecta a la red local si la señal es suficientemente fuerte, si no puede conectarse entrara de nuevo en modo AP (punto de acceso).

<div style="display: flex; justify-content: space-between; align-items: center;">

  <div style="flex: 1; text-align: center; margin: 0 10px;">
    <img src="images/Screenshot_20241215-045846.jpg" alt="Imagen 2" style="max-width: 70%; height: auto;width: auto;"> 
  </div>
  <div style="flex: 1; text-align: center; margin: 0 10px;">
    <img src="images/Screenshot_20241215-045853.jpg" alt="Imagen 3" style="max-width: 70%; height: auto;width: auto;">
  </div>
</div>

Instalar la app WLED para el teléfono Android desde Google Play:
 <div style="flex: 1; text-align: center; margin: 0 10px;">
  <a href="https://play.google.com/store/apps/details?id=com.aircoookie.WLED" target="_blank">
    <img src="images/google play.png" alt="Imagen 2" style="max-width: 50%; height: auto;width: auto;"> 
  </a>
</div>

## Galería

<div style="display: flex; justify-content: space-between; align-items: center;">

  <div style="flex: 1; text-align: center; margin: 0 10px;">
    <a href="images/IMG_20241215_060320_693.jpg" target="_blank">
      <img src="images/IMG_20241215_060320_693.jpg" alt="Imagen 2" style="max-width: 90%; height: auto;width: auto;">
    </a> 
  </div>
  <div style="flex: 1; text-align: center; margin: 0 10px;">
    <a href="images/IMG_20241210_113155_811.jpg" target="_blank">
      <img src="images/IMG_20241210_113155_811.jpg" alt="Imagen 3" style="max-width: 90%; height: auto;width: auto;">
    </a> 
  </div>
</div>

<div style="display: flex; justify-content: space-between; align-items: center;">

  <div style="flex: 1; text-align: center; margin: 0 10px;">
    <a href="images/IMG_20241215_121028_459.jpg" target="_blank">
      <img src="images/IMG_20241215_121028_459.jpg" alt="Imagen 2" style="max-width: 95%; height: auto;width: auto;">
    </a> 
  </div>
  <div style="flex: 1; text-align: center; margin: 0 10px;">
    <a href="images/IMG_20241210_192843_833.jpg" target="_blank">
      <img src="images/IMG_20241210_192843_833.jpg" alt="Imagen 3" style="max-width: 95%; height: auto;width: auto;">
    </a> 
  </div>
</div>


## Screenshots (capturas de pantalla)

<div style="flex: 1; text-align: center; margin: 0 10px;">
    <a href="images/Screenshot_6.jpg" target="_blank">
      <img src="images/Screenshot_6.jpg" alt="Imagen 1" style="max-width: 95%; height: auto;width: auto;">
    </a>
    <p>Menú principal en PC</p>
</div>


<div style="display: flex; justify-content: space-between; align-items: center;">

  <div style="flex: 1; text-align: center; margin: 0 10px;">
    <img src="images/Screenshot_1.jpg" alt="Imagen 2" style="max-width: 70%; height: auto;width: auto;">
    <p>"Ajustes" en móvil</p>
  </div>
  <div style="flex: 1; text-align: center; margin: 0 10px;">
    <img src="images/Screenshot_2.jpg" alt="Imagen 3" style="max-width: 70%; height: auto;width: auto;">
    <p>Pestaña "Información"</p>
  </div>
</div>

## Videos
<div>
<center>
Letrero led modificado con tiras led WS2812 y el WLED shield:
<iframe width=100% height=100% src="https://www.youtube.com/embed/0LlJ29TlfnQ?si=bu1M_Pl0w9ASbE-H" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
WLED + Hyperion:
<iframe width=100% height=100% src="https://www.youtube.com/embed/_pkXYHH0mGE?si=EDheS6KKrJCtD_Bx" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
Gaming PC con WLED Shield:
<iframe width=100% height=100% src="https://www.youtube.com/embed/LklitRmLoow?si=zknoBuj7EyN5wNJ4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
La placa incluye las conexiones físicas y el software los MODs para conectar una pantalla y un encoder:
<iframe width=100% height=100% src="https://www.youtube.com/embed/ulZnBt9z3TI?si=LG7SQQf3qdyRdVjZ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
WLED + FXled:
<iframe src="https://player.vimeo.com/video/1053010399?h=05dcfa3321" width=100% height=100% frameborder="0" allow="autoplay; fullscreen" allowfullscreen></iframe>
</center>
</div>

## Firmware

Se adjunta el firmware en caso de que se requiera subir nuevamente o actualizar, usar el archivo .bin con el cual desea actualizar junto a la herramienta [Flash download Tool](https://docs.espressif.com/projects/esp-test-tools/en/latest/esp32/production_stage/tools/flash_download_tool.html){target=_blank}.

- WLED V0.14.4 "HOSHI" español, traducido y compilado, incluye mods: AUTOSAVE, FOUR LINES DISPLAY ALT y ENCODER ALT.
- WLED V0.15.0. en español, traducido y compilado, incluye mods: AUTOSAVE, FOUR LINES DISPLAY ALT y ENCODER ALT.

Para versiones originales en ingles se puede usar:

- Instalador web (RECOMENDADO): https://install.wled.me
- [Binarios oficiales](https://github.com/Aircoookie/WLED/releases):  Se pueden subir al microntrolador mediante esptool.py o la herramienta de spressif [Flash download Tool](https://docs.espressif.com/projects/esp-test-tools/en/latest/esp32/production_stage/tools/flash_download_tool.html).

Para mayor información sobre la instalación en inglés: https://kno.wled.ge/basics/getting-started/

## Configuración y presets por defecto

En caso que se requiera o luego de un cambio de firmware, se puede configurar el software WLED a la placa: SHIELD V2 usando los siguientes archivos en el menú seguridad y actualizaciones (Security & Update setup):

- [WLED V0.14.4 configuraciones](https://github.com/Juaneitor3000/WLED_SPANISH/blob/wled_spanish/configuraciones/wled_cfg_default_hoshi.json)
- [WLED V0.14.4 Presets](https://github.com/Juaneitor3000/WLED_SPANISH/blob/wled_spanish/configuraciones/wled_presets_deafult_hoshi.json)

<a href="https://github.com/Juaneitor3000/WLED_SPANISH/blob/wled_spanish/configuraciones/wled_cfg_default_hoshi.json" download>Descargar Archivo</a>
