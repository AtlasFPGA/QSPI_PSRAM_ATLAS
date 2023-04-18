# QSPI_PSRAM_ATLAS

   Es una de las memorias más usadas las PSEUDOSRAM en formato SPI de 4 bit QSPI siendo su tensión de referencia en la alimentación 3v3, su tecnología no es SRAM clasica y necesitan muchas menos celdas para alcanzar tamaños considerables, el integrado escogido W25M512JV se trata de dos módulos internos de 32Mbytes, su configuración 2 x 256Mbit.
   
   La pregunta que se puede plantear es, existe algúna comunidad que de soporte con código en lenguaje descriptor de hardware de estas memorias pseudo SRAM, si la comunidad detrás de Litex:
   
https://github.com/litex-hub/litespi
   
---
Bus de conexión QSPI | nombre señal | numero pines
| :--- | ---: | :---:
Señal  | /CS | 1
Señal  | CLK | 1
Señal  | IO0 | 1
Señal  | IO1 | 1
Señal  | IO2 | 1
Señal  | IO3 | 1

Bus de conexión SPI Dual | nombre señal | numero pines
| :--- | ---: | :---:
Señal  | /CS | 1
Señal  | CLK | 1
Señal  | IO0 | 1
Señal  | IO1 | 1

Bus de conexión SPI | nombre señal | numero pines
| :--- | ---: | :---:
Señal  | /CS | 1
Señal  | CLK | 1
Señal  | MISO | 1
Señal  | MOSI | 1

---
   Al ser memorias de 3V3 su velocidad máxima en SPI es 104Mhz.

   En la página 10 de la descripción del integrado de memoria nos muestra lo plástico que és, permite configuraciones SPI, dual SPI,y la versión con cuatro señales de entrada salida.

https://www.mouser.es/datasheet/2/949/w25m512jv_revd_09052017-1489569.pdf

   Este tipo de memorias son muy usadas desde los microcontroladores ESP32 hasta controladores como los Teensy.
   El factor precio es muy importante actualmente como escoger ua memoria que estén en almacén por ejemplo en mouser vemos que añadir esta memoria de 4bits cuesta menos de 7€, actualmente en el 18 de abril del 2024 son 6,66€.  
   
https://www.mouser.es/ProductDetail/Winbond/W25M512JVEIQ-TR?qs=qSfuJ%252Bfl%2Fd6atrQZjNU60Q%3D%3D

   Cara inferior QSPI ATLAS
![Cara inferior QSPI ATLAS](https://github.com/AtlasFPGA/QSPI_PSRAM_ATLAS/blob/main/FOTOS/ATLAS_QSPI_PSRAM-CAPA-INFERIOR-MUESTRA.jpg)

---

   Cara superior QSPI ATLAS
![Cara superior QSPI ATLAS](https://github.com/AtlasFPGA/QSPI_PSRAM_ATLAS/blob/main/FOTOS/ATLAS_QSPI_PSRAM-CAPA-SUPERIOR-MUESTRA.jpg)

---

   Perspectiva QSPI ATLAS
![Perspectiva QSPI ATLAS](https://github.com/AtlasFPGA/QSPI_PSRAM_ATLAS/blob/main/FOTOS/ATLAS_QSPI_PSRAM-PERSPECTIVA-MUESTRA.jpg)

---

   PCB QSPI ATLAS
![PCB QSPI ATLAS](https://github.com/AtlasFPGA/QSPI_PSRAM_ATLAS/blob/main/FOTOS/PCB_QSPI_ATLAS.png)
