# Desafios-Python
# Desafio 1
* Escribe un programa que muestre por consola (con un print) los
 * números de 1 a 100 (ambos incluidos y con un salto de línea entre
 * cada impresión), sustituyendo los siguientes:
 * - Múltiplos de 3 por la palabra "fizz".
 * - Múltiplos de 5 por la palabra "buzz".
 * - Múltiplos de 3 y de 5 a la vez por la palabra "fizzbuzz".

 for i in range(1,101):
    if i % 3 == 0 and i % 5 == 0:
         print(f"fizzbuzz {i}\n " )
         
    elif i % 3 == 0: 
        print(f"fizz {i}\n ")
        
    elif i % 5 == 0:
        print(f"buzz {i}\n ")


    <!-- * Correr por consola para ver resultados. -->
-----------------------------------------------------------------
    # Desafio 2
* Escribe una función que reciba dos palabras (String) y retorne
 * verdadero o falso (Bool) según sean o no anagramas.
 * - Un Anagrama consiste en formar una palabra reordenando TODAS
 *   las letras de otra palabra inicial.
 * - NO hace falta comprobar que ambas palabras existan.
 * - Dos palabras exactamente iguales no son anagrama.

def anagrama(p1, p2):
        p1 = p1.lower()
        p2 = p2.lower()

        if p1 == p2:
            return False
        elif sorted(p1) == sorted(p2):
            return True

print(anagrama("Amor", "Roma"))

    <!-- * Correr por consola para ver resultados. -->
-----------------------------------------------------------------
    # Desafio 3
   * Escribe un programa que imprima los 50 primeros números de la sucesión
 * de Fibonacci empezando en 0.
 * - La serie Fibonacci se compone por una sucesión de números en
 *   la que el siguiente siempre es la suma de los dos anteriores.
 *   0, 1, 1, 2, 3, 5, 8, 13...

 def fibonacci():
 n = 50
 a, b = 0, 1
 for _ in range(n):
    yield a
    a, b = b, a + b
print(list(fibonacci()))

    <!-- * Correr por consola para ver resultados. -->
-----------------------------------------------------------------
# Desafio 4
 *Escribe un programa que se encargue de comprobar si un número es o no primo.
 * Hecho esto, imprime los números primos entre 1 y 100.

 for i in range(1, 101):
 if i > 1:
 for j in range(2, i):
 if (i % j) == 0:
 break
 else:
 print(i)
 <!-- * Correr por consola para ver resultados. -->
-----------------------------------------------------------------
# Desafio 4
 * Escribe un programa que se encargue de comprobar si un número es o no primo.
 * Hecho esto, imprime los números primos entre 1 y 100.

 for i in range(1, 100):
    if i % 2 != 0:
        print(f"{i} es primo")

<!-- * Correr por consola para ver resultados. -->
-----------------------------------------------------------------
# Desafio 5
