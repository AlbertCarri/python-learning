## Entradas/salidas   

En Python, la entrada y salida de datos nos permite interactuar con el usuario y manipular archivos. Podemos solicitar información al usuario, mostrar resultados en la pantalla y leer o escribir datos en archivos externos.

Entrada de datos del usuario
Para obtener información del usuario durante la ejecución del programa, podemos utilizar la función input(). Esta función muestra un mensaje en la pantalla y espera a que el usuario ingrese un valor.

```py
nombre = input("Ingresa tu nombre: ")
edad = input("Ingresa tu edad: ")


print("Hola, " + nombre + "!")
print("Tienes " + edad + " años.")
```

En este ejemplo, se solicita al usuario que ingrese su nombre y edad utilizando la función input(). Los valores ingresados se almacenan en las variables nombre y edad, respectivamente. Luego, se utilizan estas variables para mostrar un saludo personalizado en la pantalla.

### 🛑Importante
La función input() siempre devuelve una cadena de texto. Si deseas trabajar con otros tipos de datos, como números enteros o flotantes, debes realizar una conversión explícita utilizando funciones como int() o float().
 
```py
edad = int(input("Ingresa tu edad: "))


if edad >= 18:
    print("Eres mayor de edad.")
else:
    print("Eres menor de edad.")
```

En este ejemplo, se solicita al usuario que ingrese su edad y se convierte el valor ingresado a un número entero utilizando int(). Luego, se utiliza una estructura condicional para verificar si la edad es mayor o igual a 18 y mostrar un mensaje correspondiente.

<br>

## Salida de datos
Para mostrar información en la pantalla, utilizamos la función print(). Esta función toma uno o más argumentos y los muestra en la consola.

Podemos utilizar la f-string (formateo de cadenas) para incrustar variables directamente dentro de una cadena de texto.

```py
nombre = "Juan"
edad = 25


print(f"Hola, mi nombre es {nombre} y tengo {edad} años.")
```

En este caso, las variables se incrustan dentro de la cadena utilizando llaves {} y se precede la cadena con la letra f para indicar que es una f-string.

 
