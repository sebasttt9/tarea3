"# tarea3" 
Práctica No. 3: Persistencia de Datos en Contenedores Docker con PostgreSQL
1. Título

Persistencia de Datos en Contenedores PostgreSQL con y sin Volúmenes en Docker

2. Tiempo de duración

50 minutos

3. Fundamentos

Docker es una herramienta que permite crear contenedores ligeros y portátiles para ejecutar aplicaciones de manera aislada del sistema operativo anfitrión. Estos contenedores se construyen a partir de imágenes que incluyen el entorno necesario para que la aplicación funcione correctamente.

Cuando se ejecuta una base de datos como PostgreSQL dentro de un contenedor, los datos generados se almacenan por defecto dentro del sistema de archivos del contenedor. Esto significa que si el contenedor se elimina, toda la información almacenada desaparece. Este comportamiento puede ser útil para entornos de desarrollo o pruebas, pero no es adecuado para entornos de producción donde la persistencia de datos es fundamental.

Para resolver este problema, Docker ofrece una característica llamada volúmenes, que permite guardar los datos en una ubicación fuera del ciclo de vida del contenedor. De esta manera, aunque el contenedor se detenga o elimine, los datos permanecen en el volumen y pueden ser reutilizados por otros contenedores.

En esta práctica se observará claramente la diferencia entre un contenedor PostgreSQL sin volumen (donde los datos se pierden al eliminarlo) y otro con volumen (donde los datos persisten).

Conceptos Clave:

Contenedor: Entorno aislado donde se ejecuta una aplicación.

Imagen: Plantilla inmutable utilizada para crear contenedores.

Volumen: Espacio de almacenamiento persistente que Docker administra.

PostgreSQL: Sistema de gestión de bases de datos relacional (RDBMS) de código abierto.

Docker CLI: Interfaz de línea de comandos para interactuar con Docker.

4. Conocimientos previos

Para realizar esta práctica, el estudiante debe tener conocimientos básicos sobre:

Uso de comandos en Linux (cd, ls, docker run, docker ps, docker rm, etc.)

Manejo de Docker: creación, ejecución y eliminación de contenedores.

Conceptos básicos de bases de datos relacionales (SQL, tablas, registros).

Conexión a bases de datos mediante herramientas como DataGrip, TablePlus o pgAdmin.

Manejo de un navegador web para acceder a documentación o Docker Hub.

5. Objetivos a alcanzar

Implementar contenedores Docker que ejecuten PostgreSQL.

Comprobar la pérdida de datos sin volumen y la persistencia de datos con volumen.

Asociar volúmenes a contenedores para preservar la información almacenada.

Fortalecer el manejo de comandos Docker en entornos reales de desarrollo.

6. Equipo necesario

Computadora con sistema operativo Windows 10/11, Linux o macOS.

Docker Desktop instalado (versión 25.0 o superior).

Conexión a Internet.

Herramienta de administración de bases de datos (DataGrip, DBeaver, TablePlus o pgAdmin).

Editor de texto o terminal (Visual Studio Code, PowerShell o bash).

Cuenta opcional en Docker Hub
.

7. Material de apoyo

Documentación oficial de Docker: https://docs.docker.com

Documentación de PostgreSQL: https://www.postgresql.org/docs/

Guía de la asignatura.

Linux Cheat Sheet.

Apuntes del estudiante.

9. Resultados esperados

Al finalizar la práctica, se espera que el estudiante haya:

Comprendido la diferencia entre un contenedor con y sin volumen.

Comprobado que, al eliminar un contenedor sin volumen, los datos se pierden.

Verificado que, al usar un volumen, los datos se mantienen intactos incluso después de eliminar y recrear el contenedor.

Aplicado correctamente los comandos de Docker para administrar contenedores y volúmenes.

10. Bibliografía

Docker Inc. (2024). Docker Documentation. Recuperado de https://docs.docker.com

PostgreSQL Global Development Group. (2024). PostgreSQL Documentation. Recuperado de https://www.postgresql.org/docs/

Pahl, C., & Lee, B. (2019). Containerization and the PaaS Cloud. IEEE Software, 32(3), 24–31.

Turnbull, J. (2022). The Docker Book: Containerization is the New Virtualization.
