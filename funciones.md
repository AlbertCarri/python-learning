## Funciones
def funcion(a,b)
    return a + b


## Args (*valores)   
Todos los *valores arman una tupla   

```python
def calcular_media(*numeros):
    suma = sum(numeros)
    cantidad = len(numeros)
    media = suma/cantidad
    return media


print("Media:", calcular_media(10, 20, 30, 40))
 ``` 
