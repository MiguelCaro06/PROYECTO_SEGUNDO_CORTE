# Proyecto de Infraestructura - Punto 1: Infraestructura Base

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

##  Documentación

- Proceso completo documentado en el PDF.
- Capturas de pantalla de cada paso de instalación
- Configuraciones de red detalladas
- Troubleshooting de problemas encontrados

---

**Estado:** ✅ Completado
