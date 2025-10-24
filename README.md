# Proyecto DevOps (Resumen)
#### Elaborado por: Miguel Caro, Diana Bernal, Samuel Parra y Laura Rodriguez 

### Punto 1: Infraestructura Base

##  Arquitectura Implementada

### **Máquina Virtual Central (Administrador)**
- **Sistema Operativo:** Debian
- **Función:** Monitorización central de todas las dependencias

### **Dependencias Implementadas**

#### **Recursos Humanos**
- **Máquina Virtual:** Arch Linux (M_VRH)

#### **Tecnología** 
- **Máquina Virtual:** Rocky Linux (M_VT)

#### **Financiera**
- **Contenedor:** Garuda Linux (C.F)

#### **Comercial y de Ventas**
- **Contenedor:** Fedora (C.C&V)

### Configuración de Red

### Esquema de Subredes
- Cada dependencia cuenta con su propia subred
- Comunicación restringida a dependencias específicas
- Configuración de aislamiento de red por dependencia

##  Procesos de Instalación

### Máquina Virtual Central (Debian)
1. Descarga de ISO Debian stable
2. Configuración de QEMU/KVM
3. Instalación del sistema base
4. Configuración de herramientas de monitoreo

### Dependencia Recursos Humanos (Arch Linux)
1. Obtención de imagen Arch Linux
2. Instalación mediante QEMU
3. Configuración de red específica
4. Instalación de paquetes básicos

### Dependencia Tecnología (Rocky Linux)
1. Descarga de Rocky Linux
2. Configuración de máquina virtual
3. Establecimiento de subred
4. Instalación de herramientas de desarrollo

### Contenedor Financiero (Garuda Linux)
1. Configuración de Docker
2. Pull de imagen Garuda Linux
3. Creación de contenedor con red específica
4. Configuración de servicios financieros

### Contenedor Comercial (Fedora)
1. Obtención de imagen Fedora container
2. Despliegue en Docker
3. Configuración de red aislada
4. Instalación de herramientas comerciales

##  Tecnologías Utilizadas

- **Virtualización:** QEMU/KVM
- **Contenedores:** Docker
- **Sistemas Operativos:** Debian, Arch Linux, Rocky Linux, Garuda Linux, Fedora


#### Punto 2: Expansión de Infraestructura

## Ampliación de Dependencias

### *Dependencia de Recursos Humanos - Expansión*

#### Máquina Virtual Adicional
- *Sistema Operativo:* Manjaro
- *Configuración:* Integración con subred existente
- *Función:* Ampliación de capacidad de procesamiento

#### Contenedor Adicional
- *Sistema Operativo:* Centos (No implementado)
- *Razón:* Limitaciones técnicas en la instalación
- *Alternativa:* Documentación de proceso fallido

### *Dependencia de Tecnología - Expansión*

#### Máquina Virtual: Kali Linux
- *Propósito:* Herramientas de seguridad y pentesting
- *Configuración:* Subred tecnología
- *Características:* Suite completa de herramientas forenses

#### Máquina Virtual: Linux Mint
- *Propósito:* Estación de desarrollo
- *Configuración:* Integración con servicios existentes
- *Características:* Entorno desktop optimizado

### *Dependencia Financiera - Expansión*

#### Contenedor: Ubuntu
- *Propósito:* Servicios financieros adicionales
- *Configuración:* Red financiera
- *Características:* Estabilidad LTS

#### Contenedor: Alpine
- *Propósito:* Servicios ligeros
- *Configuración:* Minimalista para tareas específicas
- *Características:* Seguridad y eficiencia

### *Dependencia Comercial y de Ventas - Expansión*

#### Máquina Virtual: Alma Linux
- *Propósito:* Servicios comerciales empresariales
- *Configuración:* Subred comercial
- *Características:* Compatibilidad con RHEL

#### Contenedor: Debian
- *Propósito:* Aplicaciones de ventas
- *Configuración:* Contenedor estable
- *Características:* Confiabilidad y seguridad

## Limitaciones Encontradas

### Problema con CentOS
- *Issue:* Imposibilidad de instalar CentOS para las subredes
- *Impacto:* No se pudieron establecer interconexiones planeadas
- *Workaround:* Documentación del problema para futuras implementaciones

### Configuración de Red
- *Estado:* Subredes aisladas funcionando correctamente
- *Falta:* Comunicación inter-dependencias no implementada
- *Causa:* Dependencia de CentOS para configuración de gateway

## Procesos Técnicos

