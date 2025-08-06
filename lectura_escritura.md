## Lectura y escritura de archivos

Python nos permite leer y escribir datos en archivos externos. Podemos abrir archivos en diferentes modos, como lectura ("r"), 
escritura ("w") o anexar ("a"), y realizar operaciones de lectura y escritura.

 

## Lectura de archivos   

Para leer el contenido de un archivo, primero debemos abrirlo utilizando la función open() en modo de lectura ("r"). Luego, podemos leer el contenido del archivo utilizando métodos como read() o readlines().
```py
archivo = open("datos.txt", "r")
contenido = archivo.read()
print(contenido)
archivo.close()
```

En este ejemplo, se abre el archivo "datos.txt" en modo de lectura utilizando open().
Luego, se lee todo el contenido del archivo utilizando el método read() y se almacena en la variable contenido.
Finalmente, se muestra el contenido en la pantalla y se cierra el archivo utilizando el método close().

 

## Escritura de archivos   

Para escribir datos en un archivo, lo abrimos en modo de escritura ("w") utilizando la función open(). 
Si el archivo no existe, se creará automáticamente. Si el archivo ya existe, su contenido se sobrescribirá.
```py
archivo = open("datos.txt", "w")
archivo.write("Hola, mundo!")
archivo.close()
```

En este ejemplo, se abre el archivo "datos.txt" en modo de escritura utilizando open(). 
Luego, se escribe la cadena "¡Hola, mundo!" en el archivo utilizando el método write(). 
Finalmente, se cierra el archivo utilizando el método close().


### 🛑Importante
Es importante cerrar siempre los archivos después de utilizarlos para liberar los recursos del sistema. 

También puedes utilizar la declaración with para manejar la apertura y cierre de archivos de manera automática.

with open("datos.txt", "r") as archivo:
    contenido = archivo.read()
    print(contenido)
En este caso, el archivo se abre utilizando la declaración with y se cierra automáticamente una vez que se sale del bloque with,
incluso si ocurre una excepción.

La entrada y salida de datos en Python nos brinda una gran flexibilidad para interactuar con el usuario y 
manipular archivos externos. Podemos solicitar información al usuario, mostrar resultados en la pantalla y 
leer o escribir datos en archivos de texto. Recuerda siempre manejar adecuadamente la apertura y cierre de archivos, 
y considerar las posibles excepciones que pueden ocurrir durante las operaciones de entrada/salida.
