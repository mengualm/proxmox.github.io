
# Módulo 7: Alta disponibilidad y clústeres

## 1. ¿Qué es un clúster en Proxmox?
Un clúster permite gestionar múltiples nodos de Proxmox desde una única interfaz, facilitando la migración de VMs y la alta disponibilidad.

![Clúster Proxmox](images/cluster_proxmox.png)

---

## 2. Crear un clúster
- En el nodo principal, ve a "Datacenter > Clúster"
- Haz clic en "Crear clúster"
- Define el nombre y la red de comunicación

```bash
pvecm create nombre-cluster
```

![Crear Clúster](images/crear_cluster.png)

---

## 3. Unir nodos al clúster
- En los nodos secundarios, ve a "Datacenter > Clúster"
- Haz clic en "Unirse al clúster"
- Introduce la IP del nodo principal y la clave

```bash
pvecm add IP-del-nodo-principal
```

![Unir Nodo](images/unir_nodo.png)

---

## 4. Migración en vivo de VMs
Una vez en clúster, puedes mover VMs entre nodos sin apagarlas:
- Selecciona la VM > Migrar
- Elige el nodo destino

![Migración en Vivo](images/migracion_viva.png)

---

## 5. Configurar Alta Disponibilidad (HA)
- Ve a "Datacenter > HA"
- Añade recursos (VMs) al grupo de HA
- Define el comportamiento ante fallos

![Alta Disponibilidad](images/alta_disponibilidad.png)

---

## 6. Monitorización centralizada
- Desde la vista de "Datacenter" puedes ver el estado de todos los nodos
- Utiliza herramientas como syslog, Zabbix o Prometheus para monitoreo avanzado

![Monitorización](images/monitorizacion.png)

---

Este módulo te enseña a configurar un entorno de alta disponibilidad con múltiples nodos en Proxmox VE, ideal para entornos críticos y educativos avanzados.
