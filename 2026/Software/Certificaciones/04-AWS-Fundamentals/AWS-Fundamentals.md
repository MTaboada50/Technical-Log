# ☁️ AWS Cloud Foundations: Documentación Técnica

Este repositorio contiene el desglose técnico y los conceptos fundamentales adquiridos durante el trayecto de formación de **CapacitAR y AWS**. La documentación sigue los estándares de arquitectura de sistemas y gestión de recursos en la nube. La informacion que contiene, fue extraida directamente de las notas que tome durante el curso y formateada lo mejor posible para futura referencia personal o de alguien que quiera realizar la certificacion.

> 📂 **Recursos adjuntos:** [Ver Certificado de Finalización (PDF)](./Certificado-Fundamentals.pdf)

---

## 🏗️ 1. Fundamentos de la Computación en la Nube
Acceso bajo demanda a servicios de TI (cómputo, almacenamiento, bases de datos) a través de Internet con un modelo de **pago por uso**.

### Beneficios Clave
* **Agilidad:** Reducción del tiempo de despliegue de infraestructura de semanas a minutos.
* **Ahorro de Costos:** Transición de CapEx (Inversión fija en hardware) a OpEx (Gasto operativo variable).
* **Escalabilidad:** Los recursos se ajustan automáticamente según la demanda, optimizando el rendimiento y el gasto.
* **Enfoque en el Negocio:** Delegación del mantenimiento de infraestructura física a AWS.

---

## 🌍 2. Infraestructura Global y Confiabilidad
Diseño orientado a la **Alta Disponibilidad** y la tolerancia a fallos mediante la distribución física.

* **Regiones:** Áreas geográficas que contienen múltiples centros de datos.
* **Zonas de Disponibilidad (AZ):** Grupos de uno o más centros de datos con energía, red y conectividad redundantes dentro de una Región.
* **Interacción con Servicios:**
    1. **Consola de Administración:** Interfaz web gráfica.
    2. **AWS CLI:** Interfaz de línea de comandos para automatización.
    3. **AWS SDK:** Kits de desarrollo para integración a nivel de código.

---

## 💻 3. Servicios de Computación (Compute)

### Amazon EC2 (Elastic Compute Cloud)
Capacidad de cómputo segura y redimensionable (IaaS). 
* **Familias de Instancias:** Uso General, Optimizadas para Cómputo, Memoria, Almacenamiento o Computación Acelerada.

### AWS Lambda (Serverless)
Ejecución de código basada en eventos sin gestión de servidores. El cobro se realiza estrictamente por el tiempo de ejecución.

---

## 💾 4. Almacenamiento y Bases de Datos

### Tipos de Almacenamiento
* **Amazon EBS (Bloque):** Almacenamiento de alto rendimiento para instancias EC2 (volúmenes de disco).
* **Amazon S3 (Objetos):** Almacenamiento escalable mediante Buckets. Clases: *Standard, Intelligent-Tiering, One Zone-IA* y *Glacier*.
* **Amazon EFS (Archivos):** Sistema de archivos compartido para múltiples instancias.

### Bases de Datos
* **Relacionales (RDS / Aurora):** Motores administrados (MySQL, PostgreSQL, etc.).
* **No Relacionales (DynamoDB):** Base de datos de clave-valor con latencia de milisegundos a cualquier escala.

---

## 🛡️ 5. Seguridad y Redes

### Amazon VPC (Virtual Private Cloud)
Red virtual aislada lógicamente. Permite definir subredes públicas (acceso a Internet) y privadas.

### Modelo de Responsabilidad Compartida
* **AWS:** Responsable de la seguridad **DE** la nube (Infraestructura física y global).
* **Cliente:** Responsable de la seguridad **EN** la nube (Datos, configuración de parches, IAM y cifrado).

### IAM (Identity and Access Management)
Gestión de identidades bajo el **Principio de Mínimo Privilegio** (Usuarios, Grupos y Roles).

---

## 📈 6. Monitoreo y Escalabilidad
* **Amazon CloudWatch:** Métricas y alarmas en tiempo real para recursos y aplicaciones.
* **AWS CloudTrail:** Registro histórico de llamadas a la API para auditoría y gobernanza.
* **EC2 Auto Scaling:** Ajuste dinámico de la capacidad de cómputo según métricas establecidas.
* **Elastic Load Balancing (ELB):** Distribución automática del tráfico entrante entre múltiples destinos (instancias EC2).

---

## 🔐 7. Protección de Infraestructura (DDoS)
* **Ataque DDoS:** Intento malintencionado de saturar un servicio mediante tráfico coordinado desde múltiples fuentes.
* **AWS Shield:** Servicio de protección gestionado contra ataques de denegación de servicio distribuido.

---

## 🔍 Continuidad de Formación
Los conceptos presentados en este documento se profundizan con un enfoque orientado a la certificación oficial en el archivo:
* **[AWS Certified Cloud Practitioner](../05-AWS-Cloud-Practitioner/AWS-Cloud-Practitioner.md)** (WIP).