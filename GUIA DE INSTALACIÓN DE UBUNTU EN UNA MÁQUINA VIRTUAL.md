# GUIA DE INSTALACIÓN DE UBUNTU EN UNA MÁQUINA VIRTUAL
Esta guía explica cómo instalar Ubuntu Desktop en una máquina virtual utilizando VirtualBox. El objetivo es aprender a instalar y utilizar un sistema operativo Linux sin tener que sustituir el sistema operativo principal del ordenador.
- [GUIA DE INSTALACIÓN DE UBUNTU EN UNA MÁQUINA VIRTUAL](#guia-de-instalación-de-ubuntu-en-una-máquina-virtual)
  - [📖1. Introducción](#1-introducción)
  - [🖥️2. Requisitos previos](#️2-requisitos-previos)
  - [⚙️3. Instalación paso a paso](#️3-instalación-paso-a-paso)
    - [📥3.1 Descargar los programas necesarios](#31-descargar-los-programas-necesarios)
    - [🖥️3.2 Crear la máquina virtual](#️32-crear-la-máquina-virtual)
    - [🌐3.3 Configurar el adaptador de red virtual](#33-configurar-el-adaptador-de-red-virtual)
    - [💿3.4 Instalar Ubuntu](#34-instalar-ubuntu)
  - [✅4. Comprobación de la instalación](#4-comprobación-de-la-instalación)
  - [💻 5. Introducción a los comandos básicos de Linux](#5-introducción-a-los-comandos-básicos-de-linux)
  - [🛠️6. Resolución de problemas](#️6-resolución-de-problemas)
  - [🔗7. Referencias](#7-referencias)
## 📖1. Introducción
Ubuntu es un sistema operativo basado en Linux, de código abierto y utilizado tanto en ordenadores personales como en servidores.
Una máquina virtual es un ordenador simulado mediante un programa. Permite ejecutar otro sistema operativo dentro del ordenador habitual, utilizando parte de sus recursos, como la memoria RAM, el procesador y el almacenamiento.
En esta guía utilizaremos **VirtualBox** para crear una máquina virtual e instalar Ubuntu Desktop.
Una de las principales ventajas de este procedimiento es que permite practicar con Linux sin modificar directamente el sistema operativo principal.
## 🖥️2. Requisitos previos
Antes de comenzar la instalación, es necesario disponer de los siguientes elementos:
* Un ordenador con conexión a internet.
* VirtualBox instalado.
* Una imagen ISO de Ubuntu Desktop.
* Espacio libre en el disco duro.
* Memoria RAM suficiente para ejecurar el sistema principal y la máquina virtual.

La siguiente tabla muestra una configuración orientativa para realizar la práctica.

| Recurso | Configuración recomendada para la práctica | Función |
| - | - | - |
| Memoria RAM | 4GB para Ubuntu, si el equipo lo permite | Permite ejecutar el sistema virtual |
| Disco virtual | 25 GB como mínimo | Almacena Ubuntu y sus archivos |
| Procesador | 4 CPU virtuales, si están disponibles | Permite ejecutar los programas |
| Imagen ISO | Ubuntu Desktop de 64 bits compatible | Contiene los archivos de instalación |

>**Importante**: *Los recursos asignados a la máquina virtual se comparten con el ordenador principal. No asignes toda la memoria RAM ni todos los procesadores disponibles, porque el sistema principal también los necesita.*
>
## ⚙️3. Instalación paso a paso
### 📥3.1 Descargar los programas necesarios
El primer paso consiste en descargar VirtualBox y la imagen ISO de Ubuntu.

1. Accede al apartado de descargas de la página oficial de [VirtualBox](https://www.virtualbox.org/wiki/Downloads).
![3.1.1](imagenes\3.1.1.jpg)
2. Descarga la versión correspondiente al sistema operativo de tu ordenador.
![3.1.2](imagenes\3.1.2.jpg)
3. Ejecuta el instalador de VirtualBox y sigue las instrucciones que aparecen en pantalla.
![3.1.3](imagenes\3.1.3.jpg)
4. Accede a la pagina oficial de [Ubuntu Desktop](https://ubuntu.com/download/desktop).
![3.1.4](imagenes\3.1.4.jpg)
5. Descarga la imagen ISO de Ubuntu y guarda el archivo en una carpeta fácil de localizar.
![3.1.5](imagenes\3.1.5.jpg)

La imagen ISO es un archivo que contiene los datos necesarios para instalar un sistema operativo. VirtualBox permite utilizarla como si fuera un DVD de instalación virtual.

---

### 🖥️3.2 Crear la máquina virtual
Una vez instalado VirtualBox y descargada la imagen ISO, hay que crear la máquina virtual.
1. Abre VirtualBox y pulsa el botón **Nueva**.

![3.2.1](imagenes\3.2.1.jpg)

2. Introduce un nombre para la máquina, por ejemplo, Ubuntu.
3. Selecciona la imagen ISO descargada de Ubuntu.
4. Pulsa **Siguiente** para avanzar.

![3.2.2](imagenes\3.2.2.jpg)

5. Asigna memoria RAM y procesadores y disco duro virtual según las caracteristicas de tu ordenador y pulsa **Siguiente**.

![3.2.5](imagenes\3.2.5.jpg)

6. Revisa la configuración y pulsa **Terminar** para finalizar la creación de la máquina virtual.

![3.2.6](imagenes\3.2.6.jpg)

El disco duro virtual es un archivo almacenado en el ordenador real que funciona como el disco de la máquina virtual.
VirtualBox ofrece una instalación desatendida, puedes utilizarla o desactivarla para seguir manualmente los pasos del instalador de Ubuntu.

---

### 🌐3.3 Configurar el adaptador de red virtual
El adaptador de red virtual permite que Ubuntu se conecte a una red y pueda acceder a Internet. VirtualBox ofrece diferentes modos de conexión; en este caso utilizaremos **NAT**, que permite a la máquina virtual utilizar la conexión a Internet del ordenador principal sin necesidad de configurar una red independiente.
Para configurar el adaptador de red, sigue estos pasos:
1. Abre VirtualBox y selecciona la máquina virtual de Ubuntu.
2. Comprueba que la máquina virtual esté apagada.
3. Pulsa el botón **Configuración**.

![3.3.1](imagenes\3.3.1.jpg)

4. En el menú lateral, selecciona **Red**.
5. En la pestaña **Adaptador 1**, marca la casilla *Habilitar adaptador de red*.
6. En el apartado **Conectado a**, selecciona la opción **NAT**.
7. Pulsa **Aceptar** para guardar los cambios.

![3.3.4](imagenes\3.3.4.jpg)

La configuración NAT suele ser suficiente para navegar por Internet, descargar actualizaciones e instalar programas desde Ubuntu.

---

###  💿3.4 Instalar Ubuntu
Después de crear la máquina virtual, ya se puede iniciar la instalación del sistema operativo.
1. Selecciona la máquina virtual creada y pulsa **iniciar**.

![3.4.1](imagenes\3.4.1.jpg)

2. Espera a que aparezca el menú de instalación de Ubuntu.
3. Selecciona la opción para instalar Ubuntu.

![3.4.3](imagenes\3.4.3.png)

4. Escoge el idioma y la distribución del teclado.

![3.4.4](imagenes\3.4.4.png)

5. Configura las opciones de instalación que necesites.

![3.4.5.1](imagenes\3.4.5.1.jpg)
![3.4.5.2](imagenes\3.4.5.2.jpg)

6. Introduce el nombre del usuario, el nombre del equipo y una contraseña.

![3.4.6](imagenes\3.4.6.png)

7. Revisa las opciones seleccionadas e inicia la instalación.

![3.4.7](imagenes\3.4.7.png)

8. Espera a que finalice el proceso y reinicia la máquina virtual cuando se solicite.

![3.4.8](imagenes\3.4.8.png)

Durante la instalación, Ubuntu copiará los archivos necesarios al disco virtual y configurará el sistema operativo

## ✅4. Comprobación de la instalación
Cuando termine la instalación, inicia Ubuntu e introduce la contraseña del usuario creado.
Si todo ha funcionado correctamente, aparecerá el escritorio de Ubuntu y podrás utilizar sus aplicaciones.
Para comprobar que el sistema funciona, realiza las siguientes acciones:
1. Abre el menú de aplicaciones y comprueba que puedes iniciar un programa.
2. Comprueba que la conexión a Internet funciona, si has configurado la red virtual.
3. Abre la terminal de Ubuntu.
4. Ejecuta el siguiente comando para consultar la version del sistema: `lsb_release -a`. Este comando muestra información sobre la distribución de Linux instalada.
También puedes utilizar el comando `uname -r` para consultar la versión del núcleo de Linux.
Después de verificar que Ubuntu funciona, es recomendable comprobar si hay actualizaciones disponibles:

```bash
sudo apt update
sudo apt upgrade
```
El primer comando actualiza la información de los paquetes disponibles y el segundo instala las actualizaciones correspondientes. Puede solicitar la contraseña del usuario (no aparece mientras la escribes).
## 💻 5. Introducción a los comandos básicos de Linux
Una vez instalado Ubuntu, es recomendable familiarizarse con la terminal, una herramienta que permite interactuar con el sistema operativo mediante comandos de texto.
Para abrirla, pulsa las teclas **Ctrl + Alt + T**. A continuación, puedes probar algunos de los comandos básicos de Linux:
| Comando | Función |
|---|---|
| `pwd` | Muestra la ruta del directorio actual. |
| `ls` | Muestra los archivos y carpetas del directorio. |
| `cd` | Permite cambiar de directorio. |
| `mkdir` | Crea una nueva carpeta. |
| `clear` | Limpia el contenido visible de la terminal. |
| `whoami` | Muestra el nombre del usuario actual. |
Por ejemplo, para crear una carpeta llamada `Practica` y acceder a ella, ejecuta los siguientes comandos:
```bash
mkdir Practica
cd Practica
```
También es importante conocer el comando `sudo`, que permite ejecutar determinadas operaciones con permisos de administrador. Por ejemplo:
```bash
sudo apt update
```
Este comando actualiza la información de los paquetes disponibles en los repositorios de Ubuntu.
Estos comandos constituyen una primera aproximación al uso de la terminal y permiten realizar algunas tareas básicas de administración y navegación en Linux.
##  🛠️6. Resolución de problemas
Durante la instalación pueden aparecer algunos problemas. La siguiente tabla recoge situaciones habituales y sus posibles soluciones.
| Problema | Posible Causa | Solución |
|-|-|-|
| La máquina virtual no inicia | Configuración incorrecta o virtualización no disponible | Revisar la configuración y comprobar si el equipo admite la virtualización |
| No aparece el instalador de Ubuntu | La imagen ISO no está seleccionada correctamente | Revisar la configuración de almacenamiento o el medio de instalación |
| Ubuntu funciona lento | Recursos insuficientes | Ajustar la memoria RAM y los procesadores virtuales |
| No hay conexion a internet | Configuración de red incorrecta | Comprobar que el adaptador de red virtual está habilitado |
| No se puede iniciar sesión | Contraseña incorrecta | Comprobar usuario y contraseña introducidos |

Si el problema continua, consulta la documentación oficial de Ubuntu o VirtualBox para encontrar una solución especifica.
## 🔗7. Referencias
* [Página oficial de Ubuntu Desktop](https://ubuntu.com/desktop)
* [Tutorial oficial para ejecutar Ubuntu en VirtualBox](https://ubuntu.com/tutorials/how-to-run-ubuntu-desktop-on-a-virtual-machine-using-virtualbox)
* [Página oficial para descargar VirtualBox](https://www.virtualbox.org/wiki/Downloads)
* [Documentación oficial de Ubuntu](https://documentation.ubuntu.com/desktop/)
