
# Módulo 8: Integración con servicios externos

## 1. Acceso a Proxmox vía VPN
Para acceder de forma segura a Proxmox desde redes externas:
- Configura un servidor VPN (ej. OpenVPN, WireGuard)
- Asegúrate de que el puerto 8006 esté accesible solo por VPN

![VPN Acceso](images/vpn_acceso.png)

---

## 2. Integración con almacenamiento remoto
Proxmox permite montar almacenamiento externo para backups y discos virtuales.

### a. NFS
- Ve a "Datacenter > Almacenamiento > Añadir > NFS"
- Introduce la IP del servidor y la ruta exportada

```bash
mount -t nfs 192.168.1.100:/nfs/proxmox /mnt/nfs
```

![NFS Configuración](images/nfs_configuracion.png)

### b. CIFS/SMB
- Ve a "Datacenter > Almacenamiento > Añadir > CIFS"
- Introduce la IP, ruta compartida y credenciales

```bash
mount -t cifs //192.168.1.101/proxmox /mnt/cifs -o username=usuario,password=clave
```

![CIFS Configuración](images/cifs_configuracion.png)

---

## 3. Autenticación LDAP/Active Directory
Puedes integrar Proxmox con servicios de autenticación externos:
- Ve a "Datacenter > Permisos > Realms > Añadir > LDAP o AD"
- Introduce la IP del servidor, DN base y credenciales

![LDAP Configuración](images/ldap_configuracion.png)

---

## 4. Notificaciones por correo
Configura notificaciones de eventos importantes:
- Ve a "Datacenter > Correo"
- Introduce servidor SMTP, remitente y destinatario

![Correo Configuración](images/correo_configuracion.png)

---

Este módulo te enseña a integrar Proxmox VE con servicios externos para mejorar la seguridad, almacenamiento y autenticación en entornos educativos y empresariales.
