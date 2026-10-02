# Examen Práctico - Módulo 1 (AWS)
**Estudiante:** Abel Camilo Ortiz Moreno

Este repositorio documenta el desarrollo y la implementación del examen práctico de infraestructura en la nube utilizando los servicios principales de **Amazon Web Services (AWS)**.

---

## 🛠️ Pasos de Implementación y Configuración

### 1. Creación de Par de Claves (Key Pair)
* Se generó un par de claves personalizado para permitir el acceso seguro por SSH a las instancias de infraestructura.
* **Nombre de clave:** `K2K-AbelCamiloOrtizMoreno`.

### 2. Creación y Configuración de Instancia EC2
* Se desplegó una máquina virtual en Amazon EC2 utilizando una imagen base de sistema operativo (AMI).
* **Configuraciones aplicadas:**
  * Nombre de etiqueta asignado para su identificación.
  * Configuración de redes, almacenamiento y grupos de seguridad (Security Groups) para habilitar la conectividad.

### 3. Conexión a la Instancia vía SSH
* Se validó el funcionamiento del servidor conectándose de manera remota mediante la terminal utilizando la clave privada correspondiente:
  ```bash
  ssh -i "K2K-AbelCamiloOrtizMoreno.pem" ec2-user@<tu-ip-publica>
