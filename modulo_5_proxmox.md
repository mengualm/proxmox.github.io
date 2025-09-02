
# Módulo 5: Snapshots, Backups y Restore

## 1. ¿Qué es un Snapshot?
Un snapshot es una copia del estado actual de una máquina virtual o contenedor en un momento específico. Permite restaurar rápidamente en caso de errores o cambios no deseados.

![Snapshot](images/snapshot.png)

---

## 2. Crear un Snapshot
Para crear un snapshot:
- Selecciona la VM o CT en la interfaz web
- Ve a la pestaña "Snapshots"
- Haz clic en "Crear"

![Crear Snapshot](images/crear_snapshot.png)

---

## 3. Restaurar desde un Snapshot
- Ve a la pestaña "Snapshots"
- Selecciona el snapshot deseado
- Haz clic en "Restaurar"

![Restaurar Snapshot](images/restaurar_snapshot.png)

---

## 4. ¿Qué es un Backup?
Un backup es una copia completa de una VM o CT que puede almacenarse en un almacenamiento local o remoto. Es útil para recuperación ante desastres.

![Backup](images/backup.png)

---

## 5. Crear un Backup manual
- Ve a la pestaña "Backup"
- Haz clic en "Iniciar"
- Selecciona el modo (snapshot, suspendido, detenido)

![Crear Backup](images/crear_backup.png)

---

## 6. Programar Backups automáticos
- Ve a "Datacenter > Backup"
- Configura tareas de backup con cron
- Selecciona nodos, VMs/CTs y almacenamiento

![Backup Automático](images/backup_automatico.png)

---

## 7. Restaurar desde un Backup
- Ve a "Datacenter > Backup"
- Selecciona el archivo de backup
- Haz clic en "Restaurar"

![Restaurar Backup](images/restaurar_backup.png)

---

Este módulo cubre las funciones esenciales de protección de datos en Proxmox VE mediante snapshots y backups, fundamentales para mantener la integridad de los entornos virtualizados.
