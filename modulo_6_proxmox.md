
# Módulo 6: Redes y Firewall

## 1. Configuración de Bridges
Proxmox utiliza bridges para conectar las máquinas virtuales a la red física.
- vmbr0 suele estar conectado al adaptador físico (eth0).
- Puedes crear bridges adicionales para segmentar redes.

![Bridge Configuración](images/bridge_configuracion.png)

---

## 2. Crear un Bridge adicional
- Ve a "Datacenter > Nodo > Red"
- Haz clic en "Crear > Linux Bridge"
- Asigna un nombre (ej. vmbr1) y configura la IP si es necesario

![Crear Bridge](images/crear_bridge.png)

---

## 3. Configuración de VLANs
Las VLANs permiten segmentar el tráfico de red.
- Asegúrate de que tu switch físico soporte VLANs
- Configura la VLAN en la interfaz de red de la VM

![VLAN Configuración](images/vlan_configuracion.png)

---

## 4. Reglas de Firewall por VM
Proxmox permite aplicar reglas de firewall por VM:
- Ve a la VM > Firewall
- Añade reglas de entrada/salida (ej. permitir SSH, bloquear ICMP)

![Firewall VM](images/firewall_vm.png)

---

## 5. Reglas de Firewall por Nodo
También puedes aplicar reglas a nivel de nodo:
- Ve a "Datacenter > Nodo > Firewall"
- Añade reglas globales para todo el nodo

![Firewall Nodo](images/firewall_nodo.png)

---

## 6. Activar el Firewall
- Ve a "Datacenter > Firewall"
- Activa el firewall global
- Asegúrate de que esté activado en cada VM y nodo

![Activar Firewall](images/activar_firewall.png)

---

Este módulo cubre la configuración de red y seguridad mediante firewall en Proxmox VE, fundamentales para entornos multiusuario y educativos.
