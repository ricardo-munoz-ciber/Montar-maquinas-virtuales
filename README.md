Homelab Base: Despliegue de Infraestructura Virtual

Objetivo del Proyecto:
Establecer la infraestructura de virtualización base (Homelab) mediante el montaje y configuración de múltiples máquinas virtuales. Este entorno inicial y seguro sirven  para prácticas de administración de sistemas, redes, y futuras simulaciones de ciberseguridad (Blue Team / Red Team).

Hipervisor Utilizado
VMware (Workstation / ESXi)

Sistemas Operativos Desplegados

Entornos Windows
Windows 10 & Windows 11: Configurados como estaciones de trabajo cliente (Endpoints). Ideales para pruebas de despliegue de políticas, integración en dominios y simulación de usuarios finales.
Windows Server 2022 & Windows Server 2025: Servidores base preparados para asumir roles de infraestructura crítica, como Controladores de Dominio (Active Directory), DNS y DHCP.

Entornos Linux
Linux Mint: Entorno principal para tareas de administración, gestión del hipervisor y levantamiento de servicios estables.
Kali Linux: Máquina virtual aislada y dedicada a herramientas de seguridad ofensiva, escaneo de vulnerabilidades y auditorías de red.
Ubuntu: Servidor de propósito general, ideal para alojar servicios en red, contenedores o herramientas de monitorización.

Configuraciones Clave Implementadas
Gestión de Red Virtual: Configuración estratégica de adaptadores (NAT, Host-Only, Bridged) para crear segmentos de red aislados, protegiendo la red doméstica durante las simulaciones.
Optimización de Recursos: Asignación medida de memoria RAM y CPU dependiendo del rol y peso de cada sistema operativo para mantener un rendimiento fluido del hipervisor.
Snapshots (Instantáneas):Creación de puntos de restauración base ("Golden Images") tras las instalaciones limpias y actualizaciones. Esto permite revertir las máquinas a un estado seguro en segundos tras pruebas de seguridad o configuraciones fallidas.
VMware Tools: Instalación y configuración en todos los sistemas invitados para garantizar la correcta integración de red, video y rendimiento con el sistema anfitrión.

Topología / Vista del Entorno





<img width="270" height="189" alt="image" src="https://github.com/user-attachments/assets/54e0993b-74b5-4651-943d-8d0c0666ae76" />


