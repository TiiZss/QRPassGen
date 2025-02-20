# QRPassGen - Generador de tarjetas de embarque

![Static Badge](https://img.shields.io/badge/TiiZss-BullSec-blue)
[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/donate/?business=AC5N3XX2KGY2S&no_recurring=0&item_name=Seguir+con+el+desarrollo+de+la+herramienta&currency_code=EUR)

![GitHub License](https://img.shields.io/github/license/TiiZss/QRPassGen)
<img src="https://img.shields.io/github/deployments/TiiZss/QRPassGen/github-pages?label=deployment"> 
<img src="https://img.shields.io/github/v/release/TiiZss/QRPassGen?label=version"> 
<img src="https://img.shields.io/github/stars/TiiZss/QRPassGen">
![GitHub all releases](https://img.shields.io/github/downloads/TiiZss/QRPassGen/total) <br />

## Introducción y funcionaiento

Existen dos estándares que utilizan las aerolíneas para poder leer la informacion de una tarjeta de embarque de manera mecanizada: 
* PDF417 - Código de barrar 1D
* AZTEC - Código QR 2D

Los datos de las tarjetas de embarque, por tanto se codifican según un [estándar específico de la IATA](https://www.iata.org/contentassets/1dccc9ed041b4f3bbdcf8ee8682e75c4/2021_03_02-bcbp-implementation-guide-version-7-.pdf) en uno de estos 2 formatos siguiedo un determinado formato, por ejemplo: Benito Camela que tiene como localizador RC2025 se vería así:

```
M1CAMELA/BENITO ERC2025 MAD ... 203A010F0001 100
  ------ ------  ------
     |     |       |
 Apellido  | Localizazor  ...
           |
        Nombre
```
La informacion de esa cadena de texto se introduce posteriormente en el tipo elegido para que los organismos de inspección en los aeropuertos puedan leerla con el pertinente lector.

Vemos por tanto que existe un formato específico concreto que contienen los códigos de barras y los QR.

El contenido además es texto sin procesar, en claro, sin cifrar y por tanto puede leerse y manipularse para introducir otra información y generar un código "nuevo".


## Otra Informacion de utilidad
* Búsqueda de [códigos de aerolíneas y aeropuertos](https://www.iata.org/en/publications/directories/code-search/)
* International Air Transport Association airport code: http://www.airportcodes.org/
* [Airport Codes](https://web.archive.org/web/20250211075753/http://www.airportcodes.org/)
* [IATA Airport Codes](https://www.nationsonline.org/oneworld/IATA_Codes/airport_code_list.htm) - no oficial
* [OpenFlights](https://openflights.org/)
* [OpenFlights Data](https://github.com/jpatokal/openflights/tree/master/data)
* [Barcode Writer in JS](https://github.com/metafloor/bwip-js)
  
# Descargo de responsabilidad
En este sitio web se demuestra una vulnerabilidad de seguridad conocida, pero no divulgada públicamente. La herramienta utilizada para esta demostración ha sido desarrollada exclusivamente con fines educativos y de concienciación sobre los riesgos de seguridad informática.
El propietario y los colaboradores de este sitio web no se hacen responsables del uso que terceros puedan dar a esta información y herramienta. La explotación de vulnerabilidades de seguridad sin el consentimiento del propietario del sistema afectado es ilegal y puede acarrear consecuencias legales.
Se prohíbe expresamente el uso de esta herramienta para fines distintos a los educativos y de concienciación.
