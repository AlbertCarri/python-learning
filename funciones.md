## Funciones
def funcion(a,b)
    return a + b


## Args (Argumentos Posicionales Variables) se representan con * + argumento  
Todos los *valores arman una tupla   

```python
def calcular_media(*numeros):
    suma = sum(numeros)
    cantidad = len(numeros)
    media = suma/cantidad
    return media


print("Media:", calcular_media(10, 20, 30, 40))
 ```

## Funciones lambda   

```python
sumar = lambda x: x + 3

print("Sumarle 3 a un numero", sumar(5))
```
## Documentación de funciones (docstrings)   

Es una buena práctica documentar nuestras funciones utilizando docstrings. Los docstrings son cadenas de texto que describen el propósito, los parámetros y el valor de retorno de una función. Se colocan inmediatamente después de la definición de la función y se encierran entre triples comillas dobles.

```python
def area_rectangulo(base, altura):
    """
    Calcula el área de un rectángulo.


    Args:
        base (float): La base del rectángulo.
        altura (float): La altura del rectángulo.


    Returns:
        float: El área del rectángulo.
    """
    return base * altura
```


