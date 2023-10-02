# Ejercicio 1
Suponiendo el siguiente XML con su validador integrado dtd, transfórmalo para que sea validado a través de un xml Schema, y crea el Schema correspondiente. 

Ten en cuenta que el Código es numérico y opcional.

```
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE agenda[
<!ELEMENT agenda (contacto*)>
<!ELEMENT contacto (nombre, calle, ciudad, pais, codigo?, vip?)>
<!ELEMENT nombre (#PCDATA)>
<!ELEMENT calle (#PCDATA)>
<!ELEMENT ciudad (#PCDATA)>
<!ELEMENT pais (#PCDATA)>
<!ELEMENT codigo (#PCDATA)>
<!ELEMENT vip EMPTY>
]>
<agenda>
  <contacto>
     <nombre>Pepe García</nombre>
     <calle>C/Ronda, 3</calle>
     <ciudad>Moncófar</ciudad>
     <pais>España</pais>
     <codigo>18465</codigo>
     <vip/>
  </contacto>
  <contacto>
     <nombre>Lola García</nombre>
     <calle>C/Paraiso, 5</calle>
     <ciudad>Ciudad Real</ciudad>
     <pais>España</pais>
  </contacto>
</agenda>

```

# Ejercicio 2

Crea para el siguiente XML un schema validador que sea capaz de representar la información sobre calificaciones de alumnos:

```
<?xml version="1.0" encoding="UTF-8"?>
<estudiantes>
  <estudiante NIA="123456" ciclo="DAW"> 
    <nombre>María</nombre>
    <apellidos>Fernández García</apellidos>    
  </estudiante>
</estudiantes>
```

# Ejercicio 3

Crea un XML y su correspondiente schema validador para guardar la siguiente información de los empleados:
- atributo código short obligatorio
- nombre string
- apellidos string
- telefonos del empleado opcional
- máximo 1 de tipo string
- si es de un telefono movil tendrá el atributo booleano movil a true
- fecha contratación yyyy-mm-dd, sueldo float.

# Ejercicio 4

Crea un XML y su correspondiente schema validador para guardar la siguiente información de pedidos:

![image](https://github.com/profeMelola/LM-04-2023-24/assets/91023374/80173212-31ac-4e96-9097-63be4c824985)

# Ejercicio 5

Crea un XML y su correspondiente esquema de validación que sea capaz de representar la información sobre personas. 

Se proporciona un fragmento de XML válido. Hay que tener en cuenta:

1)	Cada persona tiene un DNI único como atributo, aunque es opcional ponerlo.
2)	El DNI consta de 8 dígitos y una letra mayúscula al final.
3)	Es obligatorio especificar el sexo, y ha de ser mujer u hombre.

