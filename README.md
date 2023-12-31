## :construction_worker: Integrantes 
- Roman Tomas
- Novach Jeronimo
- Sotelo Lucas


## 1° Parte - Proyecto: Contador de 0 a 99 con Display 7 Segmentos y Multiplexación.
![Tinkercad](circuito_spd.png)


## :page_with_curl: Descripción
La primera parte de nuestro proyecto consiste en crear un contador desde el 0-99 utilizando 2 displays de 7 segmentos aplicando la tecnica de Multiplexacion'. Contiene 3 pulsadores con funcionalidades distintas; uno de ellos suma el contador, otro resta y el ultimo resetea el contador a 0.
Ademas, incluye mecanismos para evitar rebotes en los pulsadores!<br>
<br>
La tecnica de multiplexación la utilizamos para combinar múltiples señales de datos en un único canal de transmisión. Esto nos permitio transmitir más información de manera eficiente a través de un medio de transmisión limitado. Hemos aplicado la multiplexacion por division de tiempo (TDM) alternando la activación de cada display de manera rápida, lo que crea la ilusión de que ambos están encendidos al mismo tiempo, pero en realidad, solo uno se enciende en un momento dado. Esto nos permitio mostrar información en ambos displays con un número limitado de pines de salida del Arduino.

## :star: Función principal
Esta funcion se encarga de encender y apagar los leds que se necesiten para formar el numero que corresponde con el contador en cada caso. 

a, b, c, d, e, f, g son #define que utilizamos para agregar los leds de los displays, asociandolo a pines de la placa arduino.

~~~ C++ (lenguaje en el que esta escrito)
void mostrar_digito(int digit){
  
    digitalWrite(a,HIGH);
    digitalWrite(b,HIGH);
    digitalWrite(c,HIGH);
    digitalWrite(d,HIGH);
    digitalWrite(e,HIGH);
    digitalWrite(f,HIGH);
    digitalWrite(g,LOW);
  
    switch(digit){
      
        case 1:
            digitalWrite(a,LOW);
            digitalWrite(b,HIGH);
            digitalWrite(c,HIGH);
            digitalWrite(d,LOW);
            digitalWrite(e,LOW);
            digitalWrite(f,LOW);
            digitalWrite(g,LOW);
            break;
        case 2:
            digitalWrite(a,HIGH);
            digitalWrite(b,HIGH);
            digitalWrite(c,LOW);
            digitalWrite(d,HIGH);
            digitalWrite(e,HIGH);
            digitalWrite(f,LOW);
            digitalWrite(g,HIGH);
            break;
        case 3:
            digitalWrite(a,HIGH);
            digitalWrite(b,HIGH);
            digitalWrite(c,HIGH);
            digitalWrite(d,HIGH);
            digitalWrite(e,LOW);
            digitalWrite(f,LOW);
            digitalWrite(g,HIGH);
            break;
        case 4:
            digitalWrite(a,LOW);
            digitalWrite(b,HIGH);
            digitalWrite(c,HIGH);
            digitalWrite(d,LOW);
            digitalWrite(e,LOW);
            digitalWrite(f,HIGH);
            digitalWrite(g,HIGH);
            break;
        case 5:
            digitalWrite(a,HIGH);
            digitalWrite(b,LOW);
            digitalWrite(c,HIGH);
            digitalWrite(d,HIGH);
            digitalWrite(e,LOW);
            digitalWrite(f,HIGH);
            digitalWrite(g,HIGH);
            break;
        case 6:
            digitalWrite(a,HIGH);
            digitalWrite(b,LOW);
            digitalWrite(c,HIGH);
            digitalWrite(d,HIGH);
            digitalWrite(e,HIGH);
            digitalWrite(f,HIGH);
            digitalWrite(g,HIGH);
            break;
        case 7:
            digitalWrite(a,HIGH);
            digitalWrite(b,HIGH);
            digitalWrite(c,HIGH);
            digitalWrite(d,LOW);
            digitalWrite(e,LOW);
            digitalWrite(f,LOW);
            digitalWrite(g,LOW);
            break;
        case 8:
            digitalWrite(a,HIGH);
            digitalWrite(b,HIGH);
            digitalWrite(c,HIGH);
            digitalWrite(d,HIGH);
            digitalWrite(e,HIGH);
            digitalWrite(f,HIGH);
            digitalWrite(g,HIGH);
            break;
        case 9:
            digitalWrite(a,HIGH);
            digitalWrite(b,HIGH);
            digitalWrite(c,HIGH);
            digitalWrite(d,HIGH);
            digitalWrite(e,LOW);
            digitalWrite(f,HIGH);
            digitalWrite(g,HIGH);
            break;
      }
  }
~~~
---

## 2° Parte - Proyecto: Modificación con Interruptor Deslizante y Números Primos.
![Tinkercad](circuito_spd_2da.png)


## :page_with_curl: Descripción
En la segunda parte de nuestro proyecto realizamos las siguientes modificaciones:<br>

:triangular_flag_on_post: ELIMINADOS:
- Boton reset --> Se encargaba de setear el contador a 0 con el fin de reiniciar el programa.

:heavy_check_mark: AGREGADOS:
- Interruptor deslizante o Switch --> Determina los valores que se mostraran en nuestros displays. Lado izquierdo: El programa seguira funcionando de la misma forma que la parte 1. Lado derecho: se mostraran los numeros primos existentes dentro del rango 0-99 en funcion de los botones que se utilicen en cada momento.
- Sensor de temperatura [TMP36] --> Interpreta la temperatura en una escala que va desde -50°C hasta 450°C. Determina si el programa muestra u oculta el valor a mostrar en los visualizadores segun la temperatura registrada. Si la temperatura es mayor a 74°C o menor a 1°C los displays ocultan el valor a mostrar, caso contrario lo muestran.

## 3° Parte - Proyecto: Implementacion de fotodiodo.
![Tinkercad](tercera_parte_spd.png)
## :page_with_curl: Descripción
Un fotodiodo es un dispositivo que convierte la luz incidente en una señal eléctrica, debido a su construccion, se comportan como celulas-fotovoltaicas, nuestra intencion al agregar este componente fue que nuestro programa prenda los visualizadores unicamente si recibe algun tipo de luz (ya sea visible o infrarroja), es decir, utilizamos lo que genero (una pequeña corriente que supere cierto valor especifico) para ello.


## :pushpin: Links al proyecto
- [1° Parte Proyecto](https://www.tinkercad.com/things/eAtVA3PDnj8)
- [2° Parte Proyecto](https://www.tinkercad.com/things/gFwOfAjB9RF)
- [3° Parte Proyecto](https://www.tinkercad.com/things/2bMBr4uYVbG)
---

### :point_down: Fuentes

- [Tutorial](https://www.youtube.com/watch?v=_Ry7mtURGDE&list=PL7LaR6_A2-E11BQXtypHMgWrSR-XOCeyD&index=4).
- [Como utilizar Fotodiodo](https://www.youtube.com/watch?v=r9B_tdsA1t8).
- [Insertar Imagen](https://www.youtube.com/watch?v=lWeEF5fmdko).
- [Emojis](https://gist.github.com/rxaviers/7360908).

---






