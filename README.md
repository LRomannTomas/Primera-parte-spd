## Integrantes 
- Roman Tomas
- Novach Jeronimo
- Sotelo Lucas


## Proyecto: Contador de 0 a 99 con Display 7 Segmentos y Multiplexación.
![Tinkercad](circuito_spd.png)


## Descripción
Nuestro proyecto consiste en crear un contador desde el 0-99 utilizando 2 displays de 7 segmentos y la tecnica de Multiplexacion. Contiene 3 pulsadores con funcionalidades distintas; Uno de ellos Suma el contador, Otro resta y el ultimo resetea el contador a 0. 

## Función principal
Esta funcion se encarga de encender y apagar los leds.

B0, B1, B2, B3 son #define que utilizamos para agregar los leds, asociandolo a pines de la placa arduino.

(Breve explicación de la función)

~~~ C (lenguaje en el que esta escrito)
void EncenderBinario(int estado3, int estado2,int estado1,int estado0)
{
  digitalWrite(B3,estado3);
  digitalWrite(B2,estado2);
  digitalWrite(B1,estado1);
  digitalWrite(B0,estado0);
}
~~~

## :robot: Link al proyecto
- [proyecto](https://www.tinkercad.com/things/aOYiibnDjWu)
## :tv: Link al video del proceso
- [video](https://www.youtube.com/watch?v=VyGjE8kx-O0)

---
### Fuentes
- [Consejos para documentar](https://www.sohamkamani.com/how-to-write-good-documentation/#architecture-documentation).

- [Lenguaje Markdown](https://markdown.es/sintaxis-markdown/#linkauto).

- [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).

- [Tutorial](https://www.youtube.com/watch?v=oxaH9CFpeEE).

- [Emojis](https://gist.github.com/rxaviers/7360908).

---






