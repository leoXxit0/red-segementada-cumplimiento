# 👩‍⚖️ ELEONOR ARIAS
### *Abogada · Ciberseguridad · Cumplimiento Normativo*

---

## Sobre Mí

Soy abogada con una visión estratégica en **PYME, gestión de proyectos y relaciones públicas**. Mi trayectoria profesional se centra en la consultoría legal, negocios y el cumplimiento normativo de personas jurídicas.

Lo que me diferencia es mi capacidad para tender puentes entre el **Derecho** y la **Tecnología**. He complementado mi formación legal con estudios técnicos en **redes IP y ciberseguridad**, lo que me permite comprender los riesgos tecnológicos y traducirlos al lenguaje legal que las empresas necesitan para protegerse.

---

## Proyecto ª1: Segmentación de Red para Cumplimiento Normativo

> **Objetivo:** Diseñar e implementar una arquitectura de red corporativa segura, aplicando el principio de **"Mínimo Privilegio"** y **"Privacidad por Diseño"**, alineada con los estándares internacionales de ciberseguridad y protección de datos.

### 🔍 ¿Qué hice?

Utilizando **Cisco Packet Tracer**, diseñé y configuré una red local (LAN) para una oficina con 3 departamentos. Para garantizar la **confidencialidad** de los datos, segmenté el tráfico mediante **VLANs** (redes virtuales) y configuré un **firewall perimetral (ACLs)** que controla quién puede comunicarse con quién dentro de la organización.

**Arquitectura de la Red:**

| Departamento | VLAN | Red IP | Clasificación de Datos |
| :--- | :--- | :--- | :--- |
| **Administración** | VLAN 10 | 192.168.10.0/24 | Alta Confidencialidad (Estrategia, Finanzas) |
| **Ventas** | VLAN 20 | 192.168.20.0/24 | Confidencial (Base de datos de clientes) |
| **Servidores Web** | VLAN 30 | 192.168.30.0/24 | Pública/Interna (Solo servicios web) |
| **Recursos Humanos** | VLAN 40 | 192.168.40.0/24 | Muy Alta Confidencialidad (Nóminas, datos personales) |

**Políticas de Seguridad Aplicadas (Firewall ACL 110):**

| Origen | Destino | Acción | Justificación |
| :--- | :--- | :--- | :--- |
| Ventas (VLAN 20) | Administración (VLAN 10) | ❌ **Denegado** | Evita que el personal comercial acceda a información financiera y estratégica. |
| RRHH (VLAN 40) | Ventas (VLAN 20) | ❌ **Denegado** | Protege los datos de nómina del acceso del equipo comercial y viceversa. |
| Cualquier Red | Servidor Web (VLAN 30) | ✅ **Permitido (Solo HTTP)** | Permite la operativa de la página web corporativa, pero protege el servidor de ataques. |
| Cualquier Red | Servidor Web (VLAN 30) | ❌ **Denegado (Ping, SSH, etc.)** | Bloquea cualquier otro intento de acceso al servidor (ping, SSH, FTP). |

---

### 🧠 ¿Por qué es importante?

Este proyecto demuestra mi capacidad para **traducir un requisito legal en una configuración técnica**. La segmentación de la red no es solo una "buena práctica informática"; es una **medida técnica exigida por normativas internacionales**:

| Normativa | Artículo / Anexo | Requisito que cumple |
| :--- | :--- | :--- |
| **GDPR (UE) 2016/679** | Art. 25 y 32 | "Privacidad por Diseño" y medidas técnicas para garantizar la seguridad de los datos. |
| **ISO 27001:2022** | Anexo A.8.22 | Segregación de redes: separar sistemas según el riesgo para controlar el flujo de tráfico. |
| **Directiva NIS2 (UE) 2022/2555** | Art. 21.2 | Medidas de gestión de riesgos de ciberseguridad (control de acceso, seguridad de redes). |

**Al aplicar estos controles, la organización puede:**

