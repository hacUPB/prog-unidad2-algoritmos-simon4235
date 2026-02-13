# Actividad 2

## Ejercicio 1  
  
Investiga cuáles son los símbolos que se utilizan para representar cada operación de un algoritmo con un diagrama de flujo. Asegúrate de que la fuente es confiable, discute lo que encontraste con tus compañeros y con el profe. Cuando estés seguro/a de tener los símbolos correctos, consigna la información en la bitácora.

### Símbolos  
  
![Simbolos diagrama de flujo](./Imagenes/Simbolos_diagrama.png)  

## Ejercicio 2  
  
Analicemos el siguiente problema y representemos su solución mediante un algoritmo secuencial.  
  
- Construye un algoritmo que, al recibir como datos **el ID** del empleado y los seis primeros sueldos del año, calcule el ingreso total semestral y el promedio mensual, e imprima el ID del empleado, el ingreso total y el promedio mensual.  
  
Entradas:  
|Nombre|Descripción|
|-|-|  
|ID|Identificador del empleado (numérico)|  
|S1, S2, S3, S4, S5, S6|Los sueldos de los 6 meses (numérico)|  
  
Datos intermedios:
|Nombre|Descripción|  
|-|-|  
  
Salidas:
|Nombre|Descripción|  
|-|-|  
|Prom|Promedio mensual|
|Total|Ingreso total|
|ID| |  

### Pseudocódigo:  

Inicio  
Leer ID, S1, S2, S3, S4, S5, S6  
Total = S1 + S2 + S3 + S4 + S5 + S6  
Prom + Total / 6
Mostrar ID, Total, Prom  
Fin  

### Diagrama de flujo

![Ejercicio ID](./Imagenes/Ejercicio-ID.png)

## Ejercicios  
  
1. Un **acuario** necesita determinar cuántos litros o galones (eso lo decide el usuario) de agua caben en un acuario, pero solo dispone de una cinta métrica (en centímetros). Diseña un algoritmo para solucionar el problema.  
  
Entradas:  
|Nombre|Descripción|
|-|-|  
|Largo|Largo del tanque en cm|  
|Ancho|Ancho del tanque en cm|  
|Alto|Alto del tanque en cm| 
|Unidad|Unidad de medida (Litro o galón) del volumen total| 
  
Datos intermedios:
|Nombre|Descripción|  
|-|-|  
  
Salidas:
|Nombre|Descripción|  
|-|-|  
|Volumen_lt|Volumen total del tanque en litros|  
|Volumen_gal|Volumen total del tanque en galones|   

### Pseudocódigo:  
  
Inicio  
Mostrar “Por favor ingrese las medidas del tanque”  
Leer Largo, Ancho, Alto  
Mostrar “Ingres L para litros y G para galones”  
Leer Unidad  

Volumen = Largo * Ancho * Alto  //en Mililitros  
Volumen_lt = Volumen/1000  //en Litros  

Si Unidad = “G” 

    Volumen_gl = Volumen_lt * 0.26  
    Mostrar Volumen_gl  

Si no 

    Mostrar Volumen_lt 

Fin Si 

Fin

### Diagrama de flujo

![Diagrama Acuario](./Imagenes/Diagrama-acuario.png)  

2. Realice un algoritmo para determinar cuánto se debe pagar por equis cantidad de lápices considerando que si son 1000 o más el costo es de $85 cada uno; de lo contrario, el precio es de $90. Represéntelo con el pseudocódigo y el diagrama de flujo.  

Entradas:  
|Nombre|Descripción|
|-|-|  
|Lapices|Cantidad de lapices|  

Datos intermedios:
|Nombre|Descripción|  
|-|-|  
|Precio|Precio de cada lápiz|  
  
Salidas:
|Nombre|Descripción|  
|-|-|  
|Precio_Total|Precio total de la compra|  

### Pseudocódigo:  
  
Inicio  
Leer Lapices  
si Lapices < 1000  

    Precio = 90

si no

    Precio = 85

Fin si  
Precio_Total = Lapices * Precio  
Mostrar Precio_Final  
Fin  

### Diagrama de flujo

![Diagrama Acuario](./Imagenes/Diagrama-lapices.png)  

3. Un almacén de ropa tiene una promoción: por compras superiores a $250 000 se les aplicará un descuento de 15%, de caso contrario, sólo se aplicará un 8% de descuento. Realice un algoritmo para determinar el precio final que debe pagar una persona por comprar en dicho almacén y de cuánto es el descuento que obtendrá. Represéntelo mediante el pseudocódigo y el diagrama de flujo.  

Entradas:  
|Nombre|Descripción|
|-|-|  
|Compra|El precio de la compra hecha|  

Datos intermedios:
|Nombre|Descripción|  
|-|-|  
  
Salidas:
|Nombre|Descripción|  
|-|-|  
|Precio|Precio total después de aplicar el descuento|  
|Descuento|Descuento aplicado|

### Pseudocódigo:  
  
Inicio  
Leer Compra  
si Compra < $250000  

    Descuento = 0.08
    Precio = Compra - Compra * Descuento  

si no

    Descuento = 0.15
    Precio = Compra - Compra * Descuento  

Fin si  
Mostrar Precio, Descuento   
Fin  

### Diagrama de flujo

![Diagrama Acuario](./Imagenes/Diagrama-descuento.png)  

4. El director de una escuela está organizando un viaje de estudios, y requiere determinar cuánto debe cobrar a cada alumno y cuánto debe pagar a la compañía de viajes por el servicio. La forma de cobrar es la siguiente: si son 100 alumnos o más, el costo por cada alumno es de $65.00; de 50 a 99 alumnos, el costo es de $70.00, de 30 a 49, de $95.00, y si son menos de 30, el costo de la renta del autobús es de $4000.00, sin importar el número de alumnos.  

Entradas:  
|Nombre|Descripción|
|-|-|  
|Alumnos|Numero de alumnos|  

Datos intermedios:
|Nombre|Descripción|  
|-|-|  
  
Salidas:
|Nombre|Descripción|  
|-|-|  
|Precio_Alumno|Precio que cada alumno debe de pagar|  
|Costo_Total|Costo total del viaje|

### Pseudocódigo:  
  
Inicio  
Leer Alumnos  
si Alumnos >= 100  

    Precio_Alumno = $65
    Costo_Total = Alumnos * Precio_Alumno  

si Alumnos =< 99 y Alumnos >= 50  

    Precio_Alumno = $70
    Costo_Total = Alumnos * Precio_Alumno

si Aumnos =< 49 y Alumnos >= 30  

    Precio_Alumno = $95
    Costo_Total = Alumnos * Precio_Alumno

si no

    Costo_Total = $4000
    Precio_Alumno = Costo_Total / Alumnos

Fin si  
Mostrar Precio_Alumno, Costo_Total   
Fin  

### Diagrama de flujo

![Diagrama Acuario](./Imagenes/Diagrama-Excursion.png)  