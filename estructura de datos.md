## Resumen rápido:   

| Tipo    | Ordenado | Mutable | Permite duplicados | Claves | Acceso por índice  |
| ------- | -------- | ------- | ------------------ | ------ | ------------------ |
| `list`  | ✅        | ✅       | ✅                  | ❌      | ✅                  |
| `tuple` | ✅        | ❌       | ✅                  | ❌      | ✅                  |
| `set`   | ❌        | ✅       | ❌                  | ❌      | ❌                  |
| `dict`  | ❌/✅\*    | ✅       | ❌ (en claves)      | ✅      | ❌ (solo por clave) |



## 🟦 1. Lista (list)   

📌 Definición:
Una lista es una colección ordenada y mutable (editable). Puede contener elementos duplicados y de cualquier tipo (números, strings, objetos, etc).

📌 Sintaxis:

```python
mi_lista = [1, 2, 3]
```

📌 Características:

* Ordenada (los elementos tienen una posición fija)
* Mutable (se pueden cambiar, agregar o eliminar elementos)
* Puede contener duplicados

📌 Métodos comunes:

```python
.append(x)        # Agrega un elemento al final
.extend(iterable) # Agrega varios elementos
.insert(i, x)     # Inserta x en la posición i
.remove(x)        # Elimina el primer elemento igual a x
.pop(i)           # Elimina y devuelve el elemento en la posición i
.index(x)         # Devuelve la primera posición de x
.count(x)         # Cuenta cuántas veces aparece x
.sort()           # Ordena la lista
.reverse()        # Invierte el orden
.clear()          # Borra todos los elementos
.copy()           # Crea una copia de la lista
```

## 🟨 2. Tupla (tuple)   

📌 Definición:
Una tupla es una colección ordenada e inmutable. También puede contener elementos de cualquier tipo, pero no se puede modificar después de su creación.

📌 Sintaxis:

```python
mi_tupla = (1, 2, 3)
```

📌 Características:

* Ordenada
* Inmutable
* Permite duplicados

📌 Métodos comunes:

```python
.index(x)    # Devuelve la primera posición de x
.count(x)    # Cuenta cuántas veces aparece x
```

➡️ Tiene pocos métodos porque no se puede modificar.

## 🟩 3. Conjunto (set)   

📌 Definición:   

Un conjunto es una colección no ordenada y sin elementos duplicados. Se usa para operaciones de teoría de conjuntos (uniones, intersecciones, etc.).

📌 Sintaxis:

```python
mi_conjunto = {1, 2, 3}
```

📌 Características:

* No ordenado
* No permite duplicados
* Mutable (se puede modificar, pero no se accede por índice)

📌 Métodos comunes:

```python
.add(x)           # Agrega un elemento
.update(iterable) # Agrega varios elementos
.remove(x)        # Elimina x, lanza error si no está
.discard(x)       # Elimina x, sin error si no está
.pop()            # Elimina y devuelve un elemento arbitrario
.clear()          # Borra todos los elementos
.copy()           # Copia el conjunto
.union(otro_set)             # Unión
.intersection(otro_set)      # Intersección
.difference(otro_set)        # Diferencia
.symmetric_difference(otro_set) # Diferencia simétrica
```

## 🟥 4. Diccionario (dict)   

📌 Definición:   

Un diccionario es una colección de pares clave:valor. Las claves deben ser únicas e inmutables.

📌 Sintaxis:

```python
mi_diccionario = {"nombre": "Alberto", "edad": 52}
```

📌 Características:

* Desordenado (aunque desde Python 3.7 mantiene el orden de inserción)
* Acceso rápido a los valores por su clave
* Mutable

📌 Métodos comunes:

```python
.keys()           # Devuelve las claves
.values()         # Devuelve los valores
.items()          # Devuelve pares clave:valor
.get(clave)       # Obtiene un valor (sin error si no existe)
.update(dict2)    # Agrega o actualiza pares
.pop(clave)       # Elimina una clave y devuelve su valor
.popitem()        # Elimina y devuelve el último par
.clear()          # Borra todo
.copy()           # Copia el diccionario
```