1.  **Mitigar el riesgo de filtración de datos:** Limitando el acceso solo al personal autorizado.
2.  **Cumplir con el principio de "Privacidad por Diseño":** Integrando la seguridad en la arquitectura desde el inicio.
3.  **Reducir la superficie de ataque:** Aislando el servidor web y protegiéndolo de accesos no autorizados.
4.  **Demostrar "Responsabilidad Proactiva":** Contar con evidencia técnica de que se han implementado medidas de seguridad exigidas por ley.

---

### 📷 Captura de la Red

![Vista lógica de la red corporativa segmentada](./Topologia.png)

*Figura 1: Vista lógica de la red corporativa segmentada. Cada departamento opera en su propia VLAN, aislada del resto. El router central aplica políticas de firewall (ACLs) para controlar el tráfico entre VLANs.*

---

### 📄 Documentación

📎 [Descargar Informe Ejecutivo en PDF](./Informe-Ciberseguridad.docx)  
*(Incluye análisis de riesgos, implicaciones legales y referencias normativas).*

📎 [Descargar Archivo de Simulación (.pkt)](./Proyecto-ciberseguridad.pkt)  
*(Para visualizar la configuración en Cisco Packet Tracer).*

---

## 📚 Formación Académica

- **LICENCIATURA EN DERECHO** – Universidad Monteávila (2024)
- **TÉCNICO EN INFORMÁTICA Y SEGURIDAD HOST** – Académica Labs (2026)
- **PROGRAMA DE NEGOCIOS PARA GERENCIA** – Harvard Business School Online (2025)
- **MAESTRÍA EN POLÍTICA EXTERIOR** – IAEDPG (En progreso)
- **ESTUDIANTE TÉCNICO EN REDES IP Y CIBERSEGURIDAD** – Académica Labs y Social Oplesk (2026)  
  *(Proyecto práctico: Diseño e implementación de arquitectura de red segmentada con firewall para cumplimiento normativo GDPR/NIS2/ISO 27001)*

---

## 💼 Experiencia Profesional

| Periodo | Cargo | Empresa / Institución |
| :--- | :--- | :--- |
| **2025 - Actualidad** | Abogada | Corporación EMJ27 |
| **2024 - 2025** | Abogada Junior | Deloitte |
| **2024** | Pasante | Ministerio de Relaciones Exteriores de Venezuela |
| **2023** | Pasante | SENIAT |

---

## 🛠️ Habilidades

- **ASESORÍA LEGAL CORPORATIVA:** Gestión integral del ciclo de vida del negocio, desde la constitución hasta la operatividad comercial, asegurando el cumplimiento normativo y la protección de activos.
- **LEGAL FINDER E INTELIGENCIA NORMATIVA:** Monitoreo y análisis exhaustivo de Gacetas Oficiales y boletines legales. Elaboración de resúmenes ejecutivos y opiniones legales sobre tendencias jurídicas actuales.
- **RECOLECCIÓN Y ANÁLISIS DE DATOS:** Elaboración de formularios de Google, curación de datos a través de Excel/PowerBI, y elaboración de dashboards en Excel/PowerBI.
- **INVESTIGACIÓN PROFUNDA:** Búsqueda avanzada de información pública con metodología OSINT y Google Search Operators.
- **ARQUITECTURA DE RED Y CIBERSEGURIDAD:** Comprensión de principios de segmentación de red (VLANs), control de accesos (firewalls/ACLs) y su aplicación para cumplir con normativas de protección de datos y ciberseguridad (GDPR, NIS2, ISO 27001).

---

## 🏆 Reconocimientos y Participaciones

- **Reconocimiento por ICAC:** Ponencia internacional sobre la IA aplicada al Derecho (Perú, 2025).
- **Reconocimiento por la Universidad de El Salvador:** Ponencia internacional "IA aplicada al Derecho" (El Salvador, 2025).

---

## 📝 Artículos Publicados

- *"IA: El Final Boss de la Geopolítica Moderna"*
- *"La Innovación Legal y la Inteligencia Artificial: ¿Cómo la Transformación Digital puede generar Discriminación Algorítmica y Vigilancia Masiva en el Sector Público?"*

---

## 📬 Contacto

📧 [elarhuaa@gmail.com](mailto:elarhuaa@gmail.com)

---

*"La seguridad digital no es solo un problema de ingenieros; es un pilar fundamental del Estado de Derecho en el siglo XXI."*