### Instalación Kali Linux
1. Descarga de imagen oficial
2. Configuración de máquina virtual
3. Instalación de herramientas de seguridad
4. Integración con monitoreo central

### Configuración Alpine Container
1. Pull de imagen oficial Alpine
2. Configuración de servicios mínimos
3. Optimización de recursos
4. Conexión a red financiera

### Implementación Alma Linux
1. Migración desde CentOS (conceptual)
2. Configuración de servicios empresariales
3. Integración con herramientas comerciales
4. Documentación de compatibilidad


# Punto 3: Análisis y Monitoreo

##  Sistema de Monitoreo Implementado

### **Análisis de Hardware y Dispositivos**

#### Comandos de Diagnóstico de Hardware
- `dmidecode` - Información del sistema y BIOS
- `hwinfo` - Detalles completos de hardware
- `lspci` - Dispositivos PCI conectados
- `lsusb` - Dispositivos USB disponibles
- `dmesg` - Mensajes del kernel y hardware

#### Comandos de Estado del Sistema
- `uname -a` - Información del kernel y sistema
- `free -h` - Uso de memoria RAM
- `df -h` - Espacio en disco
- `lshw` - Listado detallado de hardware
- `inxi` - Resumen completo del sistema

#### Comandos de Monitoreo en Tiempo Real
- `lsblk` - Dispositivos de bloque
- `udevadm` - Administración de dispositivos
- `atop` - Monitorización avanzada
- `iotop` - Uso de I/O en disco
- `iftop` - Tráfico de red

#### Herramientas de Visualización
- `glances` - Monitorización integral
- `bpytop` - Monitor de recursos con UI
- `ss -tulnp` - Conexiones de red
- `nmcli device status` - Estado de dispositivos de red
- `mount` - Sistemas de archivos montados

### **Análisis de Servicios y Procesos**

#### Monitoreo de Procesos
- `top` - Procesos en tiempo real
- `ps aux` - Listado completo de procesos
- `pstree -p` - Árbol de procesos
- `dstat` - Estadísticas del sistema

#### Gestión de Servicios Systemd
- `systemctl list-units --type=service` - Servicios activos
- `systemd-cgtop` - Grupos de control systemd
- `systemd-analyze blame` - Tiempos de arranque
- `journalctl --since "1 hour ago"` - Logs recientes

#### Análisis de Red y Puertos
- `ss -ltnp` - Puertos escuchando
- `lsof -i :80` - Procesos usando puerto 80
- `glances --webserver` - Interface web de monitoreo

### **Gestión de Archivos y Discos**

#### Herramientas Implementadas
- `ncdu` - Análisis de uso de disco
- `baobab` - Visualizador gráfico de disco
- `tree` - Estructura de directorios
- `rsync` - Sincronización de archivos

### **Gestión de Logs**

#### Analizadores de Logs
- `lnav` - Navegador avanzado de logs
- `goaccess` - Analizador de logs web en tiempo real

### **Análisis de Red Avanzado**

#### Netdata
- Implementación completa de Netdata
- Visualización de métricas en tiempo real
- Dashboards para cada dependencia
- Alertas y monitoreo proactivo

#### Wireshark
- Captura e inspección de tráfico de red
- Análisis de paquetes entre contenedores
- Diagnóstico de problemas de conectividad

#### Análisis de Discos
- `smartctl -a /dev/sdX` - Salud de discos duros
- Monitoreo de parámetros SMART
- Detección temprana de fallos

##  Desarrollo Web y Auditoría

### Aplicación Streamlit
- Página web corporativa desplegada
- Monitoreo de consumo de recursos
- Integración con servicios existentes

### Auditoría de Seguridad
- `lynis` - Auditoría interna del sistema
- Análisis de vulnerabilidades
- Recomendaciones de hardening

### Escaneo de Red
- `nmap` - Exploración de puertos
- Análisis de servicios expuestos
- Documentación de superficie de ataque

##  Resultados Obtenidos

### Métricas Capturadas
- Uso de CPU y memoria por dependencia
- Tráfico de red entre contenedores
- Estado de salud de discos duros
- Tiempos de respuesta de servicios

### Hallazgos Importantes
- Optimización de recursos identificada
- Patrones de uso caracterizados
- Puntos de mejora en configuración
- Línea base de performance establecida

##  Configuraciones Específicas

### Para Dependencia de Recursos Humanos
- Enfoque en monitoreo de procesos de usuario
- Análisis de carga laboral del sistema
- Optimización de recursos compartidos

### Para Dependencia Financiera
- Énfasis en seguridad y logs
- Monitoreo de transacciones del sistema
- Auditoría de accesos y permisos


