
# Módulo 4: Gestión de Contenedores LXC

## 1. ¿Qué es LXC?
LXC (Linux Containers) es una tecnología de virtualización ligera que permite ejecutar múltiples sistemas Linux aislados en un solo host.

![LXC Introducción](images/lxc_intro.png)

---

## 2. Crear un contenedor LXC
Para crear un contenedor:
- Accede a la interfaz web de Proxmox
- Haz clic en "Crear CT"
- Asigna un nombre y selecciona la plantilla

![Crear CT](images/crear_ct.png)

---

## 3. Configuración del contenedor
Configura los siguientes parámetros:
- Plantilla del sistema operativo (descargada previamente)
- CPU, RAM y disco
- Red (bridge: vmbr0)

![Configuración CT](images/configuracion_ct.png)

---

## 4. Instalación de servicios ligeros
Dentro del contenedor puedes instalar servicios como:
```bash
apt update && apt install apache2 mariadb-server
```

![Instalación Servicios](images/instalacion_servicios.png)

---

## 5. Acceso al contenedor
Puedes acceder al contenedor mediante:
- Consola web
- SSH (si está habilitado)

![Acceso CT](images/acceso_ct.png)

---

## 6. Gestión de contenedores
- Iniciar, detener o reiniciar
- Crear snapshots
- Realizar backups
- Monitorizar recursos

![Gestión CT](images/gestion_ct.png)

---

Este módulo te enseña a trabajar con contenedores LXC en Proxmox VE, ideales para servicios ligeros y entornos de laboratorio.
