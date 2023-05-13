# ¿Qué es Docker?

- **Docker** es una plataforma que facilita el desarrollo, despliegue y ejecución de aplicaciones.
- Permite **separar las aplicaciones de la infraestructura**, incrementando la eficiencia y comodidad en el trabajo.
- Docker permite **empaquetar y ejecutar aplicaciones en un entorno aislado**, llamado contenedor.
- Los contenedores se ejecutan **directamente sobre el kernel de la máquina**, lo que los hace más ligeros que las máquinas virtuales.
- Esto permite **ejecutar un mayor número de contenedores en el mismo equipo**.
- Facilita la **realización de pruebas rápidas** de la aplicación en múltiples entornos.
- Comparado con las máquinas virtuales, Docker **reduce el tiempo de carga y el espacio requerido**.
- El resultado es un **desarrollo más rápido y cómodo**.

# Contenedores I

- Los **contenedores** se diferencian de las máquinas virtuales en que no emulan un ordenador físico ni instalan un sistema operativo completo.
- En cambio, los contenedores utilizan el **kernel del sistema operativo anfitrión** pero contienen las capas superiores (sistema de ficheros, utilidades, aplicaciones).
- Al evitar la emulación del hardware y el sistema operativo completo, los contenedores son **más pequeños y rápidos** que las máquinas virtuales.
- A pesar de ello, al incluir el resto de capas de software, los contenedores logran el **aislamiento e independencia** entre ellos, una característica deseable que se busca con las máquinas virtuales.

# Contenedores II

- **Docker** no es una plataforma de virtualización, por lo que no incluye un hipervisor. Los procesos dentro de un contenedor Docker se ejecutan en el mismo kernel que la máquina anfitrión.
- Docker es capaz de aislar los procesos del contenedor del resto del sistema, ya sean procesos de la máquina anfitrión o de otros contenedores.
- Permite **controlar los recursos** asignados a los contenedores, como la CPU y la memoria.
- Internamente, un contenedor no tiene consciencia de que lo es, y funciona como una distribución **GNU/Linux independiente**, sin la penalización de rendimiento de los sistemas virtualizados.
- Al ejecutar un contenedor, estás ejecutando un servicio en una distribución construida a partir de una "receta", lo que garantiza la consistencia del sistema, independientemente del sistema operativo base (Ubuntu, Fedora, etc.).
- Esto asegura el desarrollo o despliegue de una aplicación con la **misma versión de todas las dependencias**, sin importar el entorno.

# Imágenes II

- Una **Imagen** es una plantilla de solo lectura que contiene las instrucciones para crear un contenedor Docker.
- Las imágenes pueden estar **basadas en otras imágenes**, usando ficheros como el Dockfile para definirlas.
- Un ejemplo de imagen podría ser un sistema operativo **Ubuntu con un servidor Apache** y tu aplicación web instalada.






