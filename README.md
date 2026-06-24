<h1 align = "center" >Administración de Red y Copias de Seguridad en Linux</h1> 


## Objetivos

- Gestionar estructuras de directorios en Linux.
- Automatizar tareas mediante scripts Bash.
- Obtener información de red del sistema.
- Configurar resolución local de nombres.
- Crear copias de seguridad utilizando `tar`.
- Sincronizar directorios mediante `rsync`.
- Restaurar archivos desde copias de seguridad.

trabajo_hugo_arcones/
├── originales/
├── copias/
├── restauracion/
├── logs/
├── scripts/
└── informes/


## Funcionalidades

### 1. Preparación del entorno

- Creación de directorios de trabajo.
- Generación de archivos de prueba.
- Automatización mediante scripts.

### 2. Inventario y diagnóstico de red

Obtención de:

- Interfaces de red.
- Interfaz activa.
- Dirección IP.
- Dirección loopback.
- Puerta de enlace.
- Servidores DNS.

### 3. Resolución local de nombres

Configuración y pruebas del archivo:

```bash
/etc/hosts

Verificación de resolución local utilizando:

getent hosts
ping
4. Copias de seguridad

Creación de backups con:

tar -cvf copia.tar originales/

Consulta del contenido:

tar -tvf copia.tar
5. Sincronización con rsync

Simulación:

rsync -av --dry-run origen/ destino/

Sincronización real:

rsync -av origen/ destino/

Sincronización eliminando archivos obsoletos:

rsync -av --delete origen/ destino/
6. Restauración

Recuperación selectiva de archivos desde copias realizadas con tar.

Tecnologías utilizadas
Linux
Bash
tar
rsync
Networking Tools
Aprendizajes obtenidos

Durante este proyecto se trabajó con conceptos fundamentales de administración de sistemas Linux:

Automatización mediante scripts.
Gestión de archivos y directorios.
Diagnóstico de red.
Resolución de nombres.
Estrategias de backup y recuperación.
Sincronización segura de datos.
<br><br>
Autor

Hugo Arcones 

Estudiante de Sistemas Microinformáticos y Redes (SMR).
