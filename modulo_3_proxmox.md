
# Módulo 3: Gestión de Máquinas Virtuales

## 1. Creación de una máquina virtual
Para crear una nueva VM en Proxmox:
- Accede a la interfaz web
- Haz clic en "Crear VM"
- Asigna un nombre y selecciona el nodo

![Crear VM](images/crear_vm.png)

---

## 2. Configuración de la VM
Configura los siguientes parámetros:
- Sistema operativo (tipo y versión)
- ISO de instalación
- CPU, RAM y disco
- Red (bridge predeterminado: vmbr0)

![Configuración VM](images/configuracion_vm.png)

---

## 3. Instalación del sistema operativo
Una vez creada la VM:
- Inicia la máquina
- Abre la consola desde la interfaz web
- Sigue el proceso de instalación del sistema operativo (Linux, Windows, etc.)

![Instalación SO](images/instalacion_so.png)

---

## 4. Acceso a la VM
Puedes acceder a la VM de varias formas:
- Consola web integrada
- SSH (si el sistema operativo lo permite)
- Escritorio remoto (RDP para Windows)

![Acceso VM](images/acceso_vm.png)

---

## 5. Gestión y mantenimiento
- Apagar, reiniciar o suspender la VM
- Crear snapshots
- Realizar backups
- Monitorizar uso de recursos

![Gestión VM](images/gestion_vm.png)

---

Este módulo te enseña a crear, configurar y gestionar máquinas virtuales en Proxmox VE, una habilidad esencial para entornos educativos y profesionales.
