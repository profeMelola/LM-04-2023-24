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

Además, debes crear un tipo simple construido (con restricción) para indicar que el código postal solo puede estar formado por 5 dígitos.


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

Además debes tener en cuenta:

El atributo NIA debe estar formado 6 dígitos y es obligatorio.
El atribto ciclo es opcional y con valor por defecto DAW

# Ejercicio 3

Crea un XML y su correspondiente schema validador para guardar la siguiente información de los empleados:
- atributo código short obligatorio
- nombre string
- apellidos string
- telefonos del empleado opcional
- máximo 1 de tipo string
- si es de un telefono movil tendrá el atributo booleano movil a true
- fecha contratación yyyy-mm-dd, sueldo float.

**Requisitos:**

- Tendremos un XML con un elemento root llamado empleados que contendrá al menos un empleado.
- El nombre tendrá una longitud máxima de 10 (restricción).
- teléfonos será un nodo o elemento complejo que contendrá elementos hijos telefono.
- El elemento teléfono puede aparecer como máximo 4 veces y es opcional. Si el elemento teléfono va a guardar un móvil entonces tendrá un atributo opcional llamado móvil con valor igual a true.

# Ejercicio 4

Crea un XML y su correspondiente schema validador para guardar la siguiente información de pedidos:

![image](https://github.com/profeMelola/LM-04-2023-24/assets/91023374/80173212-31ac-4e96-9097-63be4c824985)

Vamos a añadir el tipo simple reutilizable maxLong10 para indicar que la longitud del título como máximo debe ser 10.


## Ejercicio 5
Crea un XML y su correspondiente esquema de validación que sea capaz de representar la información sobre personas.

Se proporciona un fragmento de XML válido. 

Hay que tener en cuenta:
1) Cada persona tiene un DNI único como atributo, aunque es opcional ponerlo.
2) El DNI consta de 8 dígitos y una letra mayúscula al final.
3) Es obligatorio especificar el sexo, y ha de ser mujer, hombre, otro.


![image](https://github.com/profeMelola/LM-04-2023-24/assets/91023374/59773c10-cec5-469a-ad4b-e7381db72060)



## Ejercicio 6
Crea un XML y su correspondiente schema validador que sea capaz de representar la información sobre una lista de compra.


Se proporciona un fragmento de XML válido. 

Hay que tener en cuenta:
1) Los atributos cantidad y tipo son obligatorios.
2) El atributo tipo sólo podrá tener los valores unidad, kg o litro.
3) Al menos debe haber un item.

![image](https://github.com/profeMelola/LM-04-2023-24/assets/91023374/3c2003b5-f521-41b4-8e6a-4e7d7bf944ca)



## Ejercicio 7
Sea el siguiente XML, crea un schema validador, teniendo en cuenta:
1) Al menos habrá una multa.
2) Los elementos de la multa pueden estar desordenados.
3) El expediente ha de ser único y ha de empezar por E y después 5 dígitos.
4) La matrícula tiene 4 dígitos y 3 letras mayúsculas.
5) Las observaciones son opcionales.
6) Pagada sólo puede contener sí o no

![image](https://github.com/profeMelola/LM-04-2023-24/assets/91023374/32dbca01-a1ca-49bc-97af-9e66e2651ee1)

## Ejercicio 8: formulario con agrupaciones

A continuación se muestra el contenido parcial de un formulario de registro:

![image](https://github.com/profeMelola/LM-04-2023-24/assets/91023374/8864d13a-f492-4892-abf4-e9a149cb74c8)

![image](https://github.com/profeMelola/LM-04-2023-24/assets/91023374/fb0c3600-9473-447d-b63b-4ab128f8edcc)





