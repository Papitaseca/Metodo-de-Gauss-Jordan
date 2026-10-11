# Método de Gauss

## Descripción

Este proyecto implementa el **Método de Gauss** para resolver un sistema de ecuaciones lineales mediante una matriz aumentada.

El programa realiza dos etapas principales:

1. **Eliminación gaussiana:** transforma la matriz en una matriz triangular superior, haciendo cero los elementos que se encuentran debajo de la diagonal principal.
2. **Sustitución regresiva:** obtiene las soluciones de las variables comenzando por la última ecuación y avanzando hacia la primera.

## Lenguaje de programación

El proyecto está desarrollado en **Java**.

## Estructura del proyecto

- `src/gauss/Defmatrizz.java`: contiene la matriz aumentada del sistema de ecuaciones.
- `src/gauss/Gauss.java`: contiene los métodos para realizar la eliminación gaussiana y la sustitución regresiva.
- `src/gauss/Lanzador_gaus.java`: inicia el proceso, llama a los métodos y muestra las soluciones en consola.
- `src/Main.java`: clase generada inicialmente por IntelliJ IDEA.

## Requisitos

- Java instalado en el equipo.
- Un entorno de desarrollo compatible con Java, como IntelliJ IDEA, o una terminal con el compilador `javac`.

## Compilación y ejecución

### Opción 1: IntelliJ IDEA

1. Abrir el proyecto en IntelliJ IDEA.
2. Verificar que el proyecto tenga configurado un JDK de Java.
3. Abrir `src/gauss/Lanzador_gaus.java`.
4. Ejecutar el método `main` de `Lanzador_gaus`.
5. Revisar las soluciones mostradas en la consola.

### Opción 2: Terminal

Desde la carpeta del proyecto, compilar las clases del paquete `gauss`:

```bash
javac -d out src/gauss/Defmatrizz.java src/gauss/Gauss.java src/gauss/Lanzador_gaus.java
```

Después ejecutar el programa con:

```bash
java -cp out gauss.Lanzador_gaus
```

## Ejemplo de prueba

La matriz utilizada por el programa es:

```text
[ 3.0  -0.1  -0.2   7.85 ]
[ 0.1   7.0  -0.3 -19.30 ]
[ 0.3  -0.2  10.0  71.40 ]
```

Al ejecutar el programa se obtiene una salida equivalente a:

```text
Soluciones del sistema:
x1=3.0
x2=-2.5
x3=7.0
```

## Autor

Actividad práctica de la materia **Métodos Numéricos**, Unidad 3: Método de Gauss.
