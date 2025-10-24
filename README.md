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



#### Proyecto de Infraestructura - Punto 2: Expansión de Infraestructura

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

## Estado de Implementación

| Dependencia | Componente | Estado | Observaciones |
|-------------|------------|---------|---------------|
| RRHH | Manjaro VM | ✅ | Operativo |
| RRHH | CentOS Container | ❌ | No implementado |
| Tecnología | Kali Linux VM | ✅ | Operativo |
| Tecnología | Linux Mint VM | ✅ | Operativo |
| Financiera | Ubuntu Container | ✅ | Operativo |
| Financiera | Alpine Container | ✅ | Operativo |
| Comercial | Alma Linux VM | ✅ | Operativo |
| Comercial | Debian Container | ✅ | Operativo |

