<div align="center">

# Sistema de Gestión y Reporte de Mantenimiento de Aires Acondicionados

<img src="https://img.shields.io/badge/Estado-En%20Desarrollo-yellow?style=for-the-badge" alt="Estado">
<img src="https://img.shields.io/badge/Metodolog%C3%ADa-Kanban-blue?style=for-the-badge" alt="Metodología">
<img src="https://img.shields.io/badge/Licencia-GPL-green?style=for-the-badge" alt="Licencia">
<img src="https://img.shields.io/badge/Presupuesto-%240.00%20USD-lightgrey?style=for-the-badge" alt="Presupuesto">

**Plataforma centralizada para el registro, seguimiento y resolución de fallas en equipos de climatización.**

</div>

---

## 1. Planteamiento del Problema y Solución

| Aspecto | Descripción Detallada |
| :--- | :--- |
| **Problemática** | Actualmente los equipos de aire acondicionado presentan fallas recurrentes o dejan de enfriar sin que exista un canal centralizado para reportar las averías. Esto retrasa el mantenimiento correctivo, impide llevar un historial técnico por equipo y afecta el confort en las instalaciones. |
| **Solución Propuesta** | Desarrollar una aplicación web de gestión de activos y reporte de fallas donde los usuarios notifiquen averías en tiempo real (indicando ubicación exacta y tipo de daño) y el personal técnico gestione las órdenes de reparación mediante un tablero de flujo continuo hasta su cierre. |
| **Objetivo General** | Optimizar los tiempos de respuesta del mantenimiento técnico y garantizar la trazabilidad completa de cada equipo de aire acondicionado mediante un sistema web colaborativo. |

---

## 2. Alcance y Módulos del Sistema

| Módulo | Funcionalidades Clave | Usuarios Beneficiados |
| :--- | :--- | :--- |
| **1. Inventario de Equipos** | Registro de cada unidad con código único, marca, ubicación (aula/oficina/piso) y estado operativo (*Operativo*, *Con falla*, *En mantenimiento*). | Administradores y Técnicos |
| **2. Portal de Reportes** | Formulario rápido de notificación de averías (*no enciende, no enfría, gotea agua, ruido extraño*) con nivel de prioridad y observaciones. | Usuarios Generales / Docentes / Personal |
| **3. Panel de Control (Dashboard)** | Visualización de alertas activas, asignación de responsables técnicos y actualización de estados de reparación en tiempo real. | Equipo de Mantenimiento |
| **4. Historial Técnico** | Bitácora por equipo con registro de fallas previas, fechas de intervención, repuestos utilizados y mantenimientos preventivos. | Administradores y Auditores |

---

## 3. Matriz de Recursos del Proyecto

| Categoría | Elementos Asignados | Cantidad | Costo Estimado |
| :--- | :--- | :---: | :---: |
| **Recurso Humano** | • **Cristian Flores** (QA, Historial y Documentación)<br>• **Kevin Vega** (Gestión de Repo y Base de Datos)<br>• **Daleska Guerrero** (Diseño UI/UX y Frontend)<br>• **Lindsay Delgado** (Desarrollo Backend y API) | 4 Integrantes | $0.00 |
| **Recurso Material** | • Computadoras / Laptops personales<br>• Conexión a Internet<br>• Git y GitHub (Control de versiones y Projects)<br>• Visual Studio Code & Figma | 4 Equipos + Software | $0.00 |
| **Recurso Financiero** | • Uso exclusivo de herramientas Open Source y planes gratuitos | — | **$0.00 USD** |

---

## 4. Tablero Kanban y Planificación de Tareas

> **Nota:** El seguimiento en tiempo real de estas tarjetas se gestiona en la pestaña **[Projects](../../projects)** y en **[Issues](../../issues)** de este repositorio (4 issues activos registrados)[cite: 6].

| ID | Integrante | Tiempo | Actividad Asignada | Rama Git | Estado |
| :---: | :--- | :---: | :--- | :---: | :---: |
| **#1** | **Kevin Vega** | `3 días` | Configurar repositorio en GitHub (licencia MIT), estructurar ramas (`main`, `dev`) y diseñar el modelo relacional de base de datos (`Equipos`, `Usuarios`, `Reportes`, `Mantenimientos`). | `feature/setup-db` | En Proceso |
| **#2** | **Daleska Guerrero** | `4 días` | Diseñar prototipos de interfaz (*mockups* en Figma) y programar las vistas del formulario de reporte de fallas y listado de equipos. | `feature/ui-reportes` | Inicio |
| **#3** | **Lindsay Delgado** | `5 días` | Desarrollar la lógica del servidor (API/CRUD) para creación de reportes, cambio de estados de reparación y filtrado de alertas pendientes. | `feature/api-crud` | Inicio |
| **#4** | **Cristian Flores** | `4 días` | Implementar el módulo de historial de mantenimiento, ejecutar pruebas de integración y consolidar la documentación técnica. | `feature/historial-docs` | Inicio |

---

## 5. Flujo de Trabajo y Control de Versiones (Git)

Para mantener el orden del código entre los 4 integrantes, se aplica el siguiente flujo de trabajo:

1. **Rama `main`:** Contiene únicamente versiones estables y aprobadas del proyecto[cite: 6].
2. **Rama `dev`:** Rama de integración donde se unen los avances de cada integrante antes de pasar a producción.
3. **Ramas `feature/*`:** Cada integrante trabaja en su propia rama según la tabla Kanban y abre un **Pull Request (PR)** al finalizar su tarea para revisión del equipo.

---

