# Actividad 1  
  
### Ejercicio 1  
  
¿Cuántos estados diferentes se pueden representar usando N bits?  
  
1 bit = 2 estados  
2 bits = 4 estados  
3 bits = 8 estados  
n bits = $2^n$  
  
### Ejercicios de conversión

1. Convierte el número decimal 22 a binario.  
2. ¿Cuál es el resultado en decimal del número binario 10110?  
3. Escribe un programa en Python que convierta un número decimal introducido por el usuario a binario.  

### Respuestas

1.  
Decimal: 22  

22 ÷ 2 = 11, residuo 0  
11  ÷ 2 = 5, residuo 1  
5  ÷ 2 = 2, residuo 1  
2  ÷ 2 = 1, residuo 0   
1  ÷ 2 = 0, residuo 1   
(Residuos de abajo hacia arriba)  
  
Binario:  10110  

2. 
Binario: 10110  

$ 1*(2^4) + 0*(2^3) + 1*(2^2) + 1*(2^1) + 0*(2^0)= 16 + 0 + 4 + 2 + 0 = 22 $

### Ejercicios

1. ¿Qué número binario representa el carácter 'C' en ASCII?

### Respuestas

1. C = 67  

### Ejercicios

1. ¿Cuántos bytes se necesitan para almacenar la palabra “Hola” en ASCII?  

2. ¿Cuántos bits hay en 5 KB?  

### Respuestas

1. Se necesitan 4 bytes  

2. 40960 bits en 5 KB

### Ejercicios  
  
1. Convierte el número decimal 255 a hexadecimal.  
2. ¿Cuál es el valor hexadecimal de la secuencia binaria 11010110?  

### Respuestas

1. 255/15 = 15, residuo 15  
= FF
2. 1101 y 0110  
= D6  
  
## 4. Ejercicios Finales de Repaso  
  
1. Explica, en tus propias palabras, por qué es necesario que las computadoras representen los datos en binario.  
2. Convierte el número binario 10011011 a decimal y a hexadecimal.  
3. Investiga y describe cómo se representa una imagen en formato PNG en el disco.  
4. Analiza la siguiente situación: ¿Qué sucede si intentas almacenar un número mayor al que puede representar un byte (por ejemplo, 300)? ¿Cómo lo maneja Python?  

### Respuestas  

1. Las computadoras estan compuestas de millones de interruptores que solo pueden estar prendidos o apagados, esto hace que se tenga que utilizar un sistema compuesto de 2 salidas unicamente.  
  
2. Decimal: 155
Hexagesimal: 1001 y 1011 = 9B  
  
3. El formato PNG (Portable Network Graphics) representa imágenes en el disco como archivos binarios estructurados en bloques, utilizando compresión sin pérdida (método "Deflate") para guardar cada píxel original sin perder calidad. Se caracteriza por soportar fondos transparentes (canal alfa), imágenes a color verdadero (hasta 48 bits) o escala de grises, y organizar los datos en chunks (fragmentos) que definen la imagen.  
  
4. Python asigna dinámicamente más bytes en memoria para almacenar números grandes sin perder precisión ni truncar el valor, superando el límite estándar de 8 bits. 