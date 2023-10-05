## Integrantes 
- Roman Tomas
- Novach Jeronimo
- Sotelo Lucas


## Proyecto: Contador de 0 a 99 con Display 7 Segmentos y Multiplexación.
![Tinkercad](circuito_spd.png)


## Descripción
Nuestro proyecto consiste en crear un contador desde el 0-99 utilizando 2 displays de 7 segmentos y la tecnica de Multiplexacion. Contiene 3 pulsadores con funcionalidades distintas; Uno de ellos Suma el contador, Otro resta y el ultimo resetea el contador a 0. 

## Función principal
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






