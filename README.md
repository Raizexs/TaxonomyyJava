
# Sistema de Evaluación Basado en la Taxonomía de Bloom (Java GUI)

Este proyecto es una aplicación de escritorio desarrollada en **Java con Swing** para la asignatura **Paradigmas de Programación**. 

Su objetivo es gestionar y aplicar pruebas compuestas por ítems clasificados según la **Taxonomía de Bloom**, facilitando la administración de evaluaciones y la revisión de respuestas.

## Tecnologías Utilizadas

- **Lenguaje**: Java (JDK 23)
- **Interfaz Gráfica (GUI)**: Java Swing (GroupLayout)
- **Entorno de desarrollo**: IntelliJ IDEA

## Funcionalidades Principales

- **Carga de Ítems**: Permite cargar ítems de prueba desde un archivo de texto, mostrando la cantidad total y el tiempo estimado de la evaluación.
- **Aplicación de Prueba**: Presenta los ítems uno por uno en una interfaz gráfica. El usuario puede responder, avanzar, retroceder y mantener sus respuestas.
- **Revisión de Respuestas**: Al finalizar, se muestra un resumen con el porcentaje de aciertos por nivel de Bloom y tipo de ítem, además de permitir revisar cada pregunta individualmente.

## Alcances y Restricciones

- **Modularización**: El proyecto está dividido en paquetes `backend` (lógica del sistema) y `frontend` (interfaz gráfica), los cuales se comunican mediante un mecanismo de notificación-suscripción.
- **Validación de Archivo**: Se implementa manejo de errores por medio de excepciones para detectar problemas de formato en el archivo de ítems.
- **Tipos de Ítems Soportados**: Ítems de selección múltiple y verdadero/falso.

## Formato del Archivo de Ítems

El archivo de ítems debe ser un archivo `.txt` donde cada línea representa un ítem, con campos separados por punto y coma (`;`).

### Estructura de cada línea

```
Tipo;Nivel_Bloom;Enunciado;Opciones|Separadas|Por|Barra;Respuesta_Correcta;Tiempo_Estimado
```

### Ejemplo:

```
SELECCION MULTIPLE;RECORDAR;¿Cuál es la capital de Francia?;París|Londres|Madrid|Roma;París;30
VERDADERO/FALSO;ENTENDER;El sol gira alrededor de la Tierra.;Verdadero|Falso;Falso;15
```

## Compilación y Ejecución

1. Clonar el repositorio desde GitHub.
2. Abrir el proyecto en IntelliJ IDEA o tu entorno Java preferido.
3. Ejecutar `Main.java` desde el entorno.
4. Usar la opción de la interfaz para **cargar el archivo de ítems** y comenzar la prueba.

## Licencia y Uso

Este proyecto fue creado con fines educativos y puede ser utilizado libremente como referencia para trabajos académicos o aprendizaje personal.

## Autores

Proyecto desarrollado por estudiantes de tercer año de Ingeniería en Informática.

**Colaboradores**:
- Lukas Flores (@Raizexs)
- David Vásquez (@vsqzHK)
