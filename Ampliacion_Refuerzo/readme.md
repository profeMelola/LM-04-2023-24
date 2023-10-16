# Ejercicio 1: temperaturas

![image](https://github.com/profeMelola/LM-04-2023-24/assets/91023374/1a1ae0b7-8758-4363-8a00-64ed70e00329)


# Ejercicio 2: panel de vuelos

Si para representar la siguiente información ficticia:

![image](https://github.com/profeMelola/LM-04-2023-24/assets/91023374/c53f2f68-66bd-42e9-9807-dcf0210ecb35)

se ha escrito el siguiente documento XML:

```
<?xml version="1.0" encoding="UTF-8"?>
<aeropuerto>
   <nombre>JFK</nombre>
   <vuelos>
      <vuelo código="V22" estado="R">
         <diario />
         <origen>New York</origen>
         <destino>Chicago</destino>
         <hora-salida>09:30:00</hora-salida>
         <hora-llegada>11:30:00</hora-llegada>
      </vuelo>
      <vuelo código="V23" estado="C">
         <origen>New York</origen>
         <destino>Miami</destino>
         <hora-salida>10:15:00</hora-salida>
         <hora-llegada>11:15:00</hora-llegada>
      </vuelo>
   </vuelos>
   <fecha>2013-12-20</fecha>
</aeropuerto>
```

Escribir el código del archivo "aeropuerto.xsd" que permita validarlo, teniendo en cuenta que:

- El nombre del aeropuerto, los vuelos y la fecha pueden aparecer en distinto orden.
- Se tiene que indicar que el código ha de ser único y obligatorio para cada vuelo.
- Haciendo uso pattern indicar que los posibles estados de un vuelo son C (Cancelado), E (En hora), R (Retrasado). Dicha restricción sólo debe poder ser utilizada por el atributo estado. El valor por defecto debe ser E.
- Debe permitirse aparecer desde cero hasta ilimitados elementos vuelo y, para cada uno de ellos, se tiene que guardar la información en el mismo orden en el que aparece en el panel.
- Para indicar si un vuelo es diario, se debe utilizar un elemento vacío que, respecto a cada vuelo, podrá aparecer (en el caso de sí ser diario) o no aparecer (en el caso contrario).
- Respecto a los elementos nombre, origen, destino, hora-llegada, hora-salida y fecha, cada uno de ellos debe definirse del tipo que se considere más apropiado, de entre los proporcionados por XML Schema.
