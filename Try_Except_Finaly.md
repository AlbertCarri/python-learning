## Try   

El bloque try contiene el código que puede generar una excepción. Si ocurre una excepción dentro del bloque try, el flujo de ejecución se transfiere al bloque except correspondiente.

```py
try:
    # Código que puede generar una excepción
    resultado = 10 / 0  # División por cero
    print(resultado)
except ZeroDivisionError:
    print("Error: División por cero")
 ```
<br>

## Except   

El bloque except especifica el tipo de excepción que se desea capturar y manejar. Puedes tener múltiples bloques except para manejar diferentes tipos de excepciones.
```py
try:
    # Código que puede generar una excepción
    resultado = 10 / 0  # División por cero
    print(resultado)
except ZeroDivisionError:
    print("Error: División por cero")
except ValueError:
    print("Error: Valor inválido")
 ```
<br>

## Finally   

El bloque finally es opcional y se ejecuta siempre, independientemente de si ocurrió una excepción o no. Se utiliza comúnmente para realizar tareas de limpieza o liberación de recursos.

```py
try:
    # Código que puede generar una excepción
    archivo = open("archivo.txt", "r")
    # Realizar operaciones con el archivo
except FileNotFoundError:
    print("Error: Archivo no encontrado")
finally:
    archivo.close()  # Cerrar el archivo siempre, incluso si ocurre una excepción
```
<br>

## Excepciones personalizadas   

Además de las excepciones incorporadas en Python, también puedes crear tus propias excepciones personalizadas. Esto es útil cuando deseas manejar situaciones específicas de tu programa.

Para crear una excepción personalizada, debes crear una clase que herede de la clase base Exception o de una de sus subclases.   

```py
def funcion(a):
    if a == 6:
        raise Exception("Descripción del error")

try:
    funcion(6)
except Exception as e:
    print(f"Error:{str(e)}")
```

En este ejemplo, se define una función llamada funcion(). Dentro de la función, se verifica una condición y, si se cumple, se genera una excepción utilizando la declaración raise. En lugar de crear una clase personalizada, se utiliza directamente la clase base Exception para generar la excepción.

Luego, se utiliza un bloque try-except para capturar y manejar la excepción. La variable e se utiliza para acceder a la descripción del error proporcionada al generar la excepción.

El manejo de errores y excepciones es una parte fundamental de la programación en Python. Te permite manejar situaciones inesperadas de manera controlada y evitar que tu programa se bloquee o se detenga abruptamente.

Cuando ocurre un error en tu código, Python genera una excepción. Al utilizar bloques try-except, puedes capturar y manejar estas excepciones de manera adecuada. Puedes especificar diferentes bloques except para manejar distintos tipos de excepciones y realizar acciones específicas en cada caso.

SOA_PYT_fo01.jpg

Además, el bloque finally te permite ejecutar código de limpieza o liberación de recursos, independientemente de si ocurrió una excepción o no. Esto es útil para garantizar que ciertas acciones se realicen siempre, como cerrar archivos o conexiones de base de datos.

