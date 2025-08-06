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


